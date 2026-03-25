# Requirements Specification — PolyLine Editor

## 1) Problem statement
Create a browser-based polyline drawing and editing tool (Canvas) that allows users to create and edit pictures made from up to **100 polylines** using keyboard commands and mouse input.

## 2) Users
- HCI students / users needing a lightweight line editor
- Users who need quick draw/edit without installing software

## 3) Functional Requirements (FR)
FR1 — Begin polyline (`b` / Begin button)  
- The system shall create a new polyline and make it active.

FR2 — Add points (mouse click in draw mode)  
- The system shall add a new vertex at the clicked location to the active polyline.

FR3 — Finish polyline (`f` / double-click)  
- The system shall finish a polyline if it contains at least 2 points.

FR4 — Move point (`m`)  
- The system shall allow dragging the closest point to a new location.

FR5 — Delete point (`d`)  
- The system shall delete the closest point and reconnect adjacent segments.

FR6 — Refresh (`r`)  
- The system shall clear and redraw all polylines from the data structure.

FR7 — Quit (`q`)  
- The system shall exit/quit the session (web version: clear/reset or disable interaction).

FR8 — Save/Load (`s` / `l`) [extension but useful]  
- The system shall save polylines to JSON and load from JSON.

FR9 — Insert point (`i`) [extension hinted by prompt]  
- The system shall insert a new point by clicking on a segment.

## 4) Non-Functional Requirements (NFR)
NFR1 — Usability  
- Must show current mode and provide status feedback.

NFR2 — Performance  
- Must remain responsive for up to 100 polylines with typical point counts.

NFR3 — Learnability  
- Must include help/shortcut guide.

## 5) Constraints
- Runs fully in browser (HTML/CSS/JS, canvas).
- No backend required.
