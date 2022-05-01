#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-toml
PKG_VERSION:=0.10.2
PKG_RELEASE:=1

PYPI_NAME:=toml
PKG_HASH:=b3bda1d108d5dd99f4a20d24d9c348e91c4db7ab1b749200bded2f839ccbe68f

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_LICENSE:=MIT
PKG_LICENSE_FILES:=LICENSE

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-toml
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=A Python library for parsing and creating TOML
  URL:=https://github.com/uiri/toml
  DEPENDS:=  \
	+python3-light \
	+python3-decimal
endef

define Package/python3-ha-toml/description
  Python Library for Tom's Obvious, Minimal Language
endef

$(eval $(call Py3Package,python3-ha-toml))
$(eval $(call BuildPackage,python3-ha-toml))
