#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=ha-wled
PKG_VERSION:=0.8.0
PKG_RELEASE:=1

PYPI_NAME:=wled
PKG_HASH:=93a6ff4580e1ffe461807f6c86b7c506b5965579ff2b56101935ca8eec05d02e

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
	+python3-ha-packaging
endef

define Package/ha-wled/description
 Asynchronous Python client for WLED.
endef

$(eval $(call Py3Package,ha-wled))
$(eval $(call BuildPackage,ha-wled))
