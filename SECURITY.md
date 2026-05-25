# Security Policy

## Supported Security Posture

This repository contains public WordPress plugin package files and release metadata for RavenHawk YouTube Showcase.

## Secrets Policy

Do not commit:

- YouTube API keys
- OAuth credentials
- API keys
- WordPress credentials
- `.env` files
- SQL/database exports
- `wp-config.php`
- private keys
- debug logs
- production backups

The `.gitignore` file blocks common accidental secret and backup file patterns, but it is not a substitute for reviewing commits before pushing.

## WordPress Update Security

Custom plugin updates should use GitHub Release assets rather than mutable raw files from `main`.

Recommended update chain:

```text
versioned package
→ release ZIP
→ GitHub Release asset
→ update manifest
→ WordPress Admin update
```

## Reporting Issues

Report security issues privately to the repository owner rather than opening public issues containing exploit details or secrets.
