# CLAUDE — Portal App

This is the **PRO PORTAL** — a single-page Supabase Auth + Profile + Properties portal.

## What this app is
- Single HTML file (`index.html`) — no build step, no framework
- Dark/light theme toggle
- Features: Sign Up/In, Profile, Role management (USER/ADMIN/SUPER_ADMIN), Properties listing with favorites

## Supabase project
- Project ref: `mzmswzocehujfgiexgpl` (**separate** from Zenkai's main DB)
- URL: `https://mzmswzocehujfgiexgpl.supabase.co`
- Tables: `profiles`, `properties`, `favorites`
- RPC: `ensure_profile()` — auto-creates profile on first login

## Roles
| Role | Can do |
|------|--------|
| `USER` | default on signup, view properties |
| `ADMIN` | add properties |
| `SUPER_ADMIN` | promote other users |

## Project isolation
This repo is **completely separate** from `zenkai` and the affiliate project.
Different Supabase project, different purpose. Do NOT mix data or tokens between them.

## To edit
Open `index.html` directly in a browser. No build step needed.
