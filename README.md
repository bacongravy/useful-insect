# useful-insect

This project demonstrates how to use [GitHub Actions](https://github.com/features/actions) and [`glitcheroo`](https://www.npmjs.com/package/glitcheroo) together to continuously deploy a project from GitHub to Glitch.

## How does it work

The [`deploy`](https://github.com/bacongravy/useful-insect/blob/master/.github/workflows/deploy.yml) workflow is triggered on every push to the `master` branch. The workflow first creates a new GitHub deployment, then deploys the project with `glitcheroo`, and finally updates the GitHub deployment status with the result.

The GitHub deployments created by the workflow can be found [here](https://github.com/bacongravy/useful-insect/deployments).

The logs from the `deploy` workflow can be found [here](https://github.com/bacongravy/useful-insect/actions?query=workflow%3Adeploy).
