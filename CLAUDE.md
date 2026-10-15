# Claude notes

## CI/CD and testing (no GitHub Actions)

Owner decision (15 Oct 2026): GitHub Actions is not used for CI or for deploys.

- This repository has no GitHub Actions workflows.
- Don't add a workflow, or an automatic trigger to the app build, without asking.
- Testing is done in the local environment. Run the relevant checks locally before committing or pushing. A pull request gets no CI checks, so say in it what you ran and the result.
- Deploys do not go through GitHub Actions and don't wait on GitHub checks.

Checks to run locally (formerly in CI):

- `python manage.py test`
