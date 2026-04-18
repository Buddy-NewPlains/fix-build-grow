# Netlify Setup Notes

## Current status
- Hugo site scaffold is ready.
- Repository is live at `https://github.com/Buddy-NewPlains/fix-build-grow`.
- `netlify.toml` is configured for Netlify builds.

## Manual step still required
Netlify site creation could not be completed from this environment because no Netlify authentication token or logged-in CLI session is available.

## Fastest completion path in Netlify
1. Log into Netlify.
2. Choose **Add new site** -> **Import an existing project**.
3. Connect GitHub and select `Buddy-NewPlains/fix-build-grow`.
4. Use these settings:
   - Build command: `npx hugo --gc --minify`
   - Publish directory: `public`
   - Base directory: leave blank
5. Deploy.
6. Optional: set custom domain and enable Netlify Analytics.

## Environment values already assumed
- `HUGO_VERSION=0.149.2`
- `HUGO_ENV=production`
- `HUGO_ENABLEGITINFO=true`

## Suggested Netlify site name
- `fix-build-grow`

## Post-import checks
- Confirm homepage renders hero art and featured cards
- Verify `/tutorials/`, `/galleries/`, `/estimators/`, and `/comparisons/`
- Turn on deploy previews for pull requests
- Add form capture or newsletter once lead gen is ready
