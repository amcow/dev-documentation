---
label: Sign Up Page
order: 996
icon: lock
---

# SIGN UP PAGE WITH MAGIC LINK

**Start**

1. User arrives at the sign-up page.
2. User enters their email address.

- **Yes:** Validate email format (optional).

1. System generates a unique magic link with an embedded token and sends it to the user's email.
2. User receives an email with a link titled "Sign Up to \[Your App Name\]".

- **No:** Display error message (e.g., "Invalid email address"). End path.

1. User clicks the magic link in their email.

- **Yes:** Proceed.
- **No:** (Optional) Track that the link wasn't clicked (e.g., for analytics). End path.

1. System verifies the magic link token and checks for expiration (optional).

- **Valid and not expired:** Proceed.
- **Invalid or expired:** Display error message (e.g., "Invalid or expired link. Please request a new one"). End path.

1. **New User:**
    - Display profile completion form with fields for:
        - Full Name (required)
        - Username (required)
        - Organization (required)
        - Bio (optional)
    - User enters profile information.
    - **Yes:** Validate required fields (full name, username, organization).

- **Existing User:** (Optional) If the email address is associated with an existing account, handle it appropriately (e.g., display message "Email already in use. Please sign in").

1. **Valid information:** System creates a new user account with the provided information.
2. **Profile complete:** Redirect user to the main application dashboard.

**End**