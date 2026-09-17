# TuteDude-Courses-Data

This repository contains the structured JSON data for all TuteDude courses, automatically hosted and served via GitHub Pages.

## API Documentation

You can fetch the course data directly using our public API endpoints (served via GitHub Pages).

### Base URL
`https://epowerx-labs-private-limited.github.io/TuteDude-Courses-Data/`

### 1. All Courses Listing
Fetch a summary of all available courses, their IDs, pricing, and active status.
- **Endpoint:** [`/courses.json`](https://epowerx-labs-private-limited.github.io/TuteDude-Courses-Data/courses.json)
- **Method:** `GET`

### 2. Specific Course Content
Fetch the complete curriculum, lecture URLs, mentor assignments, and other rich metadata for a specific course.
- **Endpoint:** `/{folderName}/{course_slug}.json`
- **Method:** `GET`
- **Example:** [`/DSA/dsawithjava.json`](https://epowerx-labs-private-limited.github.io/TuteDude-Courses-Data/DSA/dsawithjava.json)

> **Note:** The `folderName` refers to the category folder the course belongs to (e.g., `AI & ML`, `Design`, `Software Development`, etc.). Make sure to URL-encode the folder name in your requests (e.g., `AI%20%26%20ML`).

---

## Data Schema
- **HLS Video Transition:** The legacy `tpStreamId` video IDs have been migrated to absolute HLS video paths (`videoUrl`).
- **Standardized Formatting:** All JSON files are strictly pretty-printed (4 spaces) and synchronized with frontend metadata requirements.
- **Lecture Length Standardization:** `lectureLength` values are formatted to a standard `HH:MM:SS` layout for seamless cross-platform rendering.
- **Course Images:** `courses.json` dynamically assigns a `courseimage` asset path to each course.
