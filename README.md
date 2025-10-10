# Quiz-list | 考卷清單管理系統

一個功能完整的考卷清單管理系統，具備到期日追蹤、日曆匯出及番茄鐘計時功能。使用原生 JavaScript 開發，專為學生追蹤考試準備進度而設計。

## 🌟 功能特色

### 核心功能
- **✅ 考卷追蹤**：新增、編輯和刪除考卷，包含科目、章節和題數
- **📅 到期日管理**：設定並追蹤考卷的到期日期
- **✓ 進度追蹤**：標記考卷為已完成並追蹤訂正進度
- **🔍 搜尋與篩選**：依科目/章節搜尋，並依到期日狀態篩選
- **📊 進度視覺化**：視覺化的進度條顯示完成和訂正率
- **📈 統計摘要**：即時顯示剩餘和已完成的題數統計

### 進階功能
- **📥 日曆匯出**：將單一或全部考卷匯出為 `.ics` 日曆檔案
- **📤 資料匯出/匯入**：以 JSON 格式匯出和匯入考卷資料
- **📄 PDF 匯出**：產生考卷清單的 PDF 快照（僅限 New.html）
- **⏱️ 番茄鐘計時器**：內建番茄鐘計時器，可自訂工作/休息間隔
- **🎨 深色模式**：在淺色和深色主題之間切換
- **💾 本地儲存**：自動將資料儲存在瀏覽器的 localStorage 中
- **📱 響應式設計**：適合行動裝置的使用者介面

## 📁 檔案說明

### New.html
**最新且功能最豐富的版本**。

**功能：**
- 完整的考卷管理系統
- 智慧型到期日追蹤和篩選
- 日曆匯出（.ics 格式）
- JSON 匯出/匯入
- **PDF 匯出**功能
- 整合的番茄鐘計時器與全螢幕模式
- 卡片檢視和清單檢視切換
- 深色模式支援
- 訂正進度追蹤
- 本地資料持久化

**適合使用情境：** 日常使用和完整的考試追蹤

### Test.html
測試/開發版本，與 New.html 類似，但具有略微不同的功能或實驗性變更。

**功能：**
- 與 New.html 類似的功能集
- 可能包含實驗性功能
- 適合在實作到主版本前進行測試

### Old.html
**簡易的純文字版本**考卷清單。

**功能：**
- 純文字格式
- 靜態考卷清單顯示
- 無 JavaScript - 純 HTML
- 輕量且極簡

**適合使用情境：** 快速參考或列印簡易清單

## 🚀 使用指南

### 開始使用

1. **開啟應用程式**： 
   - 造訪：https://quizlist.techtools.qzz.io
   - 或在瀏覽器中本地開啟 `New.html`

2. **新增考卷**：
   - 填寫科目、章節和題數
   - 可選擇性地新增到期日
   - 點擊「+」按鈕或按 Enter 鍵

3. **管理考卷**：
   - 點擊 ✓ 標記為已完成
   - 點擊「訂正」標記訂正完成
   - 點擊「編輯」編輯考卷詳細資訊
   - 點擊「刪除」刪除考卷
   - 點擊「匯出日曆」匯出到日曆

### 功能詳細說明

#### 搜尋與篩選
- 使用搜尋框依科目或章節尋找考卷
- 篩選下拉選單選項：
  - **全部**：顯示所有考卷
  - **今天到期**：今天到期的考卷
  - **本週到期**：本週到期的考卷
  - **已逾期**：已過期的考卷
  - **無標示到期日**：沒有設定到期日的考卷

#### 排序
- **依章節排序**：依字母順序排序
- **依題數排序**：依數字大小排序
- **依到期日排序**：依日期排序

#### 番茄鐘計時器
1. 點擊「顯示番茄鐘」顯示計時器
2. 選擇要與番茄鐘工作階段關聯的考卷
3. 選擇計時器模式：番茄鐘（25 分鐘）、短休息（5 分鐘）或長休息（15 分鐘）
4. 點擊「開始」啟動
5. 如需要可啟用聲音通知
6. 使用全螢幕模式以專注學習

#### 匯出選項
- **匯出全部到日曆**：將所有有到期日的考卷匯出為單一 .ics 檔案
- **匯出 JSON**：將資料備份為 JSON 格式
- **匯出 PDF**：產生 PDF 快照（僅限 New.html）
- 每個考卷都可個別匯出日曆

#### 匯入資料
1. 點擊「匯入 JSON」
2. 選擇先前匯出的 JSON 檔案
3. 資料將被載入並合併

## 🎯 使用情境

- **學生**：追蹤考試準備和學習時段
- **教師**：管理測驗時程和追蹤訂正狀況
- **自學者**：整理練習題目和追蹤進度
- **考試準備**：監控多個科目的準備進度

## 💻 技術細節

### 技術堆疊
- 純 HTML5/CSS3/JavaScript（原生 JS）
- 不需要後端 - 完全在瀏覽器中執行
- 使用 LocalStorage 儲存資料
- 外部函式庫：
  - jsPDF（用於 New.html 中的 PDF 生成）
  - html2canvas（用於 New.html 中的 PDF 渲染）

### 瀏覽器相容性
- 現代瀏覽器（Chrome、Firefox、Safari、Edge）
- 需要啟用 JavaScript
- 需要支援 LocalStorage

### 資料儲存
所有資料都使用 `localStorage` 儲存在您的瀏覽器本地。您的資料：
- ✅ 隱私（絕不會傳送到任何伺服器）
- ✅ 持久化（瀏覽器重啟後仍保留）
- ⚠️ 瀏覽器專屬（不會跨裝置同步）
- ⚠️ 可能會隨瀏覽器資料一起被清除

### 資料格式
考卷以下列 JSON 結構儲存：
```json
{
  "id": "unique-id",
  "subject": "科目名稱",
  "chapter": "章節",
  "questions": 50,
  "completed": false,
  "corrected": false,
  "dueDate": "2025-10-15"
}
```

## 🔧 自訂設定

### 修改預設資料
編輯 HTML 檔案中的 `initialData` 陣列以變更預設的考卷清單。

### 主題設定
應用程式使用 CSS 變數以便於調整主題。修改 `:root` 和 `.dark-mode` 變數以自訂顏色。

### 番茄鐘設定
在 `durations` 物件中調整計時器時長：
```javascript
durations: { pom: 25*60, short: 5*60, long: 15*60 }
```

## 📱 行動裝置支援

所有版本都是響應式的，可在行動裝置上運作。介面會針對較小的螢幕進行調整：
- 在窄螢幕上採用堆疊式佈局
- 觸控友善的按鈕
- 響應式字體
- 最佳化的番茄鐘計時器顯示

## 🤝 貢獻指南

歡迎貢獻！您可以：
- 回報錯誤
- 建議新功能
- 提交拉取請求
- 改善文件

## 📄 授權條款

此專案為開源專案。歡迎自由使用和修改以符合您的需求。

## 🌐 線上展示

造訪線上應用程式：https://quizlist.techtools.qzz.io

---



---

# Quiz-list | Exam List Management System

A comprehensive exam/quiz list management system with due date tracking, calendar export, and Pomodoro timer features. Built with vanilla JavaScript for students to track their exam preparation progress.

## 🌟 Features

### Core Features
- **✅ Exam Tracking**: Add, edit, and delete exams with subject, chapter, and question counts
- **📅 Due Date Management**: Set and track exam due dates
- **✓ Progress Tracking**: Mark exams as completed and track correction progress
- **🔍 Search & Filter**: Search by subject/chapter and filter by due date status
- **📊 Progress Visualization**: Visual progress bars showing completion and correction rates
- **📈 Statistics Summary**: Real-time statistics on remaining and completed questions

### Advanced Features
- **📥 Calendar Export**: Export individual or all exams to `.ics` calendar files
- **📤 Data Export/Import**: Export and import exam data as JSON
- **📄 PDF Export**: Generate PDF snapshots of your exam list (New.html only)
- **⏱️ Pomodoro Timer**: Built-in Pomodoro timer with customizable work/break intervals
- **🎨 Dark Mode**: Toggle between light and dark themes
- **💾 Local Storage**: Automatically saves your data in browser localStorage
- **📱 Responsive Design**: Mobile-friendly interface

## 📁 Files

### New.html
The **latest and most feature-rich version** of the application.

**Features:**
- Complete exam management system
- Due date tracking with smart filtering
- Calendar export (.ics format)
- JSON export/import
- **PDF export** functionality
- Integrated Pomodoro timer with fullscreen mode
- Card view and list view toggle
- Dark mode support
- Correction progress tracking
- Local data persistence

**Best for:** Daily use and comprehensive exam tracking

### Test.html
A testing/development version similar to New.html with slightly different features or experimental changes.

**Features:**
- Similar feature set to New.html
- May include experimental features
- Useful for testing before implementing in the main version

### Old.html
The **simple, text-based version** of the exam list.

**Features:**
- Plain text format
- Static exam list display
- No JavaScript - pure HTML
- Lightweight and minimalist

**Best for:** Quick reference or printing a simple list

## 🚀 Usage

### Getting Started

1. **Open the application**: 
   - Visit: https://quizlist.techtools.qzz.io
   - Or open `New.html` in your web browser locally

2. **Add an exam**:
   - Fill in Subject (科目), Chapter (章節), and Questions (題數)
   - Optionally add a due date (到期日)
   - Click the "+" button or press Enter

3. **Manage exams**:
   - Click ✓ to mark as completed
   - Click "訂正" to mark corrections as done
   - Click "編輯" to edit exam details
   - Click "刪除" to delete an exam
   - Click "匯出日曆" to export to calendar

### Features Guide

#### Search & Filter
- Use the search box to find exams by subject or chapter
- Filter dropdown options:
  - **全部** (All): Show all exams
  - **今天到期** (Due Today): Exams due today
  - **本週到期** (Due This Week): Exams due this week
  - **已逾期** (Overdue): Past due exams
  - **無標示到期日** (No Due Date): Exams without due dates

#### Sorting
- **依章節排序** (Sort by Chapter): Alphabetical sorting
- **依題數排序** (Sort by Questions): Numerical sorting
- **依到期日排序** (Sort by Due Date): Date-based sorting

#### Pomodoro Timer
1. Click "顯示番茄鐘" to show the timer
2. Select an exam to associate with your Pomodoro session
3. Choose timer mode: Pomodoro (25min), Short Break (5min), or Long Break (15min)
4. Click "開始" to start
5. Enable sound notifications if desired
6. Use fullscreen mode for distraction-free focus

#### Export Options
- **匯出全部到日曆** (Export All to Calendar): Exports all exams with due dates to a single .ics file
- **匯出 JSON** (Export JSON): Backup your data as JSON
- **匯出 PDF** (Export PDF): Generate a PDF snapshot (New.html only)
- Individual calendar export available per exam

#### Import Data
1. Click "匯入 JSON" (Import JSON)
2. Select your previously exported JSON file
3. Data will be loaded and merged

## 🎯 Use Cases

- **Students**: Track exam preparation and study sessions
- **Teachers**: Manage quiz schedules and track corrections
- **Self-learners**: Organize practice problems and track progress
- **Test Prep**: Monitor progress across multiple subjects

## 💻 Technical Details

### Technology Stack
- Pure HTML5/CSS3/JavaScript (Vanilla JS)
- No backend required - runs entirely in browser
- LocalStorage for data persistence
- External libraries:
  - jsPDF (for PDF generation in New.html)
  - html2canvas (for PDF rendering in New.html)

### Browser Compatibility
- Modern browsers (Chrome, Firefox, Safari, Edge)
- Requires JavaScript enabled
- Requires LocalStorage support

### Data Storage
All data is stored locally in your browser using `localStorage`. Your data is:
- ✅ Private (never sent to any server)
- ✅ Persistent (survives browser restarts)
- ⚠️ Browser-specific (not synced across devices)
- ⚠️ Can be cleared with browser data

### Data Format
Exams are stored as JSON with the following structure:
```json
{
  "id": "unique-id",
  "subject": "科目名稱",
  "chapter": "章節",
  "questions": 50,
  "completed": false,
  "corrected": false,
  "dueDate": "2025-10-15"
}
```

## 🔧 Customization

### Modifying Default Data
Edit the `initialData` array in the HTML file to change the default exam list.

### Theming
The application uses CSS variables for easy theming. Modify the `:root` and `.dark-mode` variables to customize colors.

### Pomodoro Settings
Adjust timer durations in the `durations` object:
```javascript
durations: { pom: 25*60, short: 5*60, long: 15*60 }
```

## 📱 Mobile Support

All versions are responsive and work on mobile devices. The interface adapts to smaller screens with:
- Stacked layouts on narrow screens
- Touch-friendly buttons
- Responsive typography
- Optimized Pomodoro timer display

## 🤝 Contributing

Contributions are welcome! Feel free to:
- Report bugs
- Suggest new features
- Submit pull requests
- Improve documentation

## 📄 License

This project is available as open source. Feel free to use and modify for your own purposes.

## 🌐 Live Demo

Access the live application at: https://quizlist.techtools.qzz.io

---

