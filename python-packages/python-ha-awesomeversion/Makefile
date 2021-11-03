#
# Copyright (C) 2021 @lmahmutov
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-awesomeversion
PKG_VERSION:=21.8.1
PKG_RELEASE:=1

PYPI_NAME:=awesomeversion
PKG_HASH:=a72f3fff12df257e30f5e25a8550fc4da62e7591d5fdb70714f5c96827c37645

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

