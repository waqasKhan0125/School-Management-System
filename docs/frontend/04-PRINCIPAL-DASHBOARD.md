# Principal Dashboard

## Visual layout
Match `reference-images/02-dashboard-reference.jpg`:
- Left navy sidebar.
- Large `Dashboard` title and a one-line greeting/date beneath.
- Top-right actions aligned horizontally where space allows.
- Four main cards in a two-column/two-row grid on desktop.
- Card 1 top-left: Students Overview with a large total, supporting caption, month comparison only if valid data exists, and school-level distribution chips if configured.
- Card 2 top-right: Attendance Rate with a prominent circular progress ring, percentage centered inside, present/absent count underneath, and comparison only if valid historical data exists.
- Card 3 bottom-left: Classes with a large active-class count and small class/level breakdown chips.
- Card 4 bottom-right: replace reference's `Upcoming Events` with a useful SchoolFlow summary such as Fee Collection or Exam/Results Overview. Do not create an events module just to copy sample content.

## Header actions
- `Add Student`: visible only if the Principal has create-student permission (Principal normally has it).
- `Export Report`: opens the report/export flow; do not make a fake download.

## Data rules
- Never hard-code the reference values `1,284`, `92%`, `1,180`, `104`, or `24` as live results.
- Show actual API/database values when available.
- While the backend is not implemented, use clearly isolated mock data and label the app as demo/development mode.
- Handle empty school data gracefully (e.g. zero students/classes, no attendance recorded).
- Date format should follow selected language/locale.

## Interactions
Cards may link to their relevant modules when user permission allows it. Charts must include readable text equivalents; color alone must not convey status. All action buttons must work or be clearly disabled with an explanation.