# AetherFlow

Adobe After Effects extension for local AI-assisted creative workflows.

[Download Latest Release](https://github.com/danrac/AetherFlow_Releases/releases/latest)
[View Release Repository](https://github.com/danrac/AetherFlow_Releases)
[Sponsor Development](https://github.com/sponsors/danrac)

![AetherFlow main CEP panel](assets/screenshots/aetherflow-cep-main.png)

## Overview

AetherFlow runs inside After Effects as a CEP/ZXP panel. It provides artist-facing tools for prompt-assisted image work, footage enhancement, OCR/template graphics, node-based workflow building, runtime management, and optional native AE plugin add-ons.

Large runtime dependencies and model weights are installed after the ZXP through Runtime Manager instead of being bundled into the extension installer.

## Screenshots

### Configuration

![AetherFlow configuration panel](assets/screenshots/aetherflow-cep-configuration.png)

### Runtime Manager

![AetherFlow runtime manager](assets/screenshots/aetherflow-runtime-manager.png)

### Node Workflow Workspace

![AetherFlow node workflow workspace](assets/screenshots/node-workspace.png)

## Workflow Areas

- Prompt-assisted still image generation and image editing.
- Local enhancement, upscaling, cleanup, and slow-motion workflows.
- TikTok Graphic and Template Text Graphics workflows for rebuilding editable AE precomps from reference graphics.
- Subtitle generation and editable text workflows.
- Node-based source, color, cache, viewer, composite, runtime model, and export routing.
- Native AE plugin add-ons for Depth V2, Enhance, Normal Maps, and related plugin-owned functionality.
- Runtime Manager installs, repairs, mutes, and verifies local components.

## Install

1. Download `AetherFlow_CEP.zxp` from the latest release.
2. Install the ZXP with your preferred ZXP installer.
3. Restart After Effects.
4. Open `Window > Extensions > AetherFlow`.
5. Open Configuration and run `Install / Repair Runtime`.
6. Use Runtime Manager to install the workflows, models, and plugin packages needed on that machine.

## Online And Offline Runtime Mode

| Mode | Behavior |
| --- | --- |
| Online | Uses the configured runtime cache first, then downloads missing approved components when needed. |
| Offline | Installs only from the configured runtime cache and does not use public internet fallback. |

For restricted studio machines, populate a shared runtime cache from a connected machine, then point offline workstations to that cache.

## Firewall Allowlist

```text
https://danrac.github.io/AetherFlow_Docs/
https://github.com/danrac/AetherFlow_Releases/releases/
https://github.com/danrac/AetherFlow_Releases/releases/download/
https://objects.githubusercontent.com/
```

Optional support link:

```text
https://github.com/sponsors/danrac
```

## Distribution

The public distribution model is split into:

- Private source/development: `danrac/AetherFlow_CEP`
- Public docs/site: `danrac/AetherFlow_Docs`
- Public downloads/releases: `danrac/AetherFlow_Releases`

Source code, build internals, and proprietary implementation details are not distributed publicly.
