#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-pymetno
PKG_VERSION:=0.9.0
PKG_RELEASE:=1

PYPI_NAME:=PyMetno
PKG_HASH:=9845a900577cea3803cb6002a1108bf1aab6c89fcff8d8fe46682351fb82a3ed

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_LICENSE:=MIT
PKG_LICENSE_FILES:=LICENSE

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-pymetno
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:= A library to communicate with the met.no api.
  URL:=https://pypi.org/project/pymetno/
  DEPENDS:= \
	+python3-ha-aiohttp \
	+python3-ha-async-timeout \
	+python3-ha-pytz \
	+python3-ha-xmltodict
endef

define Package/python3-ha-pymetno/description
 A library to communicate with the met.no api.
endef

$(eval $(call Py3Package,python3-ha-pymetno))
$(eval $(call BuildPackage,python3-ha-pymetno))
