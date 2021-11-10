#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-jose
PKG_VERSION:=3.3.0
PKG_RELEASE:=1

PYPI_NAME:=python-jose
PKG_HASH:=55779b5e6ad599c6336191246e95eb2293a9ddebd555f796a65f838f07e5d78a

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_LICENSE:=BSD-3-Clause
PKG_LICENSE_FILES:=LICENSE

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-jose
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=A JOSE implementation in Python.
  URL:=https://pypi.org/project/python-jose/
  DEPENDS:= \
	+python3-ha-cryptodome \
	+python3-ha-ecdsa \
	+python3-ha-pyasn1 \
	+python3-ha-rsa \
	+python3-ha-six
endef

define Package/python3-ha-jose/description
 A JOSE implementation in Python.
 .
 The JavaScript Object Signing and Encryption (JOSE) technologies - JSON Web
 Signature (JWS), JSON Web Encryption (JWE), JSON Web Key (JWK), and JSON Web
 Algorithms (JWA) - collectively can be used to encrypt and/or sign content 
 using a variety of algorithms.
endef

$(eval $(call Py3Package,python3-ha-jose))
$(eval $(call BuildPackage,python3-ha-jose))
