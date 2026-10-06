# ClassMate — College Class App

A mobile-first, installable PWA made with plain HTML, CSS and JavaScript. No coding knowledge is required to use it.

## First version features
- Home dashboard
- Announcements
- Timetable
- Study materials
- Assignments/deadlines
- Faculty information
- Attendance
- Exam information
- Automatic 22-student / 11-pair water duty rotation
- Today duty + previous/upcoming duty list
- Admin editor for class name, student names, duty start date and content
- Offline-friendly PWA caching

## Important
The current version stores information in the browser/device. It is ideal for testing and for a first prototype. It is **not yet a shared multi-user database**: changing an item on one phone does not change it on another phone.

## How to run locally
You need a local web server because service workers do not work from a file:// URL.

If Python is installed:
`python -m http.server 8000`
Then open `http://localhost:8000`.

Or use any static hosting service. Upload all files in this folder.

## Water duty logic
Pair 1 = students 1 & 2; Pair 2 = 3 & 4; ... Pair 11 = 21 & 22. Each calendar day advances one pair. After Pair 11 it returns to Pair 1. The first duty date can be changed from Admin → Water Duty Settings.
