# yarr

**yarr** (yet another rss reader) is a web-based feed aggregator which can be used both
as a desktop application and a personal self-hosted server.

This is a fork of [the original](https://github.com/nkanaev/yarr) with some enhancements:

- Modified shortcuts
  - `d` `u` scroll content forward / backward
  - `g` scroll to top feed
  - `G` scroll to bottom feed
  - `esc` hide current dialog
  - `?` show shortcuts
- Added navigation button in article view, to support a better navigation on mobile devices.
  - <img width="573" alt="Screenshot 2024-04-17 at 16 31 24" src="https://github.com/waynezhang/yarr/assets/480052/fb61add8-1f08-4f7d-9a24-5b512a040b22">
- Automatically docker image build.
  - [https://github.com/waynezhang/yarr/pkgs/container/yarr](https://github.com/waynezhang/yarr/pkgs/container/yarr)

---

The app is a single binary with an embedded database (SQLite).

![screenshot](etc/promo.png)

## usage

The latest prebuilt binaries for Linux/MacOS/Windows AMD64 are available
[here](https://github.com/nkanaev/yarr/releases/latest). Installation instructions:

* MacOS

  Download `yarr-*-macos64.zip`, unzip it, place `yarr.app` in `/Applications` folder, [open the app][macos-open], click the anchor menu bar icon, select "Open".

* Windows

  Download `yarr-*-windows64.zip`, unzip it, open `yarr.exe`, click the anchor system tray icon, select "Open".

* Linux

  Download `yarr-*-linux64.zip`, unzip it, place `yarr` in `$HOME/.local/bin`
and run [the script](etc/install-linux.sh).

* Docker

  `docker pull ghcr.io/waynezhang/yarr:master`

[macos-open]: https://support.apple.com/en-gb/guide/mac-help/mh40616/mac

For self-hosting, see `yarr -h` for auth, tls & server configuration flags.

See more:

* [Building from source code](doc/build.md)
* [Fever API support](doc/fever.md)

## credits

[Feather](http://feathericons.com/) for icons.
