# CSS3D Transform Experiments

> Experimental CSS3D transformation effects created in 2015

## Live Demos

**👉 [View All Demos](https://heavenyuan.github.io/poc-css3d/demo.html)**

Or access individual demonstrations:

- [Basic 3D Flip](https://heavenyuan.github.io/poc-css3d/index.html)
- [Double-Sided Card Flip](https://heavenyuan.github.io/poc-css3d/index_2cat.html)
- [3D Carousel](https://heavenyuan.github.io/poc-css3d/index_css3d.html)

## Overview

This is a proof-of-concept project exploring CSS3D Transform capabilities. Created in 2015 as an experimental playground for understanding 3D transformations in CSS, it showcases three different 3D effects using pure CSS and vanilla JavaScript.

## Demonstrations

### 1. Basic 3D Flip (index.html)

Two colored boxes with 3D flip animation triggered by hover.

**Interaction**: Mouse hover
**Technologies**:
- `transform-style: preserve-3d`
- `translateZ()`
- `rotateX()`

**Effect**: The boxes flip in 3D space when you hover over them.

### 2. Double-Sided Card Flip (index_2cat.html)

Two cat images arranged back-to-back with flip animation.

**Interaction**: Click
**Technologies**:
- `rotateY()`
- `backface-visibility`
- CSS transitions

**Effect**: Each click rotates the card 180 degrees, revealing the other side.

### 3. 3D Carousel (index_css3d.html)

15 images arranged in a circular carousel with dynamic rotation.

**Interaction**: Click any image
**Technologies**:
- Circular arrangement (360° / 15)
- Dynamic scaling and opacity based on distance
- Smart rotation (shortest path calculation)

**Effect**: Clicking an image rotates the carousel to bring that image to the center, with smooth transitions and perspective effects.

## Technical Implementation

**Core Technologies:**
- HTML5
- CSS3 Transform
  - `perspective` - Defines viewing distance
  - `transform-style: preserve-3d` - Maintains 3D space
  - `rotateX/rotateY` - 3D rotation
  - `translateZ` - Z-axis translation
- Vanilla JavaScript - Dynamic calculations and interaction logic

**No Frameworks Required**: All effects are achieved with pure CSS and native JavaScript, demonstrating the power of modern web standards (as of 2015).

## Project Structure

```
poc-css3d/
├── demo.html           # Landing page for all demonstrations
├── index.html          # Basic 3D flip demonstration
├── index_2cat.html     # Double-sided card flip
├── index_css3d.html    # 3D carousel
├── arrayIndexOf.js     # Array.indexOf polyfill for older browsers
├── cat.png            # Cat image 1
└── cat2.png           # Cat image 2
```

## Browser Support

Requires modern browsers with CSS3D Transform support:

- Chrome 12+
- Firefox 10+
- Safari 4+
- Edge (all versions)
- IE 10+ (with limited support)

## Usage

1. Open any HTML file directly in a web browser
2. Interact according to each demo:
   - `index.html`: Hover over boxes
   - `index_2cat.html`: Click the card
   - `index_css3d.html`: Click any image

## Historical Context

**Created**: 2015
**Purpose**: Experimental / Proof of Concept

This project was created in 2015 to explore and demonstrate CSS3D Transform capabilities. At that time, CSS3D was still relatively new and not widely understood. This collection of demos served as a learning tool and reference for implementing 3D effects in web applications.

## Legacy

While CSS3D has since become more mainstream with broader browser support and better documentation, these demonstrations remain useful as:
- Simple, focused examples of specific CSS3D techniques
- Reference implementations without framework dependencies
- Educational tools for understanding 3D transform fundamentals

---

**Built in 2015 to explore the possibilities of CSS3D**

## 繁體中文

### 專案簡介

> 2015 年創建的實驗性 CSS3D 轉換效果

## 線上演示

**👉 [立即體驗所有演示](https://heavenyuan.github.io/poc-css3d/demo.html)**

或直接訪問個別演示：

- [基礎 3D 翻轉](https://heavenyuan.github.io/poc-css3d/index.html)
- [雙面卡片翻轉](https://heavenyuan.github.io/poc-css3d/index_2cat.html)
- [3D 旋轉木馬](https://heavenyuan.github.io/poc-css3d/index_css3d.html)

## 專案結構

```
poc-css3d/
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
- **JavaScript** - 動態計算與互動邏輯

## 使用方法

1. 用瀏覽器直接打開任一 HTML 檔案
2. 根據不同檔案的互動方式進行操作：
   - `index.html`: 滑鼠移到方塊上
   - `index_2cat.html`: 點擊圖片
   - `index_css3d.html`: 點擊任一圖片

## 瀏覽器支援

需要支援 CSS3D Transform 的現代瀏覽器：

- Chrome 12+
- Firefox 10+
- Safari 4+
- Edge (所有版本)
