#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-pygithub
PKG_VERSION:=1.55
PKG_RELEASE:=1

PYPI_NAME:=PyGithub
PKG_HASH:=1bbfff9372047ff3f21d5cd8e07720f3dbfdaf6462fcaed9d815f528f1ba7283

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_LICENSE:=MIT
PKG_LICENSE_FILES:=LICENSE

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-pygithub
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=Use the full Github API v3.
  URL:=https://pypi.org/project/pygithub/
  DEPENDS:= \
	+python3-ha-pyjwt
endef

define Package/python3-ha-pygithub/description
 Github API v3 python implementation.
endef

$(eval $(call Py3Package,python3-ha-pygithub))
$(eval $(call BuildPackage,python3-ha-pygithub))
