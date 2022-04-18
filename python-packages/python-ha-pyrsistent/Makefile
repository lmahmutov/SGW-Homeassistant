#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-pyrsistent
PKG_VERSION:=0.16.0
PKG_RELEASE:=1

PYPI_NAME:=pyrsistent
PKG_HASH:=28669905fe725965daa16184933676547c5bb40a5153055a8dee2a4bd7933ad3

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_LICENSE:=MIT
PKG_LICENSE_FILES:=LICENSE.mit

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-pyrsistent
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=Persistent/Functional/Immutable data structures
  URL:=https://github.com/tobgu/pyrsistent
  DEPENDS:= \
	+python3-light \
	+python3-ha-six
endef

define Package/python3-ha-pyrsistent/description
  Pyrsistent is a number of persistent collections (by some referred to as functional data structures).
  Persistent in the sense that they are immutable.
endef

$(eval $(call Py3Package,python3-ha-pyrsistent))
$(eval $(call BuildPackage,python3-ha-pyrsistent))
