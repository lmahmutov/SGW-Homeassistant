#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-appdirs
PKG_VERSION:=1.4.4
PKG_RELEASE:=1

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_LICENSE:=MIT
PKG_LICENSE_FILES:=LICENSE.txt

PYPI_NAME:=appdirs
PKG_HASH:=7d5d0167b2b1ba821647616af46a749d1c653740dd0d2415100fe26e27afdf41

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-appdirs
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=A small Python module
  URL:=https://pypi.org/project/appdirs/
  DEPENDS:=+python3-light
endef

define Package/python3-ha-appdirs/description
 A small Python module for determining appropriate platform-specific dirs, e.g. a "user data dir"..
endef

$(eval $(call Py3Package,python3-ha-appdirs))
$(eval $(call BuildPackage,python3-ha-appdirs))
