#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-pyusb
PKG_VERSION:=1.2.1
PKG_RELEASE:=1

PYPI_NAME:=pyusb
PKG_HASH:=a4cc7404a203144754164b8b40994e2849fde1cfff06b08492f12fff9d9de7b9

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_LICENSE:=MIT
PKG_LICENSE_FILES:=LICENSE

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-pyusb
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=Python USB access module.
  URL:=https://pypi.org/project/pyusb/
  DEPENDS:= +python3-ha-humanfriendly \
	+python3-ha-pyrsistent
endef

define Package/python3-ha-pyusb/description
 PyUSB offers easy USB devices communication in Python.
endef

$(eval $(call Py3Package,python3-ha-pyusb))
$(eval $(call BuildPackage,python3-ha-pyusb))
