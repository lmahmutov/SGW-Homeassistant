#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-ffmpeg
PKG_VERSION:=3.0.2
PKG_RELEASE:=1

PYPI_NAME:=ha-ffmpeg
PKG_HASH:=8d92f2f5790da038d828ac862673e0bb43e8e972e4c70b1714dd9a0fb776c8d1

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_LICENSE:=BSD-3-Clause
PKG_LICENSE_FILES:=LICENSE

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-ffmpeg
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=ffmpeg for home-assistant.
  URL:=https://pypi.org/project/ha-ffmpeg/
  DEPENDS:= \
	+ffmpeg \
	+python3-ha-async-timeout
endef

define Package/python3-ha-ffmpeg/description
 Home-Assistant ffmpeg interface.
 .
 A python library that handling with ffmpeg for home-assistant Async
 - Emulate webcam from any video input source for HA
 - Analyse a video/audio stream for noise or motion detection
 - Grab image from a stream.
endef

$(eval $(call Py3Package,python3-ha-ffmpeg))
$(eval $(call BuildPackage,python3-ha-ffmpeg))
