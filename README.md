# Web UI Website - Stoic Dreams

[Version: 0.11.18](https://github.com/StoicDreams/WebUIWeb)

[View the site - webui.stoicdreams.com](https://webui.stoicdreams.com)

[Stoic Dreams Discord](https://discord.gg/5X4YSDFdHD)

## About

This is the documentation and demo website for Web UI, at [webui.stoicdreams.com](https://webui.stoicdreams.com).

- The Web UI components and styles it documents are served from [cdn.myfi.ws](https://cdn.myfi.ws), from the [MyFiCDN](https://github.com/StoicDreams/MyFiCDN) repo.
- The `webui` Rust crate, the `webui` starter tool, and `webapp_post_build` are in the [WebUI](https://github.com/StoicDreams/WebUI) repo. This site uses the crate from that repo's `main` branch.

## Setup

Follow the [Web CLI Setup](https://webui.stoicdreams.com/tools/cli) guide and the [Web UI Rust Tools Setup](https://webui.stoicdreams.com/tools/rust) guide to install the necessary tools.

## Running the Site

Run the site locally at http://localhost:8114. The script lists any missing tools before building.

```terminal:Run the project from the root directory
./PowerShell/RunLocal.ps1
```

## Testing and Publishing

The site has the same Playwright tests as the other Stoic Dreams websites. They need no build or server.

```terminal:Run the UI tests
npm install
npm test
```

`./PowerShell/Publish.ps1` prepares a commit: it increments the version, minifies the CSS and JavaScript, rebuilds the sitemap, updates the page screenshots, and runs the tests that CI runs.

Pushing to `main` deploys the site.

## Author

**[Erik Gassler](https://www.erikgassler.com) - [Stoic Dreams](https://www.stoicdreams.com)** - Forging solutions for tomorrow's software development.

**Support** - Visit [Stoic Dreams' GitHub Sponsor page](https://github.com/sponsors/StoicDreams) if you would like to provide support to Stoic Dreams.

## License

[MIT](LICENSE)
