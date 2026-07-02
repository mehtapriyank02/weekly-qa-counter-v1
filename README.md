# Weekly QA Counter - Full Clean Repo v500

Use this as a brand-new GitHub repository.

## Files

Upload all files in this folder to the root of the new repo:

- `index.html`
- `styles.css`
- `app.js`
- `config.js`
- `README.md`
- `supabase-final-fail-fix.sql`

## Supabase

Run `supabase-final-fail-fix.sql` in Supabase SQL Editor.

This adds `weekly_assignments.fail_count` and makes the Fail buttons use that column directly.

## Config

Edit `config.js` and paste your anon public key:

```js
window.SUPABASE_URL = "https://gvporifcjbenmhuewzqb.supabase.co";
window.SUPABASE_ANON_KEY = "your anon public key";
```

Do not use the service_role key.

## GitHub Pages

Settings -> Pages:

- Source: Deploy from a branch
- Branch: main
- Folder: / root

Open the site with:

```text
https://mehtapriyank02.github.io/YOUR-NEW-REPO-NAME/?v=500
```

## Expected Fail behavior

The Fail column should show `0 1 2 3+`.

- Click `1`, `2`, or `3+` -> target becomes 7.
- Click `0` -> target resets to 5.
