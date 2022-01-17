#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-python-miio
PKG_VERSION:=0.5.9.2
PKG_RELEASE:=1

PYPI_NAME:=python-miio
PKG_HASH:=005c1aad18459277f04d2bd20c6a1613efe6bf52940f65e758aff1081aab378a

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_LICENSE:=MIT
PKG_LICENSE_FILES:=LICENSE

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-python-miio
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:= library for interfacing with Xiaomi
  URL:=https://pypi.org/project/python-miio/
  DEPENDS:=+python3-light
endef

define Package/python3-ha-python-miio/description
  Python library for interfacing with Xiaomi smart appliances.
endef

$(eval $(call Py3Package,python3-ha-python-miio))
$(eval $(call BuildPackage,python3-ha-python-miio))
