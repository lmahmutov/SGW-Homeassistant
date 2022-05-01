#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=hass-configurator
PKG_VERSION:=0.4.1
PKG_RELEASE:=1

PYPI_NAME:=hass-configurator
PKG_HASH:=5bc443fc693af688a3d84ee28e5ed40ad43adea2b13e8240c1cd81b8ac5bed57

PKG_LICENSE:=MIT
PKG_LICENSE_FILES:=LICENSE
PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/hass-configurator
  CATEGORY:=Homeassistant
  SUBMENU:=Components
  TITLE:=HASS-Configurator.
  URL:=https://pypi.org/project/hass-configurator/
  DEPENDS:= +homeassistant \
	+python3-ha-pyotp \
	+python3-ha-gitpython \
	+python3-ha-smmap
endef

define Package/hass-configurator/description
 HASS-Configurator.
endef

define Py3Package/hass-configurator/install
	$(INSTALL_DIR) $(1)/usr/bin 
	$(INSTALL_BIN) $(PKG_INSTALL_DIR)/usr/bin/hass-configurator $(1)/usr/bin

	$(INSTALL_DIR) $(1)/etc/init.d
	$(INSTALL_BIN) ./files/hass-configurator $(1)/etc/init.d
endef


$(eval $(call Py3Package,hass-configurator))
$(eval $(call BuildPackage,hass-configurator))
