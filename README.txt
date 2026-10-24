TEACHER DASHBOARD STARTER
=========================

This is a starter frontend, not the completed production system.

WHAT WORKS AFTER CONFIGURATION
- Responsive sign-in, sign-up, sign-out, forgot-password and password-update screens using Supabase Auth.
- Starter dashboard screens for quiz drafts, student list drafts, timetable entries, resources, and profile/menu notes.
- Draft records currently save to this browser's localStorage only.

NOT YET IMPLEMENTED
- Cloud database syncing / secure student records
- AI quiz generation (requires a server-side function and an AI provider key)
- Shareable student test links and automatic grading/results
- Editable navigation menu persisted in the database

SETUP
1. Open index.html in a code editor.
2. Replace SUPABASE_URL with your Supabase Project URL.
3. Replace SUPABASE_ANON_KEY with your Supabase publishable/anon key.
   Never use a service_role/secret key in browser code.
4. In Supabase Authentication > URL Configuration, set Site URL to the deployed website URL once it exists.
   Add the deployed URL to Redirect URLs. During local development, add http://localhost:3000 if using a local server.
5. For password recovery, ensure the deployed URL is in Redirect URLs and configure email confirmation / SMTP settings as needed.
6. Host this static site with GitHub Pages or another static host. A GitHub repository alone does not automatically publish a website.

IMPORTANT
- Do not store real student personal information in this prototype.
- The browser-local drafts are not synced across devices and may be lost if browser storage is cleared.
- Before production, create database tables and Row Level Security policies in Supabase. Never expose a service_role key.
