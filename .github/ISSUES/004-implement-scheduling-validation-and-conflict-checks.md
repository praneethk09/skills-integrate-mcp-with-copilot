Title: Implement scheduling validation and conflict checks

Description:
Add server-side checks to validate schedules, avoid overlapping sessions for the same student or instructor, and enforce `max_participants`.

Acceptance criteria:
- Reject signups that exceed `max_participants` with a clear error.
- Prevent duplicate signups and overlapping times for the same student across activities.
- Add utilities to parse schedule strings into structured times or introduce a structured schedule model.
- Unit tests covering conflicts and capacity limits.

Suggested tasks:
- Add schedule parsing helpers in `src/schedule.py`.
- Update signup endpoint to validate capacity and conflicts.
- Add tests in `tests/test_schedule.py`.

Priority: Medium
Estimate: 1-2 days
