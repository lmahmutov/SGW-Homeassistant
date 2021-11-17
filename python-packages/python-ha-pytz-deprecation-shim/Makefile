#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-pytz-deprecation-shim
PKG_VERSION:=0.1.0.post0
PKG_RELEASE:=1

PYPI_NAME:=pytz_deprecation_shim
PKG_HASH:=af097bae1b616dde5c5744441e2ddc69e74dfdcb0c263129610d85b87445a59d

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_LICENSE:=MIT
PKG_LICENSE_FILES:=LICENSE

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-pytz-deprecation-shim
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=Shims to make deprecation of pytz easier
  URL:=https://pypi.org/project/pytz-deprecation-shim/
  DEPENDS:=  \
	+python3-light
endef

define Package/python3-ha-pytz-deprecation-shim/description
 Shims to make deprecation of pytz easier.
endef

$(eval $(call Py3Package,python3-ha-pytz-deprecation-shim))
$(eval $(call BuildPackage,python3-ha-pytz-deprecation-shim))
