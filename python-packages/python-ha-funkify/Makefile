#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-funkify
PKG_VERSION:=0.3.0
PKG_RELEASE:=1

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_LICENSE:=MIT
PKG_LICENSE_FILES:=LICENSE.txt

PYPI_NAME:=funkify
PKG_HASH:=a7273eac299f37d0785b7b99a581ee20885451637355e589e653a32d8bd6eaad

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-funkify
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=Funkify modules
  URL:=https://pypi.org/project/funkify/
  DEPENDS:=+python3-light
endef

define Package/python3-ha-funkify/description
 Funkify modules so that they are callable.
endef

$(eval $(call Py3Package,python3-ha-funkify))
$(eval $(call BuildPackage,python3-ha-funkify))
