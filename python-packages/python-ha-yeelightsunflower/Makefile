#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-yeelightsunflower
PKG_VERSION:=0.0.10
PKG_RELEASE:=1

PYPI_NAME:=yeelightsunflower
PKG_HASH:=978465e964822baf3f5c1c029dda2736ede478f0d77d2b3fb885da0a4ac84fb8

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_LICENSE:=MIT
PKG_LICENSE_FILES:=LICENSE

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-yeelightsunflower
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=Yeelight Sunflower bulbs
  URL:=https://pypi.org/project/yeelightsunflower/
  DEPENDS:=  \
	+python3-light
endef

define Package/python3-ha-yeelightsunflower/description
 Python package for interacting with Yeelight Sunflower bulbs.
endef

$(eval $(call Py3Package,python3-ha-yeelightsunflower))
$(eval $(call BuildPackage,python3-ha-yeelightsunflower))
