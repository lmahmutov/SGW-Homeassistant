#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-ecdsa
PKG_VERSION:=0.16.0
PKG_RELEASE:=1

PYPI_NAME:=ecdsa
PKG_HASH:=494c6a853e9ed2e9be33d160b41d47afc50a6629b993d2b9c5ad7bb226add892

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_LICENSE:=MIT
PKG_LICENSE_FILES:=LICENSE

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-ecdsa
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=ECDSA cryptographic signature library.
  URL:=https://pypi.org/project/ecdsa/
  DEPENDS:= +python3-ha-six
endef

define Package/python3-ha-ecdsa/description
 This is an easy-to-use implementation of ECC (Elliptic Curve Cryptography) with support for ECDSA
 (Elliptic Curve Digital Signature Algorithm) and ECDH (Elliptic Curve Diffie-Hellman),
 implemented purely in Python, released under the MIT license.
endef

$(eval $(call Py3Package,python3-ha-ecdsa))
$(eval $(call BuildPackage,python3-ha-ecdsa))
