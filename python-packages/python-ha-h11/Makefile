#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-h11
PKG_VERSION:=0.12.0
PKG_RELEASE:=1

PYPI_NAME:=h11
PKG_HASH:=47222cb6067e4a307d535814917cd98fd0a57b6788ce715755fa2b6c28b56042

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_LICENSE:=MIT
PKG_LICENSE_FILES:=LICENSE

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-h11
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=This is a little HTTP/1.1 library.
  URL:=https://pypi.org/project/h11/
  DEPENDS:=+python3-light
endef

define Package/python3-ha-h11/description
  This is a little HTTP/1.1 library written from scratch in Python, heavily
 inspired by hyper-h2.
endef

$(eval $(call Py3Package,python3-ha-h11))
$(eval $(call BuildPackage,python3-ha-h11))
