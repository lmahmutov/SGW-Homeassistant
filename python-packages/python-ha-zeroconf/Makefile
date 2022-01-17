#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-zeroconf
PKG_VERSION:=0.38.1
PKG_RELEASE:=1

PYPI_NAME:=zeroconf
PKG_HASH:=10c501b25d8881b656e56c34674d98fe6bc752240a572e74f918bc849c93ba9c

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_LICENSE:=Apache-2.0
PKG_LICENSE_FILES:=COPYING

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-zeroconf
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=Multicast DNS Service Discovery Library
  URL:=https://github.com/jstasiak/python-zeroconf
  DEPENDS:= \
	  +python3-light \
	  +python3-logging \
	  +python3-ha-ifaddr
endef

define Package/python3-ha-zeroconf/description
  Pure Python Multicast DNS Service Discovery Library (Bonjour/Avahi compatible)
endef

$(eval $(call Py3Package,python3-ha-zeroconf))
$(eval $(call BuildPackage,python3-ha-zeroconf))
