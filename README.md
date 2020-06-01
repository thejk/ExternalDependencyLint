# ExternalDependencyLint

Sample project for a bug where running lint for a flavor references artifacts
for all flavors.

To reproduce:
1) Clone this repo
2) Run :app:lintBetaRelease task

The task fails with error about final.jar not existing, as we're linting
and building the beta flavor this looks like an error in the lint task.
