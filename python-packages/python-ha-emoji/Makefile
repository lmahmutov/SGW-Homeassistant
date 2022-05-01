#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-emoji
PKG_VERSION:=1.5.0
PKG_RELEASE:=1

PYPI_NAME:=emoji
PKG_HASH:=2eddd062f940924fb25a3108d84d77dc571927d91a419b4c30f37e253c791b19

PKG_LICENSE:=BSD-3-Clause
PKG_LICENSE_FILES:=LICENSE
PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-emoji
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=Emoji for Python
  URL:=https://pypi.org/project/emoji/
  DEPENDS:=+python3-light
endef

define Package/python3-ha-emoji/description
  Emoji for Python. This project was inspired by kyokomi.
endef

$(eval $(call Py3Package,python3-ha-emoji))
$(eval $(call BuildPackage,python3-ha-emoji))
