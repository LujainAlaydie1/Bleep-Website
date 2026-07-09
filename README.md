# Bleep website

Four self-contained, bilingual (Arabic/English) static pages. Arabic is the
default language, with an EN/عربي toggle in the nav.

- `index.html` — landing page
- `terms.html` — Terms of Use
- `privacy.html` — Privacy Policy
- `support.html` — Support / FAQ

## Deploy to Vercel via GitHub

1. `git init && git add . && git commit -m "Bleep website"`, push to a new GitHub repo.
2. In Vercel: **Add New Project** → import that repo. No build command needed.
3. Add a subdomain (e.g. `bleep.lsquared.sa`) under **Settings → Domains**.
4. `vercel.json` enables clean URLs.

## Content notes

The Terms of Use page is adapted directly from the app's own in-app
`TermsView.swift` (same 10 sections, same zero-tolerance content policy,
same 24-hour report review promise) — translated into Arabic, not rewritten,
so the website and the app stay consistent. The Privacy Policy is grounded
in what the app actually collects (Firebase Auth/Firestore/Storage,
microphone + photo library access) and explains the anonymous-posting
feature honestly: anonymous posts hide your identity from other users, but
your account stays linked to it internally for moderation purposes.
