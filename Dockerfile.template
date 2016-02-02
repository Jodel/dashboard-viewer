FROM resin/%%RESIN_MACHINE_NAME%%-python

ENV DEBIAN_FRONTEND noninteractive

RUN apt-get update && apt-get install -y \
  iceweasel dropbear xserver-xorg-core xserver-xorg-video-fbdev x11-xserver-utils \
  libgl1-mesa-dri xserver-xorg-video-modesetting xserver-xorg-video-vesa \
  matchbox-window-manager openvpn xautomation feh \
  && apt-get clean && rm -rf /var/lib/apt/lists/*

ADD run /bin/run
ADD jodel-wallpaper.png /etc/wallpaper.png
ADD dot-mozilla /root/.mozilla

ENTRYPOINT [ "/bin/run" ]
