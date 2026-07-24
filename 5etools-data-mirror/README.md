# 5etools-data

Personal data mirror for the Rules Lawyer Discord bot. A GitHub Actions
workflow syncs the `data/` directory from the upstream 5etools source repo
once a day (or on demand via the Actions tab -> Sync 5etools data -> Run
workflow).

If the upstream mirror org ever rotates (5etools-mirror-3 -> -4 etc.),
update the clone URL in `.github/workflows/sync.yml`. Nothing downstream
needs to change - that's the point of this repo.

`.last-sync` records the upstream commit and date of the most recent sync.
