# Quiz-list | 考卷清單管理系統

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

**Made with ❤️ for students and learners**