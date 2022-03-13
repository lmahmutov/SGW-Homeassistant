#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-pyric
PKG_VERSION:=0.1.6.3
PKG_RELEASE:=1

PYPI_NAME:=pyric
PKG_HASH:=b539b01cafebd2406c00097f94525ea0f8ecd1dd92f7731f43eac0ef16c2ccc9

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_LICENSE:=MIT
PKG_LICENSE_FILES:=LICENSE

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-pyric
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=Python Wireless Library
  URL:=https://pypi.org/project/pyric/
  DEPENDS:=  \
	+python3-light
endef

define Package/python3-ha-pyric/description
Python Wireless Library.
endef

$(eval $(call Py3Package,python3-ha-pyric))
$(eval $(call BuildPackage,python3-ha-pyric))
