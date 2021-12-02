#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-enum34
PKG_VERSION:=1.1.6
PKG_RELEASE:=1

PYPI_NAME:=enum34
PKG_HASH:=8ad8c4783bf61ded74527bffb48ed9b54166685e4230386a9ed9b1279e2df5b1

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_LICENSE:=BSD-3-Clause
PKG_LICENSE_FILES:=LICENSE

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-enum34
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=Python 3.4 Enum backported
  URL:=https://pypi.org/project/enum34/
  DEPENDS:=+python3-light
endef

define Package/python3-ha-enum34/description
 Python 3.4 Enum backported
endef

$(eval $(call Py3Package,python3-ha-enum34))
$(eval $(call BuildPackage,python3-ha-enum34))
