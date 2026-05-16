<p align="center">
  <img src="resources/logo.png" alt="Kuba" width="128" />
</p>

# Kuba

**Kuba** is a desktop Kubernetes manager for Windows and Linux. Connect to your clusters via kubeconfig, browse workloads, view logs, exec into pods, edit YAML, and more.

> Not affiliated with the Kubernetes project or the CNCF.

## Download

Install the latest release for your platform:

| Platform | Installer | Portable |
|----------|-----------|----------|
| **Windows** | [Kuba-0.1.1-Setup.exe](https://github.com/inno-byte/kuba/releases/download/v0.1.1/Kuba-0.1.1-Setup.exe) | [Kuba-0.1.1-Portable.exe](https://github.com/inno-byte/kuba/releases/download/v0.1.1/Kuba-0.1.1-Portable.exe) |
| **Linux** | [Kuba-0.1.1-Setup.deb](https://github.com/inno-byte/kuba/releases/download/v0.1.1/Kuba-0.1.1-Setup.deb) | [Kuba-0.1.1-Portable.AppImage](https://github.com/inno-byte/kuba/releases/download/v0.1.1/Kuba-0.1.1-Portable.AppImage) |

See all assets on the [Releases](https://github.com/inno-byte/kuba/releases) page.

## Requirements

- A valid **kubeconfig** (`~/.kube/config` or `KUBECONFIG`)
- Network access to your cluster API (HTTPS/TLS, same as `kubectl`)
- **Windows** 10/11 (x64) or **Linux** x64

## Installation

### Windows (installer)

1. Download `Kuba-0.1.1-Setup.exe`
2. Run the installer and follow the wizard
3. Launch **Kuba** from the Start menu or desktop shortcut

### Windows (portable)

1. Download `Kuba-0.1.1-Portable.exe`
2. Run it directly — no installation required

### Linux (Debian/Ubuntu)

```bash
sudo dpkg -i Kuba-0.1.1-Setup.deb
kuba
```

### Linux (portable)

```bash
chmod +x Kuba-0.1.1-Portable.AppImage
./Kuba-0.1.1-Portable.AppImage
```

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
