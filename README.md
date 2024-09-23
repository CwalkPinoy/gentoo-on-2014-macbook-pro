# gentoo on 4014 macbook pro
 stuff i need to know for gentoo on a 2014 macbook pro

uefi amd64 handbook is fine
mate has slow and buggy performance, xfce seems to work fine
broadcom-sta is unmaintained and requires custom kernel, i bought this to solve the issue
https://www.amazon.com/dp/B008IFXQFU? tp-link tl-wn725n

XFCE seems to work. MATE glitches out without proprietary drivers.

USE="wayland gles2 dist-kernel"

VIDEO_CARDS="nvidia"

/etc/portage/package.mask

```>x11-drivers/nvidia-drivers-471```

/etc/portage/package.use/nvidia-drivers

```x11-drivers/nvidia-drivers tools```

go to nvidia settings, advanced force composition

UTM on MacOS

enable 3d acceleration
switch display to virtio-vga-gl
