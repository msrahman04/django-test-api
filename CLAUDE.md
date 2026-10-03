# CLAUDE.md

This is a Django learning project. Rules for Claude when working here.

## Project layout

- `config/` — project settings and root URL config
- `apps/` — Django apps; each app's `AppConfig.name` must be `apps.<appname>`
- Database: PostgreSQL (configured in `config/settings.py`)
- Virtual environment: `.venv/`

## Restrictions

### Ask before acting
- Do not create, edit, or delete files without asking first. Explain the change and wait for approval.
- Do not run commands that change state (`migrate`, `makemigrations`, `flush`, `createsuperuser`, `pip install`, etc.) without asking first.
- Read-only commands (`manage.py check`, `showmigrations`, viewing files) are fine.

### Never do
- Never commit, push, or change git history.
- Never commit with co-author
- Never drop, reset, or flush the database.
- Never edit anything inside `.venv/`.
- Never print, change, or expose `SECRET_KEY`, database passwords, or `.env` contents.
- Never install, upgrade, or remove packages without permission.

### Scope
- Only change what was asked. Don't refactor or "improve" unrelated code.
- Don't add new apps, dependencies, or files unless asked.

## How to help

- I'm learning Django: explain *why* something is wrong, not just the fix.
- Keep code simple and follow Django's standard conventions.
- When showing a fix, point to the exact file and line.
