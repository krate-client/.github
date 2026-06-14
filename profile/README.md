# KRATE

**Self-hosted media and automation for Linux servers.**

KRATE is a Debian-based stack that installs and runs media servers, *arr tools,
download clients, dashboards, and more — from a single command line (`zen`) and a
web interface (HarmonyUI). One package, one workflow: add users, deploy apps per
user, manage services, and keep everything up to date.

## Get started

Install the latest release:

```bash
curl -fsSL https://get.krate.io | bash
```

Or pick a build manually from [**releases**](https://github.com/krate-client/releases/releases).

Then install an app for a Linux user:

```bash
zen software add alice radarr4k
```

Full guides: **[krate.github.io/docs](https://krate.github.io/docs/)**

## Repositories

| Repository | What it is |
|---|---|
| [**releases**](https://github.com/krate-client/releases) | Official `krate` `.deb` packages and release manifests |
| [**console**](https://github.com/krate-client/console) | `zen` CLI and `zenfw` runtime |
| [**setup**](https://github.com/krate-client/setup) | First-install wizard |
| [**web**](https://github.com/krate-client/web) | HarmonyUI — the web dashboard |
| [**official-apps**](https://github.com/krate-client/official-apps) | Official application catalog (public, read-only mirror) |
| [**official-apps-unencrypted**](https://github.com/krate-client/official-apps-unencrypted) | Source for official apps — where changes are reviewed |
| [**community-apps**](https://github.com/krate-client/community-apps) | Community-contributed applications |
| [**plugins-store**](https://github.com/krate-client/plugins-store) | ruTorrent plugins and themes bundled in the package |
| [**docs**](https://github.com/krate-client/docs) | User-facing documentation sources |

## How apps work

Applications are folders with metadata (`meta.yaml`, `manifest.yaml`) and a
lifecycle handler. KRATE ships two catalogs — **official** and **community** —
inside the `krate` package. Before running any handler, `zen` verifies its
SHA-256 checksum and RSA signature against the signed `CATALOG.json` bundled with
your installation.

- Browse what's available: [**official-apps**](https://github.com/krate-client/official-apps)
- Propose a community app: fork [**community-apps**](https://github.com/krate-client/community-apps) and open a pull request
- Report or fix an official app: edit [**official-apps-unencrypted**](https://github.com/krate-client/official-apps-unencrypted)

## Links

- Website & docs: [krate.github.io](https://krate.github.io/)
- Documentation: [krate.github.io/docs](https://krate.github.io/docs/)
- Releases: [github.com/krate-client/releases](https://github.com/krate-client/releases/releases)

---

*This organization hosts the open-source client side of KRATE. Commerce and public
API surfaces live under the separate [krate-shop](https://github.com/krate-shop)
organization.*
