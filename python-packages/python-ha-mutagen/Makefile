#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-mutagen
PKG_VERSION:=1.45.1
PKG_RELEASE:=1

PYPI_NAME:=mutagen
PKG_HASH:=6397602efb3c2d7baebd2166ed85731ae1c1d475abca22090b7141ff5034b3e1

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_LICENSE:=GPL-2.0-or-later
PKG_LICENSE_FILES:=LICENSE

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-mutagen
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=Mutagen is a Python module to handle audio metadata.
  URL:=https://pypi.org/project/mutagen/
  DEPENDS:=+python3-light
endef

define Package/python3-ha-mutagen/description
  Mutagen is a Python module to handle audio metadata. It supports ASF,
 FLAC, MP4, Monkey’s Audio, MP3, Musepack, Ogg Opus, Ogg FLAC, Ogg Speex,
 Ogg Theora, Ogg Vorbis, True Audio, WavPack, OptimFROG, and AIFF audio
 files. All versions of ID3v2 are supported, and all standard ID3v2.4
 frames are parsed. It can read Xing headers to accurately calculate the
 bitrate and length of MP3s. ID3 and APEv2 tags can be edited regardless
 of audio format. It can also manipulate Ogg streams on an individual
 packet/page level.
endef

$(eval $(call Py3Package,python3-ha-mutagen))
$(eval $(call BuildPackage,python3-ha-mutagen))
