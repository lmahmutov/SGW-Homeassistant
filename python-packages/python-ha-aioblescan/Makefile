#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-aioblescan
PKG_VERSION:=0.2.9
PKG_RELEASE:=1

PYPI_NAME:=aioblescan
PKG_HASH:=8e9b5b8f3396b573cb2ce63f232f1fc42050ef64ecace0af878c49a281c79270

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_LICENSE:=Apache-2.0
PKG_LICENSE_FILES:=COPYING

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-aioblescan
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=Scanning Bluetooth for advertised
  URL:=https://pypi.org/project/aioblescan/
  DEPENDS:= \
	  +python3-light
endef

define Package/python3-ha-aioblescan/description
  Scanning Bluetooth for advertised
endef

$(eval $(call Py3Package,python3-ha-aioblescan))
$(eval $(call BuildPackage,python3-ha-aioblescan))
