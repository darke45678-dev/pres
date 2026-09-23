# FridgeAI 專案技術簡報與演講系統 (Presentation Deck)

> 專為家庭廚房與邊緣運算設計的「零伺服器成本 · 100% 隱私保護」食材感知與智慧管理系統技術簡報。

---

## 🌐 線上展示與部署網址 (Live Links)

* 🖥️ **專案官方技術簡報 (Presentation Slides)**  
  👉 [https://darke45678-dev.github.io/pres/](https://darke45678-dev.github.io/pres/)
  * 支援鍵盤方向鍵（`←` / `→` / `Space`）翻頁
  * 支援手機滑動（Swipe）翻頁
  * 置中自適應放大排版，純淨白話展示

* 🎙️ **面試雙螢幕提詞系統 (Dual-Screen Teleprompter)**  
  👉 [https://darke45678-dev.github.io/pres/speech_presentation.html](https://darke45678-dev.github.io/pres/speech_presentation.html)
  * 左側：簡報投影預覽
  * 右側：對應 10 頁的口語逐字講稿與時間提醒

---

## 📊 專案技術亮點一覽

1. **零伺服器成本 (0 Server Cost)**：YOLO 模型轉 ONNX FP16 半精度量化（26MB $\rightarrow$ 13MB，瘦身 50%），利用 WebGL 在瀏覽器純本地 45ms 極速推論。
2. **5,560 張真實照片與三階資料劃分**：87% 訓練集、9% 驗證集、4% 盲測測試集。
3. **多維影像增強提升泛化能力**：導入 Mosaic（抗遮擋）、Mixup（抗反光與霧氣）、HSV 抖動（抗黃白燈光與手影）。
4. **定位懲罰調優**：調高 Box Loss 懲罰（$\lambda_{box} = 7.5$），精準鎖定食材發黑發霉邊緣，達成 86.8% mAP@50 與腐壞肉類 100% 滿分辨識率。
5. **前端體驗優化**：手勢操作鎖防誤觸、200% RWD 彈性排版、iOS 60 FPS 順暢算圖。

---

## 🚀 部署說明 (Deployment)

本專案由 GitHub Actions 自動建置並部署至 GitHub Pages。
