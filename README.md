# oauthpage

CLI for [OAuthPage](https://oauth.page) — protect any website with OAuth in one command.

## Install

```bash
npm install -g oauthpage
```

Or use directly with `npx`:

```bash
npx oauthpage deploy ./dist --site my-app
```

## Quick Start

```bash
# 1. Log in to your OAuthPage account
oauthpage login

# 2. Create a site
oauthpage add "My App"

# 3. Deploy files
oauthpage deploy ./dist --site my-app

# That's it — your site is live and protected!
```

## Commands

| Command | Description |
|---------|-------------|
| `oauthpage login` | Authenticate with your OAuthPage account |
| `oauthpage logout` | Clear stored credentials |
| `oauthpage add <name>` | Create a new site |
| `oauthpage deploy <dir\|file> --site <slug>` | Deploy files or markdown to a site |
| `oauthpage sites` | List all your sites |
| `oauthpage status [slug]` | Show site details or account usage |
| `oauthpage access <slug>` | List approved users for a site |
| `oauthpage approve <slug> <email>` | Approve access for a user |
| `oauthpage deny <slug> <email>` | Deny a pending access request |
| `oauthpage revoke <slug> <email>` | Revoke a user's access |
| `oauthpage remove <slug>` | Delete a site |
| `oauthpage link create <slug>` | Create a one-time access link |
| `oauthpage link list <slug>` | List active one-time links |
| `oauthpage link revoke <id>` | Revoke a one-time link |

## Deploy Markdown

Turn any `.md` file or folder into a beautifully rendered, private documentation site:

```bash
# Single file
oauthpage deploy README.md --site docs

# Folder of markdown files
oauthpage deploy ./docs --site docs
```

## Aliases

The CLI is also available as `opage` for convenience:

```bash
opage deploy ./dist --site my-app
```

## License

MIT — [Unplug.io](https://unplug.io)
