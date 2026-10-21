# Healthy Together

A phone-friendly single-page Healthy Together app with Supabase authentication and database reads/writes.

## What is included
- Mobile-first forest/sage/cream design
- Email/password sign in and account creation
- Daily habit check-ins and XP
- Weekly progress, little wins, rewards, movement guides
- Optional private weight log
- Supabase connection settings entered in the browser and stored on that device

## Important before using real data
This is a starter build. It expects your existing Supabase tables and RLS policies to match the columns listed in `supabase/schema.sql`. It does not yet implement household invitations/shared partner access or reward claims. Verify RLS and test with non-sensitive data first.

## Deploying as a static site
`index.html` is self-contained and can be hosted on Vercel as a static site. If using GitHub, the repository root must contain `index.html` (not just a ZIP). The provided SQL is optional and only adds the `wins` table plus a user-only RLS policy; review before running it.

Never add service-role/secret keys to client-side code or commit them to GitHub.
