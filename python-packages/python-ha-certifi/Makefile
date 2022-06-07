#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-certifi
PKG_VERSION:=2022.5.18.1
PKG_RELEASE:=1

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_LICENSE:=MPL-2.0
PKG_LICENSE_FILES:=LICENSE

PYPI_NAME:=certifi
PKG_HASH:=9c5705e395cd70084351dd8ad5c41e65655e08ce46f2ec9cf6c2c08390f71eb7

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-certifi
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=(HA CORE) Python package for Mozilla's CA Bundle
  URL:=http://certifi.io/
  DEPENDS:=+python3-light
endef

define Package/python3-ha-certifi/description
  Certifi is a carefully curated collection of Root Certificates for validating the
  trustworthiness of SSL certificates while verifying the identity of TLS hosts.
endef

$(eval $(call Py3Package,python3-ha-certifi))
$(eval $(call BuildPackage,python3-ha-certifi))

