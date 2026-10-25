# Web Files for arrudabaga.com

[arrudabaga.com](https://arrudabaga.com)

## Hosting

- Host: Hostinger (hPanel; LiteSpeed server, `.htaccess`-compatible)
- Domain registrar: Porkbun; DNS: Hostinger (`dns-parking.com`)
- Deploy: push to `main` → GitHub Action FTP-syncs `http/` to `/domains/arrudabaga.com/public_html/`

Directories deployed by other repos:

| Path | Repo | Notes |
|---|---|---|
| `people-collector/` | `people-collector-poc` | Alya game |
| `twin-blog/` | `twin-blog` (private) | Password-protected via hPanel; never ship an `.htaccess` there |

## Error pages

`http/errors/<code>.html`, wired up via `ErrorDocument` in `http/.htaccess`. Subdirectories inherit them, including `twin-blog/`.
