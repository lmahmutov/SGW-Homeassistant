#
# Copyright (C) 2021 @lmahmutov
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-awesomeversion
PKG_VERSION:=21.10.1
PKG_RELEASE:=1

PYPI_NAME:=awesomeversion
PKG_HASH:=871318fbb7940d0e36ba6f9b3a07cc5ce84d810986522ef19262e82b55be5c8b

PKG_LICENSE:=MIT
PKG_LICENSE_FILES:=LICENSE
PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-awesomeversion
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=(HA CORE) AwesomeVersion
  URL:=https://pypi.org/project/awesomeversion/
  DEPENDS:=+python3-light
endef

define Package/python3-ha-awesomeversion/description
One version package to rule them all, One version package to find them, One version package to bring them all, and in the darkness bind them.
endef

$(eval $(call Py3Package,python3-ha-awesomeversion))
$(eval $(call BuildPackage,python3-ha-awesomeversion))

