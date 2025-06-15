# Auto Commit Log

This project automatically creates commits every 30 minutes to log the repository's activity time.

## How it works

- Uses GitHub Actions to run automatically every 30 minutes
- Each run adds a new line to `log.txt` with a timestamp
- Automatically commits and pushes changes to the repository

## Configuration

The workflow is configured in `.github/workflows/auto-commit.yml` with the following features:

- Runs automatically every 30 minutes
- Can be triggered manually through GitHub Actions
- Uses GitHub Actions bot to create commits
- Only commits the `log.txt` file

## Usage

1. Fork this repository to your GitHub account
2. Ensure the repository has push access (Settings > Actions > General > Workflow permissions)
3. The workflow will automatically run and create commits every 30 minutes

## Notes

- `log.txt` will be created automatically on the first workflow run
- Each commit will contain a timestamp of when it was created
- You can track the repository's activity history through `log.txt`