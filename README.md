<p align="center">
  <img src="resources/logo.png" alt="Kuba" width="128" />
</p>

# Kuba

**Kuba** is a desktop Kubernetes manager for Windows, Linux and macOS. Connect to your clusters via kubeconfig, browse workloads, view logs, exec into pods, edit YAML, and more.

> Not affiliated with the Kubernetes project or the CNCF.

## Download

Install the latest release for your platform:

| Platform | Installer | Portable |
|----------|-----------|----------|
| **Windows** | [Kuba-0.1.2-Setup.exe](https://github.com/inno-byte/kuba/releases/download/v0.1.2/Kuba-0.1.2-Setup.exe) | [Kuba-0.1.2-Portable.exe](https://github.com/inno-byte/kuba/releases/download/v0.1.2/Kuba-0.1.2-Portable.exe) |
| **Linux** | [Kuba-0.1.2-Setup.deb](https://github.com/inno-byte/kuba/releases/download/v0.1.2/Kuba-0.1.2-Setup.deb) | [Kuba-0.1.2-Portable.AppImage](https://github.com/inno-byte/kuba/releases/download/v0.1.2/Kuba-0.1.2-Portable.AppImage) |
| **macOS** | [Kuba-0.1.2-Setup-arm64.dmg](https://github.com/inno-byte/kuba/releases/download/v0.1.2/Kuba-0.1.2-Setup-arm64.dmg) (Apple Silicon) · [x64](https://github.com/inno-byte/kuba/releases/download/v0.1.2/Kuba-0.1.2-Setup-x64.dmg) (Intel) | [arm64](https://github.com/inno-byte/kuba/releases/download/v0.1.2/Kuba-0.1.2-Portable-arm64.zip) · [x64](https://github.com/inno-byte/kuba/releases/download/v0.1.2/Kuba-0.1.2-Portable-x64.zip) |

See all assets on the [Releases](https://github.com/inno-byte/kuba/releases) page.

## Requirements

- A valid **kubeconfig** (`~/.kube/config` or `KUBECONFIG`)
- Network access to your cluster API (HTTPS/TLS, same as `kubectl`)
- **Windows** 10/11 (x64), **Linux** x64 or **macOS** 11+ (Apple Silicon or Intel)

## Installation

### Windows (installer)

1. Download `Kuba-0.1.2-Setup.exe`
2. Run the installer and follow the wizard
3. Launch **Kuba** from the Start menu or desktop shortcut

### Windows (portable)

1. Download `Kuba-0.1.2-Portable.exe`
2. Run it directly — no installation required

### Linux (Debian/Ubuntu)

```bash
sudo dpkg -i Kuba-0.1.2-Setup.deb
kuba
```

### Linux (portable)

```bash
chmod +x Kuba-0.1.2-Portable.AppImage
./Kuba-0.1.2-Portable.AppImage
```

### macOS (installer)

1. Download `Kuba-0.1.2-Setup-arm64.dmg` (Apple Silicon) or `Kuba-0.1.2-Setup-x64.dmg` (Intel)
2. Open the `.dmg` and drag **Kuba** to **Applications**
3. Launch **Kuba** from Applications (first launch: right-click → Open if Gatekeeper blocks unsigned builds)

### macOS (portable)

1. Download `Kuba-0.1.2-Portable-arm64.zip` or `Kuba-0.1.2-Portable-x64.zip`
2. Unzip and double-click `Kuba.app`

## Kubeconfig

Kuba uses your standard Kubernetes configuration:

- Default: `~/.kube/config`
- Or set `KUBECONFIG` to point to one or more files
- You can add extra kubeconfig files from the app header

If `kubectl` works with your cluster, Kuba should work too.

## License

This project is licensed under the [MIT License](LICENSE).

## Support

Report issues on [GitHub Issues](https://github.com/inno-byte/kuba/issues).
