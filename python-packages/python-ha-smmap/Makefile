#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-smmap
PKG_VERSION:=5.0.0
PKG_RELEASE:=1

PYPI_NAME:=smmap
PKG_HASH:=c840e62059cd3be204b0c9c9f74be2c09d5648eddd4580d9314c3ecde0b30936

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_LICENSE:=MIT
PKG_LICENSE_FILES:=LICENSE

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-smmap
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:= sliding window memory map manager
  URL:=https://pypi.org/project/smmap/
  DEPENDS:=+python3-light
endef

define Package/python3-ha-smmap/description
 A pure Python implementation of a sliding window memory map manager.
endef

$(eval $(call Py3Package,python3-ha-smmap))
$(eval $(call BuildPackage,python3-ha-smmap))
