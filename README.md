# 31374
Reproduction for [Renovate Discussion 31374](https://github.com/renovatebot/renovate/discussions/31374).

## Current behavior
Renoate creates PR's for the single deployment and apiVersion's.
Music Assistant PR: [ghcr.io/music-assistant/server	patch	2.2.3 -> 2.2.4](https://github.com/morotsgurka/renovate-helm-reproduction/pull/3)

## Expected behavior
Renovate creates PR's for the helm releases.
Example:
```authentik "2024.6.4" -> "2024.8.1"```

## Link to the Renovate issue or Discussion
Put your link to the Renovate issue or [Discussion here](https://github.com/renovatebot/renovate/discussions/31374).

## Includes helm releases:
- authentik
    - version: "2024.6.4" but version: "2024.8.1" is available
- cert-manager
    - version: v1.15.0 but version: v1.15.3 is available
- longhorn
    - version: "v1.6.1" but version: "v1.7.1" is available
- traefik
    - version: "v28.0.0" but version: "v31.0.0" is available
        - also values pinned image version: tag: "v3.0.1" but version "v3.1.2" is available

## Includes a single Deployment:
- music assistant server
    - version: 2.2.3 but version: 2.2.4 is available