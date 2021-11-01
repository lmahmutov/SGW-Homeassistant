#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-yarl
PKG_VERSION:=1.6.3
PKG_RELEASE:=1

PYPI_NAME:=yarl
PKG_HASH:=8a9066529240171b68893d60dca86a763eae2139dd42f42106b03cf4b426bf10

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_LICENSE:=Apache-2.0
PKG_LICENSE_FILES:=LICENSE

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-yarl
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=(HA CORE) Yet another URL library
  URL:=https://github.com/aio-libs/yarl
  DEPENDS:= \
  +python3-light \
  +python3-ha-multidict \
  +python3-urllib \
  +python3-ha-idna
endef

define Package/python3-ha-yarl/description
Yet another URL library
endef

$(eval $(call Py3Package,python3-ha-yarl))
$(eval $(call BuildPackage,python3-ha-yarl))

