# Grameen Bazar v13 — real cloud marketplace

This build uses Supabase for real multi-device accounts, seller listings, orders and stock. It falls back to the local demo if the config is left blank.

## Setup
1. Create a Supabase project.
2. In SQL Editor, run `supabase_schema.sql`.
3. Enable Email authentication. For a school demo, disable email confirmation so login is immediate.
4. Put your Project URL and anon/public key in `supabase-config.js`.
5. Upload all files to GitHub Pages.
6. Register `admin@grameenbazar.in` with your chosen password. That account receives admin/God Mode automatically.

The anon key is meant for browser apps; the security comes from Supabase RLS. Never put a Supabase service-role key in this website.


## Supabase connection - v14

1. Open `supabase-config.js`.
2. Keep the Project URL already filled in.
3. Replace `PASTE_YOUR_PUBLISHABLE_KEY_HERE` with your Supabase Publishable key.
4. Do not use a secret/service_role key.
5. Upload the files to GitHub Pages.

The database schema should be run in Supabase SQL Editor first. The admin role is stored in `public.profiles.role`.
