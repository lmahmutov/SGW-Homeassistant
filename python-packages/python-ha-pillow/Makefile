#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-pillow
PKG_VERSION:=9.1.1
PKG_RELEASE:=1

PYPI_NAME:=Pillow
PKG_HASH:=7502539939b53d7565f3d11d87c78e7ec900d3c72945d4ee0e2f250d598309a0

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_LICENSE:=HPND
PKG_LICENSE_FILES:=LICENSE
PKG_CPE_ID:=cpe:/a:python:pillow

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-pillow
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=The friendly PIL fork
  URL:=https://python-pillow.org/
  DEPENDS:=+libfreetype +libjpeg +libtiff +zlib +python3
endef

define Package/python3-pillow/description
  The friendly PIL fork
endef

PYTHON3_PKG_SETUP_GLOBAL_ARGS += build_ext \
	--enable-zlib \
	--enable-jpeg \
	--enable-tiff \
	--enable-freetype \
	--disable-lcms \
	--disable-webp \
	--disable-webpmux \
	--disable-jpeg2000 \
	--disable-imagequant \
	--disable-platform-guessing

$(eval $(call Py3Package,python3-ha-pillow))
$(eval $(call BuildPackage,python3-ha-pillow))
