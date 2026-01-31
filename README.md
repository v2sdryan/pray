# 靈修日記 | Meditation Diary

這是一個受郇山堂 (https://shunshan.org.hk/) 風格啟發的靈修日記網站。每日可以上傳靈修圖片和音頻，配合日曆瀏覽。

This is a meditation diary website inspired by the style of Shun Shan Church (郇山堂).
Upload daily meditation images and audio files, browse them with a calendar interface.

## 🌟 特點 Features

- 📅 **左側日曆**：輕鬆瀏覽每日靈修記錄
- 🖼️ **圖片展示**：顯示每日 WhatsApp 圖片
- 🎵 **音頻播放**：播放每日靈修音頻
- 📱 **響應式設計**：支持手機和桌面瀏覽
- 🎨 **郇山堂風格**：溫暖、典雅的設計風格

## 📁 檔案結構 File Structure

```
靈修日記/
├── index.html          # 主頁面
├── media/              # 存放媒體檔案
│   ├── WhatsApp Image 2026-01-31.jpg
│   ├── WhatsApp Audio 2026-01-31.mp3
│   ├── WhatsApp Image 2026-02-01.jpg
│   ├── WhatsApp Audio 2026-02-01.mp3
│   └── ...
└── README.md           # 說明文件
```

## 📝 檔案命名規則 File Naming Convention

- **圖片**：`WhatsApp Image YYYY-MM-DD.jpg`
  - 範例：`WhatsApp Image 2026-01-31.jpg`
  
- **音頻**：`WhatsApp Audio YYYY-MM-DD.mp3`
  - 範例：`WhatsApp Audio 2026-01-31.mp3`

## 🚀 如何上傳到 GitHub How to Upload to GitHub

### 步驟 1：創建 GitHub 倉庫

1. 登入 [GitHub](https://github.com)
2. 點擊右上角的 **+** 按鈕，選擇 **New repository**
3. 輸入倉庫名稱，例如：`meditation-diary`
4. 選擇 **Public**（公開）
5. 勾選 **Add a README file**
6. 點擊 **Create repository**

### 步驟 2：上傳檔案

#### 方法一：使用 GitHub 網頁上傳

1. 在新創建的倉庫頁面，點擊 **Add file** → **Upload files**
2. 將 `index.html` 檔案拖放到上傳區域
3. 點擊 **Commit changes**

#### 方法二：使用 Git 命令列

```bash
# 克隆倉庫到本地
git clone https://github.com/YOUR_USERNAME/meditation-diary.git

# 進入倉庫目錄
cd meditation-diary

# 創建 media 資料夾
mkdir media

# 複製你的 index.html 和媒體檔案
cp /path/to/index.html .
cp /path/to/WhatsApp\ Image\ 2026-01-31.jpg media/
cp /path/to/WhatsApp\ Audio\ 2026-01-31.mp3 media/

# 添加檔案
git add .

# 提交更改
git commit -m "Initial commit: Add meditation diary website"

# 推送到 GitHub
git push origin main
```

### 步驟 3：啟用 GitHub Pages

1. 在倉庫頁面，點擊 **Settings**（設定）
2. 左側選單選擇 **Pages**
3. 在 **Source** 部分，選擇 **Deploy from a branch**
4. 選擇 **main** 分支，資料夾選擇 **/(root)**
5. 點擊 **Save**
6. 等待幾分鐘，網站就會發布在 `https://YOUR_USERNAME.github.io/meditation-diary`

## 📱 如何使用 How to Use

### 每日上傳新內容

1. 準備好你的圖片和音頻檔案
2. 按照命名規則重新命名：
   - `WhatsApp Image 2026-01-31.jpg`
   - `WhatsApp Audio 2026-01-31.mp3`
3. 上傳到 `media/` 資料夾：
   - 使用 GitHub 網頁：點擊 media 資料夾 → Upload files
   - 或使用 Git：複製檔案到 media/ 資料夾，然後 `git add . && git commit -m "Add 2026-01-31" && git push`
4. 等待 GitHub Pages 自動更新（約 1-2 分鐘）
5. 刷新網站查看新內容

### 在網站上瀏覽

1. 打開網站 URL
2. 點擊左側日曆上的日期
3. 右側會顯示該日期的圖片和音頻
4. 如果該日期沒有內容，會顯示提示訊息

## 🎨 自定義 Customization

### 修改顏色主題

在 `index.html` 的 `<style>` 部分，修改 CSS 變數：

```css
:root {
    --bg: #f5f0e8;        /* 背景色 */
    --fg: #3a3a3a;        /* 文字色 */
    --accent: #8b7355;    /* 強調色 */
    --card: #181c25;      /* 卡片色 */
}
```

### 修改標題

在 `<header>` 部分修改：

```html
<div class="header">
    <h1>你的標題</h1>
    <p>你的副標題</p>
</div>
```

## 🔧 技術說明 Technical Notes

- **純 HTML/CSS/JS**：不需要伺服器端程式
- **GitHub Pages**：免費靜態網站託管
- **日曆功能**：使用原生 JavaScript 生成
- **檔案加載**：自動檢查 media/ 資料夾中的檔案
- **響應式**：使用 CSS Flexbox 和 Grid

## ⚠️ 注意事項 Notes

1. **檔案大小限制**：GitHub 免費帳戶有 1GB 儲存限制
2. **音頻格式**：目前只支持 MP3 格式
3. **圖片格式**：建議使用 JPG 或 JPEG 格式
4. **瀏覽器**：建議使用 Chrome、Firefox、Safari 或 Edge

## 📞 支援 Support

如有問題，請在 GitHub 倉庫開啟 Issue。

For issues, please open an issue in the GitHub repository.

---

願平安與你同在 🙏
