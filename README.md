# Wanderer's Atlas — Mark 5 Cleanup 2A Supabase Configured

This package has Supabase 7-character online share codes enabled in `atlas-config.js`.

Upload these files to the root of the GitHub repository:

- index.html
- styles.css
- app.js
- atlas-config.js
- skyrim-map.jpg
- .nojekyll
- README.md
- supabase-schema.sql

Supabase project configured:
- URL: https://dwqwwmrhayewjkntjrmc.supabase.co
- Key type: publishable key
- Table: atlas_shares
- Expiration: 30 days

Still required:
1. Open Supabase.
2. Go to SQL Editor.
3. Open `supabase-schema.sql` from this package.
4. Paste the full contents into a new SQL query.
5. Click Run.
6. Upload this package to GitHub.

After those steps:
- `Copy 7-Char Code` should create a short online code.
- Receive should accept that 7-character code.
- `Copy Offline Code` still works as a fallback.

Important:
- Do not use a secret key or service_role key in `atlas-config.js`.
- The publishable key is meant for browser use when Row Level Security and policies are configured.
- The SQL file creates the table, constraints, grants, and Row Level Security policies.

Retained:
- Mark 5 stable Leaflet behavior.
- Map/zoom/pan/drawing behavior unchanged.
- Storage keys unchanged.
- Public-sharing safeguards.
- Duplicate detection.
- Strong Replace confirmation.
- No file uploads.
- No Guild system.
- No visible Share Code textarea.
- No Export JSON Backup.
- No Import JSON / Choose File.

Full map size remains 8192 × 6144.
