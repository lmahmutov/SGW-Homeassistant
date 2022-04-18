#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-aiodns
PKG_VERSION:=3.0.0
PKG_RELEASE:=1

PYPI_NAME:=aiodns
PKG_HASH:=946bdfabe743fceeeb093c8a010f5d1645f708a241be849e17edfb0e49e08cd6

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_LICENSE:=MIT
PKG_LICENSE_FILES:=LICENSE

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-aiodns
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=Simple DNS resolver for asyncio.
  URL:=https://pypi.org/project/aiodns/
  DEPENDS:= \
	+python3-light
endef

define Package/python3-ha-aiodns/description
 Simple DNS resolver for asyncio.
endef

$(eval $(call Py3Package,python3-ha-aiodns))
$(eval $(call BuildPackage,python3-ha-aiodns))
