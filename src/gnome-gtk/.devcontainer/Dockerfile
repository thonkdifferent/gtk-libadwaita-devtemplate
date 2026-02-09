FROM quay.io/gnome_infrastructure/gnome-build-meta:core-${templateOption:sdkVersion}
RUN useradd -m -s /bin/bash vscode
RUN mkdir -p /run/user/1001
RUN chown -R 1001:1001 /run/user/1001
RUN systemd-machine-id-setup