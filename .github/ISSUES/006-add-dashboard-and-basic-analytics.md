Title: Add dashboard and basic analytics for admin users

Description:
Provide a dashboard page with key metrics: total activities, total signups, activities near capacity, and recent signups.

Acceptance criteria:
- Add backend endpoints or aggregations to compute metrics.
- Add an admin dashboard page showing charts/tables of metrics.
- Protect dashboard behind admin auth.

Suggested tasks:
- Add `src/analytics.py` with aggregation helpers.
- Add `static/admin-dashboard.html` or extend admin UI with charts (Chart.js or simple tables).

Priority: Low
Estimate: 1-2 days
