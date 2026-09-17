# TuteDude-Courses-Data

This repository contains the structured JSON data for all TuteDude courses. 

## Structure

- `courses.json`: The master index containing a summary of all available courses, their IDs, pricing, and active status.
- `{course_slug}.json`: Individual files for each specific course (e.g., `python.json`, `canva.json`), detailing the complete curriculum, lecture URLs, mentor assignments, and other rich metadata.

## Data Schema Updates
- **HLS Video Transition:** The legacy `tpStreamId` video IDs have been migrated to absolute HLS video paths (`videoUrl`).
- **Standardized Formatting:** All JSON files have been strictly pretty-printed (4 spaces) and synchronized with frontend metadata requirements.
- **Lecture Length Standardization:** `lectureLength` values have been formatted to a standard `HH:MM:SS` layout for better cross-platform rendering.
