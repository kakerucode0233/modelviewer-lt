---
marp: true
paginate: true
theme: gaia
style: | 
    :root {--main-color: #238c3c;}
    section.title {
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        height: 100%;
    }
    img.icon {
        border: 5px solid #000;
        border-radius: 50%;
    }
    section .introduction{
      display: flex;
      flex-direction: column;
    }
    section {
        background-color: white;
        font-family: "Helvetica Neue", Arial, "Hiragino Kaku Gothic ProN","Hiragino Sans", Meiryo, sans-serif;
    }
---
<!-- _class: title -->
# WebGLを使って、
# あまてくのロゴで遊ぼう！

<!--
_color: white
-->
![bg brightness:0.4](title-slide.png)

---
<!-- 
_class: center
 -->
<img src="kirby.jpg" width=250px class="icon">
にっしー

---
## アジェンダ
- はなすこと・はなさないこと
- WebGLとは
- Model Viewerとは
- Model Viewerの使い方
- サンプルコード
---

## はなすこと・はなさないこと

#### はなすこと
- WebGLについて
- htmlでWebGLを実装
- 弊社の応用事例

#### はなさないこと
- バックエンドとか

---

## WebGLとは

WebGLは、ブラウザ上で3Dグラフィックスを描画するためのJavaScript APIです。WebGLを使うことで、ユーザーはWeb上で直感的な3Dコンテンツにアクセスできるようになります。

---

## Model Viewerとは

Model Viewerは、Googleが開発した、Web上で3Dコンテンツを表示するためのフレームワークです。Model Viewerを使うことで、ユーザーはWeb上で高品質な3Dモデルをインタラクティブに操作することができます。

---

## Model Viewerの使い方


1. Model Viewerを読み込む

   ```html
   <script src="https://modelviewer.dev/shared/modelviewer-base.js"></script>
   ```

2. 3Dモデルを表示する

  ```html
  <model-viewer
    src="path/to/model.glb"
    alt="A 3D model"
    camera-controls
  ></model-viewer>
  ```

---

## サンプルコード

```html
  <!DOCTYPE html>
  <html>
    <head>
      <meta charset="utf-8" />
      <title>Model Viewer Example</title>
      <script src="https://modelviewer.dev/shared/modelviewer-base.js"></script>
    </head>
    <body>
      <model-viewer
        src="https://modelviewer.dev/shared-assets/models/Astronaut.glb"
        alt="A 3D model of an astronaut"
        camera-controls
      ></model-viewer>
    </body>
  </html>
