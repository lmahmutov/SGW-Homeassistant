#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-micloud
PKG_VERSION:=0.4
PKG_RELEASE:=1

PYPI_NAME:=micloud
PKG_HASH:=a3966bc9fabfc739ca15e07dc0ad42ff4c473fe3969a34f3e6d282b541456fab

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_LICENSE:=MIT
PKG_LICENSE_FILES:=LICENSE

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-micloud
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=Xiaomi cloud connect library
  URL:=https://pypi.org/project/micloud/
  DEPENDS:=  \
	+python3-light
endef

define Package/python3-ha-micloud/description
 Xiaomi cloud connect library.
endef

$(eval $(call Py3Package,python3-ha-micloud))
$(eval $(call BuildPackage,python3-ha-micloud))
