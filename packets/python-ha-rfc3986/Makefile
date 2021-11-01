#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-rfc3986
PKG_VERSION:=1.4.0
PKG_RELEASE:=1

PYPI_NAME:=rfc3986
PKG_HASH:=112398da31a3344dc25dbf477d8df6cb34f9278a94fee2625d89e4514be8bb9d

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_LICENSE:=Apache-2.0
PKG_LICENSE_FILES:=LICENSE

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-rfc3986
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=Validating URI References per RFC 3986.
  URL:=https://pypi.org/project/rfc3986/
  DEPENDS:=+python3-ha-idna
endef

define Package/python3-ha-rfc3986/description
  A Python implementation of RFC 3986 including validation and authority parsing.
endef

$(eval $(call Py3Package,python3-ha-rfc3986))
$(eval $(call BuildPackage,python3-ha-rfc3986))
