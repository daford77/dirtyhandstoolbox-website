# dirtyhandstoolbox-website

Marketing site and published web build for Dirty Hands Toolbox.

## Structure

- `index.html` - main landing page / chooser page for the public domain
- `app/` - published Flutter web build served from `/app/`
- `landing/` - marketing images used by the landing page
- `downloads/` - direct download assets such as the Android APK
- `privacy.html` - privacy policy page

## Update flow

The Flutter app source lives separately in:

- `C:\Source\DirttyHandsToolbox`

The web app inside `app/` is generated from that Flutter repo using:

- `C:\Source\DirttyHandsToolbox\scripts\build_publish_web.ps1`

That script builds Flutter web output directly into this repo's `app/` folder using the `/app/` base href.

## Notes

- Keep marketing-page edits in this repository.
- Keep Flutter app feature work in the main Flutter repository.
- If landing-page screenshots or branding change, update files in `landing/` and adjust `index.html` as needed.
