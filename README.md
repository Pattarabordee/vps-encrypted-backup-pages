# VPS Encrypted Backup — OAuth informational website

Public informational pages for the private **VPS Encrypted Backup** Google Drive OAuth application.

- `index.html`: homepage explaining the encrypted PostgreSQL backup workflow
- `privacy.html`: privacy policy covering Google Drive scope, OAuth credentials, storage, and retention
- `terms.html`: terms of use for the informational website

## Publishing with GitHub Pages

Go to **Settings → Pages → Build and deployment**, choose **Deploy from a branch**, then select `main` and `/(root)`. Save the setting.

Once GitHub confirms deployment, check:
- Home: `https://pattarabordee.github.io/vps-encrypted-backup-pages/`
- Privacy: `https://pattarabordee.github.io/vps-encrypted-backup-pages/privacy.html`
- Terms: `https://pattarabordee.github.io/vps-encrypted-backup-pages/terms.html`

These are expected paths; verify that the live pages respond successfully before entering them into Google Auth Platform. Google may require domain ownership verification before OAuth production publishing. GitHub Pages availability does not itself establish Google acceptance.

## Security

**Never commit:** database dumps, `.gpg` archives, rclone config, Google OAuth IDs/secrets/tokens, passphrases, or other production credentials. This repository contains only public HTML and documentation; backups remain in encrypted Google Drive storage.

This website does not trigger backup jobs, host database data, or expose the VPS to the public.
