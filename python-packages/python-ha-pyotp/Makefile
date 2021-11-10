#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-pyotp
PKG_VERSION:=2.6.0
PKG_RELEASE:=2

PYPI_NAME:=pyotp
PKG_HASH:=d28ddfd40e0c1b6a6b9da961c7d47a10261fb58f378cb00f05ce88b26df9c432

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_LICENSE:=MIT
PKG_LICENSE_FILES:=LICENSE

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-pyotp
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=Python One-Time Password Library
  URL:=https://github.com/pyauth/pyotp
  DEPENDS:=+python3-light
endef

define Package/python3-ha-pyotp/description
  PyOTP is a Python library for generating and verifying one-time passwords.
  It can be used to implement two-factor (2FA) or multi-factor (MFA) authentication methods
  in web applications and in other systems that require users to log in.
endef

$(eval $(call Py3Package,python3-ha-pyotp))
$(eval $(call BuildPackage,python3-ha-pyotp))
