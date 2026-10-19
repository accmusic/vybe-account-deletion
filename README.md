# VYBE — eliminar cuenta / delete account / видалити акаунт

Static page for deleting a VYBE account (Google Play account deletion requirement).

- Only static files: `index.html` with inline CSS and JavaScript, no libraries, no external resources, no analytics, no cookies.
- Contains only public values of the Supabase project: the project URL and the **publishable** key. No secret or service role keys.
- The user signs in with email and password (Supabase Auth); the page then calls the `delete-account` Edge Function, which re-checks the password and deletes the account. Nothing is stored in the browser.
- Fallback: a request by email to the support address shown on the page.

Languages: Spanish (default), English, Ukrainian (`?lang=es|en|uk` or the browser language).
