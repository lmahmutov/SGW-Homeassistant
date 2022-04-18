#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-pyqrcode
PKG_VERSION:=1.2.1
PKG_RELEASE:=1

PYPI_NAME:=PyQRCode
PYPI_SOURCE_EXT:=zip
PKG_HASH:=1b2812775fa6ff5c527977c4cd2ccb07051ca7d0bc0aecf937a43864abe5eff6

PKG_LICENSE:=BSD-3-Clause
PKG_LICENSE_FILES:=LICENSE
PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-pyqrcode
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=A QR code generator
  URL:=https://pypi.org/project/pyqrcode/
  DEPENDS:=+python3-ha-pypng
endef

define Package/python3-ha-pyqrcode/description
 A QR code generator written purely in Python with SVG, EPS, PNG and terminal
 output.
endef

$(eval $(call Py3Package,python3-ha-pyqrcode))
$(eval $(call BuildPackage,python3-ha-pyqrcode))
