FROM archlinux/base

RUN useradd -m -G wheel aur

RUN pacman -Syu --noconfirm base-devel

RUN sh -c "echo '%wheel ALL=(ALL) NOPASSWD: ALL' > /etc/sudoers.d/wheel-nopass"

WORKDIR /aur

VOLUME /aur
