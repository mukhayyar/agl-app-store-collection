# AGL App Store Collection

Collection of all component repositories for the **AGL (Automotive Grade Linux) App Store** system — a secure Flatpak application distribution platform for in-vehicle infotainment (IVI) devices.

## Components

| Component | Repository |
|---|---|
| Backend (gRPC Service) | [mukhayyar/backend-agl-app-store](https://github.com/mukhayyar/backend-agl-app-store) |
| Frontend Admin (Moderation) | [mukhayyar/admin-frontend-agl](https://github.com/mukhayyar/admin-frontend-agl) |
| Frontend Client (Flutter IVI) | [mukhayyar/frontend-agl-app-store](https://github.com/mukhayyar/frontend-agl-app-store) |
| Flatpak Server (PENSHub) | [mukhayyar/flatpak-server-agl-app-store](https://github.com/mukhayyar/flatpak-server-agl-app-store) |
| Flat-Manager (Repo Manager) | [mukhayyar/flat-manager](https://github.com/mukhayyar/flat-manager) |
| App Store Meta Application | [mukhayyar/agl-app-store](https://github.com/mukhayyar/agl-app-store) |
| Yocto Layer (meta-agl) | [mukhayyar/agl_meta-agl-app-store](https://github.com/mukhayyar/agl_meta-agl-app-store) |
| Toradex Build Configuration | [mukhayyar/toradex-agl](https://github.com/mukhayyar/toradex-agl) |
| Meta Flatpak Flutter (AGL) | [Freezer9/flutter-agl](https://github.com/Freezer9/flutter-agl) |
| Sample Flatpak App Collection | [mukhayyar/simple-flatpak-app-collections](https://github.com/mukhayyar/simple-flatpak-app-collections) |

## Live Deployments

| Service | URL |
|---|---|
| Store Frontend | [agl-store.cyou](https://agl-store.cyou) |
| Admin / Moderation Panel | [admin.agl-store.cyou](https://admin.agl-store.cyou) |
| REST API | [api.agl-store.cyou](https://api.agl-store.cyou) |
| Backend (gRPC gateway) | [backend.agl-store.cyou](https://backend.agl-store.cyou) |
| PENSHub Flatpak Repo | [repo.agl-store.cyou](https://repo.agl-store.cyou) |
| Flat-Manager Hub | [hub.agl-store.cyou](https://hub.agl-store.cyou) |
| Flatpak Server | [flatpak.agl-store.cyou](https://flatpak.agl-store.cyou) |
| Webhook Receiver | [webhook.agl-store.cyou](https://webhook.agl-store.cyou) |

## Architecture Overview

The system consists of:

- **Backend** — gRPC service handling app submission, scanning, and distribution
- **Security Scanner** — Static analysis pipeline with 18 permission rules (CVSS v3.1-grounded thresholds)
- **Flat-Manager / PENSHub** — OSTree-based Flatpak repository server with GPG signing
- **Admin Frontend** — Web moderation interface for reviewing submitted apps
- **Flutter IVI Client** — In-vehicle touchscreen app store running on AGL
- **Yocto / Toradex layers** — Board Support Package (BSP) integration for Toradex hardware

## License

MIT License. See [LICENSE](LICENSE).
