# CSS3D-TEST

CSS 3D 變換效果展示專案，包含多個 3D 互動範例。

## 專案結構

```
CSS3D-TEST/
├── index.html          # 基礎 3D 翻轉效果
├── index_2cat.html     # 雙面卡片翻轉
├── index_css3d.html    # 3D 旋轉木馬
├── arrayIndexOf.js     # Array.indexOf polyfill
├── cat.png            # 貓咪圖片 1
└── cat2.png           # 貓咪圖片 2
```

## 功能展示

### 1. index.html - 基礎 3D 翻轉
- 兩個方塊的 3D 翻轉動畫
- **互動方式**: 滑鼠懸停 (hover)
- **技術**: `transform-style: preserve-3d`, `translateZ()`, `rotateX()`

### 2. index_2cat.html - 雙面卡片翻轉
- 兩張貓咪圖片的背對背旋轉
- **互動方式**: 點擊卡片
- **技術**: `rotateY()`, `backface-visibility`
- **效果**: 每次點擊旋轉 180 度

### 3. index_css3d.html - 3D 旋轉木馬
- 15 張圖片環繞排列的旋轉木馬
- **互動方式**: 點擊任意圖片
- **技術**:
  - 圓周排列計算 (360° / 15)
  - 動態縮放和透明度 (距離中心越遠越小)
  - 智能旋轉方向 (選擇最短路徑)
- **效果**: 點擊後該圖片會旋轉至正中央

## 技術棧

- **HTML5**
- **CSS3 Transform**
  - `perspective` - 透視距離
  - `transform-style: preserve-3d` - 保持 3D 空間
  - `rotateX/rotateY` - 3D 旋轉
  - `translateZ` - Z 軸位移
- **jQuery 1.11.2**
- **JavaScript** - 動態計算與互動邏輯

## 使用方法

1. 用瀏覽器直接打開任一 HTML 檔案
2. 根據不同檔案的互動方式進行操作：
   - `index.html`: 滑鼠移到方塊上
   - `index_2cat.html`: 點擊圖片
   - `index_css3d.html`: 點擊任一圖片

## 核心原理

### 旋轉木馬 (index_css3d.html)

```javascript
// 圓周排列
var n = 15;                    // 圖片數量
var l = 20 * n;                // 半徑 (300px)
var r = 360 / n;               // 每張圖片間隔角度 (24°)

// 動態縮放計算
function mathScale(angle) {
  return (Math.abs((180 - (Math.abs(angle) % 360)) / 180)) * 0.5 + 0.5;
}

// Transform 組合
transform: rotateX(-5deg) rotateY(angle) translateZ(300px) scale(s)
```

## 瀏覽器支援

需要支援 CSS3D Transform 的現代瀏覽器：
- Chrome 12+
- Firefox 10+
- Safari 4+
- Edge (所有版本)

## 注意事項

- 依賴外部資源: `../reset.css`, `../js/jquery-1.11.2.min.js`
- 確保圖片檔案 (`cat.png`, `cat2.png`) 存在
