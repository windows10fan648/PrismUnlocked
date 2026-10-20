<p align="center">
<picture>
  <source media="(prefers-color-scheme: dark)" srcset="/program_info/org.prismlauncher.PrismLauncher.logo-darkmode.svg">
  <source media="(prefers-color-scheme: light)" srcset="/program_info/org.prismlauncher.PrismLauncher.logo.svg">
  <img alt="Prism Unlocked" src="/program_info/org.prismlauncher.PrismLauncher.logo.svg" width="40%">
</picture>
</p>

<p align="center">
  Prism Unlocked is a community fork of Prism Launcher for managing multiple Minecraft installations.<br />
  It keeps Microsoft account sign-in and adds a separate Offline Mode for username-based local play.
</p>

## Features

- Manage multiple Minecraft instances and versions.
- Sign in with a Microsoft account using the normal account workflow.
- Launch with an offline username without signing in to Microsoft.
- Use offline profiles for single-player, LAN, or private servers configured to allow offline players.

Offline Mode does not provide a Minecraft license or authenticated access to online-mode servers. Use the game and servers according to their terms and only share private servers with people you trust.

## Download

Release and development artifacts are available from the repository's [GitHub Actions](https://github.com/windows10fan648/PrismUnlocked/actions) workflows. Builds are provided for Linux, Windows, and macOS when the corresponding workflow jobs complete.

Development builds may contain bugs and are intended for testing. Download the newest artifact from a successful Release or Build workflow.

## Usage

1. Add or import a Minecraft instance.
2. Select the instance.
3. Use **Launch** for the normal Microsoft-account workflow.
4. Use **Offline Mode** to enter a username and launch without a Microsoft account.

Offline accounts can also be created from **Settings → Accounts → Add Offline**.

## Building

Prism Unlocked uses CMake and follows the upstream Prism Launcher build layout. Configure the project with the available CMake preset, then build and test it:

```bash
cmake --preset linux
cmake --build --preset linux --config Release
ctest --preset linux --build-config Release
```

Use the platform-appropriate preset for Windows or macOS. The repository's GitHub Actions workflow contains the complete dependency setup and packaging process.

## Support

For bugs or feature requests, [open an issue](https://github.com/windows10fan648/PrismUnlocked/issues). When reporting a problem, include your operating system, launcher version, instance version, and relevant logs.

## Relationship to Prism Launcher

Prism Unlocked is an independent community fork. It is not endorsed by, affiliated with, or an official release of the Prism Launcher project.

This project retains upstream Prism Launcher code and assets where applicable. Changes made in this fork are maintained in this repository.

## License

Prism Unlocked is distributed under the [GPL-3.0-only license](LICENSE).

The logo and related assets are provided under the CC BY-SA 4.0 license where applicable. See the repository and upstream notices for attribution details.
