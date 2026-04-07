# Media Relay Client for Linux

**Media Relay Client** is the display-side for **Media Relay** — a multi-platform application that lets you upload and control media playback on multiple display devices. It is intended for use in kiosks, projectors, televisions, and interactive smart displays. 

This Linux client runs as a display receiver, waiting for a controller device to connect and push media content to it over a local network, if your network does not allow UDP broadcasts you'll need to manually add the IP Address.

Unlike casting, which mirrors/streams your screen and requires a constant connection, Media Relay uploads media files directly to the display device and will allow you to persist the media between system reboots so long as you set the app to startup with the device.

![Raspbian](https://github.com/Wandtket/Media-Relay-Releases/blob/main/Images/Raspbian.png)

## Installation

### From a `.deb` package (Debian / Ubuntu / Raspberry Pi OS)

Download the `.deb` file for your architecture and install it with `apt`:

```bash
sudo apt install ./mediarelay-<arch>.deb
```

The package is self-contained and will automatically install the required dependencies (`vlc`, `libvlc5`, `gtk-sharp2`).

## Uninstall

```bash
sudo apt-get remove mediarelay
```

### Supported Architectures

| Architecture | Runtime Identifier |
|--------------|--------------------|
| x86-64       | `linux-x64`        |
| ARM 64-bit   | `linux-arm64`      |
| ARM 32-bit   | `linux-arm`      |

## Usage

After installation, launch the app from your application menu or from the terminal:

```bash
MediaRelay.Client.Linux
```

On first launch you will be guided through a short setup to name your display and optionally set a password. Once configured, the display will appear on the local network and can be controlled from any Media Relay controller app.

### Supported Media Formats

| Type  | Extensions                                  |
|-------|---------------------------------------------|
| Video | `.mp4` `.mov` `.avi` `.mkv` `.webm` `.m4v`  |
| Image | `.jpg` `.jpeg` `.png` `.gif` `.bmp` `.webp` |
| Audio | `.mp3` `.wav` `.aac` `.flac` `.ogg` `.m4a`  |
| Web   | `.weblink`                                  |

## Other Platforms

Media Relay is also available on:

- **Android** — [Google Play](https://play.google.com/store/apps/details?id=com.wandtke.mediarelay)
- **Windows** — [Microsoft Store](https://www.microsoft.com/store/apps/9P2ZLZ5K1G8S)

### iOS / macOS

An iOS or macOS version is not publicly available at this time. Organizations interested in a build for Apple platforms should contact the developer directly to discuss licensing and deployment options.

## Contact

- **Developer:** Tyler J. Wandtke
- **Email:** [wandtket@gmail.com](mailto:wandtket@gmail.com)
- **LinkedIn:** [Tyler J. Wandtke](https://www.linkedin.com/in/tyler-wandtke-001614128/)

## License

This software is proprietary. All rights reserved.
