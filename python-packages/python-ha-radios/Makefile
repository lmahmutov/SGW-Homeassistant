#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-radios
PKG_VERSION:=0.1.1
PKG_RELEASE:=1

PYPI_NAME:=radios
PKG_HASH:=9ac0aaffc1476d47d6766b2adb35aea5039713aec6d20669ff008bffaa4d599e

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_LICENSE:=MIT
PKG_LICENSE_FILES:=LICENSE

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-radios
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=Python client for the Radio Browser API.
  URL:=https://pypi.org/project/radios/
  DEPENDS:= \
	+python3-light	\
	+python3-ha-aiodns \
	+python3-ha-aiohttp \
	+python3-ha-awesomeversion \
	+python3-ha-backoff \
	+python3-ha-cachetools \
	+python3-ha-pycountry \
	+python3-ha-pydantic \
	+python3-ha-yarl
endef

define Package/python3-ha-radios/description
 Asynchronous Python client for the Radio Browser API.
endef

$(eval $(call Py3Package,python3-ha-radios))
$(eval $(call BuildPackage,python3-ha-radios))
