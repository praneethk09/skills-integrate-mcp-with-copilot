Title: Add authentication and role-based authorization (JWT + admin)

Description:
Implement authentication for admin actions and optional Google SSO for convenience. Add role-based authorization (admin vs student) so only authorized users can modify activities and view admin pages.

Acceptance criteria:
- Implement JWT-based auth with login/logout endpoints.
- Add a simple users table with roles (`admin`, `student`).
- Protect admin endpoints (create/edit/delete activities, view participants).
- Optional: implement Google OAuth redirect flow for sign-in.
- Documentation for creating an initial admin user.

Suggested tasks:
- Add `src/auth.py` implementing JWT token creation/verification.
- Add `src/models.py` user model (if not added by storage issue).
- Add decorator/dependency in `src/app.py` to require admin role.
- Update UI to show login flow and protected admin UI.

Priority: High
Estimate: 1-2 days
