#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-aiofiles
PKG_VERSION:=0.7.0
PKG_RELEASE:=1

PYPI_NAME:=aiofiles
PKG_HASH:=a1c4fc9b2ff81568c83e21392a82f344ea9d23da906e4f6a52662764545e19d4

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_LICENSE:=MIT
PKG_LICENSE_FILES:=LICENSE

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-aiofiles
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=File support for asyncio.
  URL:=https://pypi.org/project/aiofiles/
  DEPENDS:= +python3-light
endef

define Package/python3-ha-aiofiles/description
  aiofiles is an Apache2 licensed library, written in Python, for handling local disk files in asyncio applications.
endef

$(eval $(call Py3Package,python3-ha-aiofiles))
$(eval $(call BuildPackage,python3-ha-aiofiles))
