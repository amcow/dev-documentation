---
label: Log In Page
order: 997
icon: key
---

## USER LOGIN PAGE FLOW CHART

**Option 1: Login with Magic Link**

**Start**

1. User arrives at login page.
2. User enters their email address.

- **Yes:** Validate email format (optional).

1. System generates a unique magic link with an embedded token and sends it to the user's email.
2. User receives an email with a link titled "Log In to \[Your App Name\]".

- **No:** Display error message (e.g., "Invalid email address"). End path.

1. User clicks the magic link in their email.

- **Yes:** Proceed.
- **No:** (Optional) Track that the link wasn't clicked (e.g., for analytics). End path.

1. System verifies the magic link token and checks for expiration (optional).

- **Valid and not expired:** Proceed.
- **Invalid or expired:** Display error message (e.g., "Invalid or expired link. Please request a new one"). End path.

1. System retrieves user information associated with the email address.
2. **Valid user:** Redirect user to the main application dashboard.

- **Invalid user:** (Optional) Handle situation (e.g., display message "Email not found. Please sign up").

**Option 2: Login with Oauth (Google/Facebook etc.)**

**Start**

1. User arrives at login page.
2. User chooses "Login with \[Provider name\] (e.g., Google, Facebook)".
3. User is redirected to the chosen provider's login page.
4. User logs in to their chosen provider account (if not already logged in).
5. User grants permission to the application to access some of their profile information (e.g., name, email).
6. The chosen provider redirects the user back to your application with an authorization code.
7. Your application exchanges the authorization code with the chosen provider for an access token.
8. Your application uses the access token to retrieve the user's profile information from the chosen provider.
9. **Valid user:** Based on the retrieved information, your application:
    - Links the user account to the chosen provider account (if a new user).
    - Authenticates the user and redirects them to the main application dashboard.

- **Invalid user:** (Optional) Handle situation (e.g., display message "Email not found. Please sign up").

**End** (for both options)