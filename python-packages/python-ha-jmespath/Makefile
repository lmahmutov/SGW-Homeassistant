#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-jmespath
PKG_VERSION:=0.9.3
PKG_RELEASE:=2

PYPI_NAME:=jmespath
PKG_HASH:=6a81d4c9aa62caf061cb517b4d9ad1dd300374cd4706997aff9cd6aedd61fc64

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_LICENSE:=MIT

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-jmespath
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=jmespath
  URL:=https://github.com/jmespath/jmespath.py
  DEPENDS:=+python3
endef

define Package/python3-ha-jmespath/description
  JMESPath (pronounced “james path”) allows you to declaratively specify how to extract
  elements from a JSON document.
endef

$(eval $(call Py3Package,python3-ha-jmespath))
$(eval $(call BuildPackage,python3-ha-jmespath))
