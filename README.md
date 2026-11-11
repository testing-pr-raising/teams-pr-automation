# teams-pr-automation

Central reusable workflow that posts a Microsoft Teams card when a PR is raised.

## Add a project

1. Copy `.github/workflows/pr-notify.yml` from any project repo into the new repo's `develop` branch.
2. Change `title_prefix` (and `default_mentions` if needed).

## Org settings (one time)

- Secret `TEAMS_WEBHOOK_URL`: Teams Workflow webhook URL.
- Variable `TEAMS_USER_MAP`: `{"<github-login>":{"name":"<Teams name>","email":"<Teams email>"}}`.
