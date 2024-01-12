# Awesome IP Camera [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> A list of IP Camera related stuff. Because the IP Camera ecosystem is definitely not awesome, there&#39;s a low bar to inclusion.


## Contents

- [Generic software](#generic-software)
- [NVR software](#nvr-or-management)
- [Chip specific software](#chip-specific-software)


## Generic software

Projects that target multiple IP cameras or use generic Linux interfaces.

### Firmware

- [OpenIPC](https://openipc.org)

### Video Streaming

- [MediaMTX](https://github.com/bluenviron/mediamtx)
- [go2rtc](https://github.com/AlexxIT/go2rtc)
- [V4L2 rtspserver](https://github.com/mpromonet/v4l2rtspserver)
- [GStreamer](https://gstreamer.freedesktop.org/documentation/additional/rtp.html)
- [LIVE555](http://www.live555.com/)
- [smolrtsp](https://github.com/OpenIPC/smolrtsp)

### ONVIF

#### Libraries

- [gsoap ONVIF examples](https://www.genivia.com/examples/onvif/index.html)
- [libonvif](https://github.com/sr99622/libonvif)
- [libONVIF](https://github.com/Tereius/libONVIF)
- [onvif](https://github.com/agsh/onvif) - Javascript client
- [onvif](https://github.com/use-go/onvif) - Go client

#### Servers

- [rpos](https://github.com/BreeeZe/rpos) - Raspberry PI ONVIF server, but will work any v4l2
- [v4l2onvif](https://github.com/mpromonet/v4l2onvif)
- [onvif_srvd](https://github.com/KoynovStas/onvif_srvd)
- [generic-onvif-server](https://github.com/n1tsu/generic-onvif-server)

#### Clients

See also [NVR section](#nvr).

- [ONVIFViewer](https://gitlab.com/caspermeijn/onvifviewer)
- [ODM](https://sourceforge.net/projects/onvifdm/) - official ONVIF Device Manager
- [OnvifDeviceManager](https://github.com/Quedale/OnvifDeviceManager)
- [Open Camera](https://github.com/eltonkola/opencamera)
- [Onvier - IP Camera Monitor](https://www.ipcent.com/mobile/onvifer)
- [libonvif](https://github.com/sr99622/libonvif) - includes client applications

## NVR or Management

- [Home Assistant WebRTC](https://github.com/AlexxIT/WebRTC)
- [Home Assistant Camera integration](https://www.home-assistant.io/integrations/generic/)
- [Frigate](https://docs.frigate.video/)
- [ZoneMinder](https://zoneminder.com/)
- [motionEye](https://github.com/motioneye-project/motioneye)
- [Shinobi](https://shinobi.video/)


## Chip specific software

Projects that target a particular chipset or a chipset family
from a particular manufacturer.

### Ingenic

#### Firmware

These firmwares tend to have interesting software scattered around
in their packages, some of which only exists in their repo. Only
some of these are called out below.

- [OpenMiko](https://github.com/openmiko/openmiko)
- [atomcam_tools](https://github.com/mnakada/atomcam_tools)
- [DaFang Hacks](https://github.com/Dafang-Hacks/Main)
  - [Xiaomi DaFang Hacks](https://github.com/EliasKotlyar/Xiaomi-Dafang-Hacks)
- [wyrecam](https://github.com/radredgreen/wyrecam) - based on OpenIPC
- [wz_mini_hacks](https://github.com/gtxaspec/wz_mini_hacks)

#### Camera software

- [openingenic](https://github.com/OpenIPC/openingenic) - part of openipc
- [libimp_control](https://github.com/gtxaspec/libimp_control) - part of openipc
- push to v4l2 from libimp
  - [ingenic_videocap](https://github.com/openmiko/ingenic_videocap)
  - [libcallback](https://github.com/mnakada/atomcam_tools/tree/b482274bb789aebe7436c474f6d23612b0e32580/libcallback) - part of atomcam_tools
- standalone servers
  - [rtspServer](https://github.com/Dafang-Hacks/Main/tree/master/rtspServer)
  - [v4l2rtspserver](https://github.com/Dafang-Hacks/Main/tree/master/v4l2rtspserver-master) - this is the original v4l2rtspserver with libimp as a source (i.e. does _not_ use v4l2; README is not updated)
- simple servers based on libimp -> fifo -> live555 (no sound)
  - [carrier-rtsp-server](https://github.com/beihuijie/carrier-rtsp-server)
  - [t31-rtspd](https://github.com/radredgreen/t31-rtspd)
  - [t20-rtspd](https://github.com/geekman/t20-rtspd)


## Contribute

Contributions welcome! Read the [contribution guidelines](contributing.md) first.