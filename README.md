# Next.js + Supabase Multi-tenant Starter

## Quickstart
1) Clone & install
```bash
npm i
npm run dev
```
2) Create a Supabase project, copy Project URL + anon key into `.env.local`
3) Execute SQL in `supabase/schema.sql` (SQL editor)
4) In Auth -> Providers -> Email, enable Magic Link and set Redirect URL (e.g. http://localhost:3000/(auth)/signin)
5) Create at least one hotel and a membership row for your user.

## Notes
- Dashboard reads from `memberships_view` to show hotels for the current user.
- RLS policies restrict data per hotel (tenant).
