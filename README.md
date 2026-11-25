# ReUseLoop — Full-Stack Ready Starter

This project follows the attached ReUseLoop presentation: campus marketplace, registration/login,
profiles, listings, search/filtering, requests, favorites, reports, admin moderation, responsive UI,
Supabase authentication, PostgreSQL and storage.

## 1. Requirements
- Node.js 18+ (Node 20+ recommended)
- A Supabase project
- Internet connection

## 2. Install
```bash
npm install
```

## 3. Configure Supabase
1. Create a project at Supabase.
2. Open SQL Editor.
3. Paste and run `supabase/schema.sql`.
4. Copy `.env.example` to `.env`.
5. Put your Supabase URL and anon/publishable key in `.env`.

Example:
```env
VITE_SUPABASE_URL=https://xxxxx.supabase.co
VITE_SUPABASE_ANON_KEY=xxxxx
```

Do NOT put a Supabase service-role key in this frontend.

## 4. Start
```bash
npm run dev
```
Open the local URL shown by Vite, normally:
http://localhost:5173

## 5. First account
- Register from the website.
- Select `SR Group of Institutions`.
- If email confirmation is enabled in Supabase, confirm your email.
- Sign in.

## 6. Admin
After registering, open Supabase -> Table Editor -> profiles.
Change that user's `role` from `student` to `admin`.
The Admin link then appears after the next sign-in/session refresh.

## Implemented
- Responsive mobile/desktop UI
- Login / registration
- Campus profile
- Browse/search/filter
- Listing creation
- Image upload to Supabase Storage
- Listing detail
- Favorites
- Request submission
- Owner request accept/reject
- Listing close
- Reports
- Admin moderation queue
- PostgreSQL schema
- Row Level Security policies
- Storage policies
- Basic transaction/message tables ready for future chat/transaction completion

## Scope
The presentation says online payments, shipping, escrow and advanced identity verification are not included.
This build keeps the physical handover offline and does not add a payment gateway.
