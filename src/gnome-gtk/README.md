# Development Container for GNOME applications

> [!CAUTION]
> This container requires a functioning wayland socket on your system. There are some hardcoded values that SHOULD work on most systems. 
> The container was ONLY tested with AMD GPUs for hardware acceleration. Other GPUs (particularly NVIDIA ones) may not work. PRs are very much welcomed

Develop GNOME apps with GTK4 and Libadwaita on Linux with C. The environment is identical to the flatpak SDK.

## Options

| Options Id | Description | Type | Default Value |
|-----|-----|-----|-----|
| sdkVersion | GNOME SDK version. This matches with the flatpak SDK | string | 49 |

