# Actions-Sandbox

Run GitHub Actions runners as a sandbox to test and fix your workflow.

## Introduction

These workflows allow you to run GitHub Actions runners as a sandbox to test and fix your workflow.

By accessing the sandbox through Tailscale, you can:

-   Check what's actually inside the runner image.
-   Watch what's going on inside the runner.
-   View file changes manually.
-   Run commands dynamically.
-   Interact with Windows GUI manually.

## Notice

GitHub hosted runners are public resources. They should not be used for any non-development use.

You need to set `TS_OAUTH_CLIENT_ID` and `TS_OAUTH_SECRET` secrets in your repository. The OAuth client should has write access to `auth_keys` (Read or modify auth keys.) scope for `tag:ci`.
