#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=ha-wled
PKG_VERSION:=0.13.2
PKG_RELEASE:=1

PYPI_NAME:=wled
PKG_HASH:=85a3f23f94c8c47cd99c171deed784be59ecda8002a6c1516a596f18acb41ac1

PKG_LICENSE:=MIT
PKG_LICENSE_FILES:=LICENSE
PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/ha-wled
  CATEGORY:=Homeassistant
  SUBMENU:=Components
  TITLE:=Python client for WLED.
  URL:=https://pypi.org/project/wled/
  DEPENDS:= +homeassistant \
	+python3-ha-backoff \
	+python3-ha-packaging \
	+python3-ha-cachetools
endef

define Package/ha-wled/description
 Asynchronous Python client for WLED.
endef

$(eval $(call Py3Package,ha-wled))
$(eval $(call BuildPackage,ha-wled))
