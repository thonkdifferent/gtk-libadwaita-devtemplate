# Development Container for GNOME applications

This repository provides a quick and easy OCI based [development container](https://containers.dev) for GTK applications. Unlike the Flatpak SDK this can be seamlessly used from all solutions that support the open dev containers standard.


> [!CAUTION]
> This container requires a functioning wayland socket on your system. There are some hardcoded values that SHOULD work on most systems. 
> The container was ONLY tested with AMD GPUs for hardware acceleration. Other GPUs (particularly NVIDIA ones) may not work. PRs are very much welcomed


# What works
- GUI
- D-Bus
- Wayland
- GPU Acceleration (NO compute)
- compilation with Meson and GCC


# How to use

1. Make sure you have the Dev Containers extension installed in VS Code
2. Open the Command Pallete `Ctrl+Shift+P` and run `Dev Containers: New Dev Container`
3. Type for the template `ghcr.io/thonkdifferent/gtk-libadwaita-devtemplate/gnome-gtk:latest`
4. Trust `@unknown`
5. **Important** Select More options
6. Select your SDK version
7. **Crucial** Type your logged in user id. You can get it by running `$ id`. Your user id is the number after uid. Copy JUST THE NUMBER
8. Get a cup of $drink
9. Test: Open bash inside VSCode and try to run `gnome-text-editor`

# Known issues

- D-Bus only works for one bash session. I am looking into how to have a more persistant d-bus envinronment inside the container
- A11y support is missing (help needed)


# Untested

- NVIDIA/Intel GPU acceleration