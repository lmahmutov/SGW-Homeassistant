#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-pytest-asyncio
PKG_VERSION:=0.15.1
PKG_RELEASE:=1

PYPI_NAME:=pytest-asyncio
PKG_HASH:=2564ceb9612bbd560d19ca4b41347b54e7835c2f792c504f698e05395ed63f6f

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_LICENSE:=MIT
PKG_LICENSE_FILES:=LICENSE

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-pytest-asyncio
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=Pytest support for asyncio.
  URL:=https://pypi.org/project/pytest-asyncio/
  DEPENDS:= 
endef

define Package/python3-ha-pytest-asyncio/description
 pytest-asyncio is an Apache2 licensed library, 
 written in Python, for testing asyncio code with pytest..
endef

$(eval $(call Py3Package,python3-ha-pytest-asyncio))
$(eval $(call BuildPackage,python3-ha-pytest-asyncio))
