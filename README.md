# OpenClient_Debug

Independent automation repository for personal, non-commercial Debug builds of OpenClient.

It checks `ntoporcov/openclient` hourly. When the latest upstream commit has been quiet for at least four hours, the workflow checks out that exact upstream commit, builds the existing Debug configuration, packages an unsigned IPA, publishes it as a release here, and updates only the OpenClient entry in `wes1993/altstore-repo/apps.json`.

The upstream source is not stored or mirrored in this repository.

## Required secret

Create the Actions secret `ALTSTORE_REPO_TOKEN` with write access to `wes1993/altstore-repo`.
