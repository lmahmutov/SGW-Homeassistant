#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-future
PKG_VERSION:=0.18.2
PKG_RELEASE:=1

PYPI_NAME:=future
PKG_HASH:=a3966bc9fabfc739ca15e07dc0ad42ff4c473fe3969a34f3e6d282b541456fab

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_LICENSE:=MIT
PKG_LICENSE_FILES:=LICENSE

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-future
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=Clean single-source
  URL:=https://pypi.org/project/future/
  DEPENDS:=  \
	+python3-light
endef

define Package/python3-ha-future/description
 future is the missing compatibility layer between Python 2
 and Python 3. It allows you to use a single, clean Python 3.x-compatible
 codebase to support both Python 2 and Python 3 with minimal overhead.
endef

$(eval $(call Py3Package,python3-ha-future))
$(eval $(call BuildPackage,python3-ha-future))
