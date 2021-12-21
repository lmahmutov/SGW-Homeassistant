#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-frozenlist
PKG_VERSION:=1.2.0
PKG_RELEASE:=1

PYPI_NAME:=frozenlist
PKG_HASH:=68201be60ac56aff972dc18085800b6ee07973c49103a8aba669dee3d71079de

PKG_LICENSE:=BSD-3-Clause
PKG_LICENSE_FILES:=LICENSE
PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-frozenlist
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=Python-frozenlist.
  URL:=https://pypi.org/project/frozenlist/
  DEPENDS:=+python3-light
endef

define Package/python3-ha-frozenlist/description
A list-like structure which implements collections.abc.MutableSequence.
endef

$(eval $(call Py3Package,python3-ha-frozenlist))
$(eval $(call BuildPackage,python3-ha-frozenlist))
