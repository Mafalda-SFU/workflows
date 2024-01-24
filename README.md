# Mafalda SFU workflows

Generic Github Actions workflows for testing and update dependencies

## Usage

These workflows are meant to be used as shared workflows.

- `main.yml`: run tests when merging to `main` branch, and generate code
  coverage badge
- `pull_request.yml`: run tests when opening a pull request
- `schedule.yml`: check for updates to specified dependency, and if so, update
  them, run tests and commit changes. If everything went well, it publish a new
  release in both npmjs and GPR registries, generate docs, and upload a packed
  module to the Github release assets.
