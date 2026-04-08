#  CalX: Interactive Calendar Component

A modern, responsive **React-based Interactive Calendar** featuring range selection and integrated note-taking. Designed with a clean “wall calendar” aesthetic and built for speed using **Vite + React + Vanilla CSS**.

[![React](https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB)](https://reactjs.org/)
[![Vite](https://img.shields.io/badge/Vite-646CFF?style=flat-square&logo=vite&logoColor=white)](https://vitejs.dev/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

---

##  Features

###  Calendar UI & Experience
* **Wall Calendar Aesthetic:** Custom hero image header and realistic spiral binding effect.
* **Visual Transitions:** Smooth SVG clip-path flow for a high-end feel.
* **Responsive:** Side-by-side layout for desktop and stacked layout for mobile.

###  Date Range Selection
* **Intuitive Picking:** Select start and end dates with clear visual indicators.
* **Hover Preview:** Visualizes the potential range before you commit to a selection.
* **Visual States:** Circular highlights for terminal dates and rectangular spans for the range.

###  Notes Integration
* **Persistence:** Integrated notes section using `localStorage`.
* **No Backend Needed:** Data remains saved on your device even after a refresh.

---

##  Design & Technical Decisions

### Component Architecture
```text
src/
└── components/
    └── Calendar/
        ├── Calendar.jsx      # Parent state manager
        ├── CalendarGrid.jsx  # Grid logic and date rendering
        ├── Notes.jsx         # LocalStorage handler
        └── HeroImage.jsx     # Aesthetic header component
```
### Tech Stack
Framework: React (via Vite)

Styling: Pure CSS (Grid + Flexbox) — No heavy UI libraries.

State: React useState and useEffect for date logic.

### Run Locally

**Clone the Repo**
   ```bash
   git clone [https://github.com/Amanjeeta21/CalX.git](https://github.com/Amanjeeta21/CalX.git)
   cd CalX
```
**Install Dependencies**
```bash
npm install
```
**Start Development Server**
```bash
npm run dev
```
**Open in Browser**
```bash
Visit http://localhost:5173
```
### Testing the App

Date Selection: Click a start date, then hover over other dates to see the preview.
Persistence: Write a note in the sidebar, refresh the page, and verify the note is still there.
Responsiveness: Use Chrome DevTools to toggle mobile view and check the stacked layout.

### Future Improvements
1) Event scheduling for specific times.
2) Dark Mode support.
3) Drag-and-drop selection functionality.
