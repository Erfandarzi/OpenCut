<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="brand/marks/symbol-light.svg">
    <source media="(prefers-color-scheme: light)" srcset="brand/marks/symbol-dark.svg">
    <img alt="OpenCut symbol" src="brand/marks/symbol-dark.svg" width="96">
  </picture>
</p>

<h1 align="center">OpenCut</h1>

<p align="center">
  <strong>Cut freely. Build openly.</strong><br>
  A free and open-source video editor, available today in Classic and being rebuilt in public.
</p>

<p align="center">
  <a href="https://opencut.app"><strong>EDIT TODAY ↗</strong></a>
  &nbsp;&nbsp;&nbsp;
  <a href="#build-next"><strong>BUILD NEXT ↓</strong></a>
</p>

<picture>
  <source media="(max-width: 600px)" srcset="brand/readme-hero-mobile.webp">
  <img alt="Abstract collage of video frames and timeline tracks opening through a diagonal cut" src="brand/readme-hero.webp" width="100%">
</picture>

## Edit today

[OpenCut Classic](https://github.com/OpenCut-app/opencut-classic) is the working editor. Open it in your browser at **[opencut.app →](https://opencut.app)**.

The original Classic code remains available in its archived repository.

## Build next

This branch is the new foundation:

- **Web** — a React workspace with a placeholder home page and `/editor` route.
- **API** — a Cloudflare Worker with status, health, and echo endpoints.
- **Desktop** — a GPUI shell with browser, preview, inspector, and timeline panels.

The Editor API, plugin architecture, shared Rust core, mobile app, MCP server, headless rendering, and in-editor scripting are the direction—not shipped editor features.

### Quick start

Install [proto](https://moonrepo.dev/proto), then start the web workspace with the repository's pinned toolchain:

<details>
<summary><strong>Install proto</strong></summary>

**Linux, macOS, or WSL**

```sh
bash <(curl -fsSL https://moonrepo.dev/install/proto.sh)
```

**Windows PowerShell**

```powershell
irm https://moonrepo.dev/install/proto.ps1 | iex
```

If proto's shims are blocked, run `Set-ExecutionPolicy -Scope CurrentUser RemoteSigned`.

</details>

```sh
proto use
moon run web:dev
```

Open `http://localhost:5173`. The `/editor` route currently reads “Coming soon.”

<details>
<summary><strong>API and desktop workspaces</strong></summary>

```sh
moon run api:dev       # http://localhost:8787
moon run desktop:dev   # early native editor shell
```

Desktop platform requirements are documented in [`apps/desktop/README.md`](apps/desktop/README.md).

</details>

## Stay close

[Discord](https://discord.gg/zmR9N35cjK) · [Issues](https://github.com/OpenCut-app/OpenCut/issues) · [Security](.github/SECURITY.md) · [X](https://x.com/opencutapp)

The architecture is still being designed, so outside contributions are not open yet. OpenCut is supported by [fal.ai](https://fal.ai?utm_source=github-opencut&utm_campaign=oss); sponsorship inquiries can be sent to [sponsor@opencut.app](mailto:sponsor@opencut.app).

OpenCut is available under the [MIT License](LICENSE).

See [`apps/desktop/README.md`](apps/desktop/README.md) for desktop build notes.

<!-- sync2 -->
<!-- readme: format -->
