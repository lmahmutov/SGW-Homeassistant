#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-snitun
PKG_VERSION:=0.30.0
PKG_RELEASE:=1

PYPI_NAME:=snitun
PKG_HASH:=20a543852b233249e9a453e5a3164eeae50f438b3eb53753ce746ce42261a125

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_LICENSE:=GPL-3.0-or-later
PKG_LICENSE_FILES:=LICENSE

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-snitun
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=SNI proxy with TCP multiplexer
  URL:=https://pypi.org/project/snitun/
  DEPENDS:=+python3-ha-async-timeout \
	+python3-ha-attrs \
	+python3-ha-cryptography
endef

define Package/python3-ha-snitun/description
  End-to-End encryption with SNI proxy on top of a TCP multiplexer.
endef

$(eval $(call Py3Package,python3-ha-snitun))
$(eval $(call BuildPackage,python3-ha-snitun))
