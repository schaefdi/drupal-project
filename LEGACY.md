# Legacy status

This repository is preserved as a historical Drupal 8 Composer template. Its manifest targets Drupal Core `^8.6.0` and the surrounding 2018-era Composer ecosystem.

It must **not** be treated as a supported or production-secure Drupal baseline:

- Drupal 8 is end-of-life.
- There is no committed `composer.lock`, so the repository does not define a reproducible dependency graph.
- Installing the historical manifest on a current PHP/Composer runtime may fail because old plugins and packages use obsolete APIs.
- A modern replacement should start from a supported Drupal release and migrate project-specific configuration/content deliberately rather than attempting an in-place dependency jump.

CI for this branch therefore validates only the preserved source contract: Composer metadata syntax, PHP syntax, and the explicit legacy-version declaration. It does not claim that the historical application is deployable or secure.
