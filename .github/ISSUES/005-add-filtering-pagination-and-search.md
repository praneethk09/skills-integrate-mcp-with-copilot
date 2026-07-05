Title: Add filtering, pagination and search to activities API

Description:
Enable efficient browsing for many activities by adding pagination, filtering by area/schedule/availability, and search by name/description.

Acceptance criteria:
- Replace current `/activities` response with paginated results or add query params (`page`, `limit`).
- Implement search (`q`) to match name/description.
- Add filters for `area`, `day`, and `availability` (open spots only).
- Update front-end to request and display paginated results.

Suggested tasks:
- Add `src/lib/pagination.py` and search helpers.
- Update endpoints to accept query parameters and return metadata (`total`, `page`, `per_page`).
- Update `static/app.js` to show pagination controls.

Priority: Medium
Estimate: 1-2 days
