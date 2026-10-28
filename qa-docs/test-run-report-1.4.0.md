# Test run report: Regression 1.4.0

**Run:** Regression 1.4.0 – Contact Form, Booking, Admin Rooms

**Build / env / date:** 1.4.0 / test / Chrome 130 / 2026-10-28

**Scope:** Contact form validation, room booking, admin room management, and authentication.

**Results:** Total: 13 | Passed: 6 | Failed: 5 | Blocked: 1 | Untested: 1

**Bugs (severity pending confirmation):**

- BUG-1 (Open): Duplicate room numbers are allowed.
- BUG-2 (Open): Double-clicking Book creates duplicate bookings.
- BUG-3 (Open): Booking with checkout before check-in is accepted.
- BUG-4 (Reopened): Expired token returns 500 instead of 401; no login redirect.
- BUG-5 (New): A 100-character subject causes HTTP 500.
- BUG-6 (New): Intermittent email delivery failure found in logs.

**Not tested and why:** TC-06 blocked due to missing mailbox access; TC-11 untested due to time limitations.

**Risks:** Invalid and duplicate bookings may affect customers.

**Recommendation:** Do not release build 1.4.0 until critical issues are fixed and retested.