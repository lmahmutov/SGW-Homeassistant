#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-python-miio
PKG_VERSION:=0.5.8
PKG_RELEASE:=1

PYPI_NAME:=python-miio
PKG_HASH:=d7a5c46a1e6b81e9bf2fc03fce8d733eb89fad4d7954c93ae76ac52d972f8e28

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
