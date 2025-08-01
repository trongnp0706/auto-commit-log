# Auto Commit Log

This project automatically creates commits twice daily to log the repository's activity time in Vietnam timezone (UTC+7).

## How it works

- Uses GitHub Actions to run automatically twice a day
- Runs at 7:00 AM and 7:00 PM Vietnam time (UTC+7)
- Each run adds a new entry to `log.txt` with timestamp in Vietnam timezone
- Automatically commits and pushes changes to the repository

## Configuration

The workflow is configured in `.github/workflows/auto-commit.yml` with the following features:

- Runs automatically at 7:00 AM and 7:00 PM Vietnam time
- Can be triggered manually through GitHub Actions
- Uses GitHub Actions bot to create commits
- Only commits the `log.txt` file
- Uses Vietnam timezone (UTC+7) for all timestamps

## Usage

1. Fork this repository to your GitHub account
2. Ensure the repository has push access (Settings > Actions > General > Workflow permissions)
3. The workflow will automatically run twice daily at:
   - 7:00 AM Vietnam time (UTC+7)
   - 7:00 PM Vietnam time (UTC+7)

## Log Format

Each entry in `log.txt` follows this format:
```
[YYYY-MM-DD HH:MM:SS] Auto commit
```

## Notes

- `log.txt` will be created automatically on the first workflow run
- Each commit will contain a timestamp in Vietnam timezone
- You can track the repository's activity history through `log.txt`
- The workflow can be manually triggered at any time using the "Run workflow" button in GitHub Actions
