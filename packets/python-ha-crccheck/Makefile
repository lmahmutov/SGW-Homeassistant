#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-crccheck
PKG_VERSION:=1.0
PKG_RELEASE:=1

PYPI_NAME:=crccheck
PKG_HASH:=17c42dc4f069308ae962b682b2974bdbf2f80ee682c7032a9df44880fca3c9ab

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_LICENSE:=MIT
PKG_LICENSE_FILES:=LICENSE

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-crccheck
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=Calculation library for CRCs and checksums.
  URL:=https://pypi.org/project/crccheck/
  DEPENDS:= 
endef

define Package/python3-ha-crccheck/description
 The crccheck.crc module implements all CRCs listed in the Catalogue of parametrised CRC algorithms.
endef

$(eval $(call Py3Package,python3-ha-crccheck))
$(eval $(call BuildPackage,python3-ha-crccheck))
