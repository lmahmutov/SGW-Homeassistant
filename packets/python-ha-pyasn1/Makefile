#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-pyasn1
PKG_VERSION:=0.4.8
PKG_RELEASE:=2

PYPI_NAME:=pyasn1
PKG_HASH:=aef77c9fb94a3ac588e87841208bdec464471d9871bd5050a287cc9a475cd0ba

PKG_LICENSE:=BSD-2-Clause
PKG_LICENSE_FILES:=LICENSE.txt
PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-pyasn1
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=ASN.1 library for Python
  URL:=https://github.com/etingof/pyasn1
  DEPENDS:=+python3-light
endef

define Package/python3-ha-pyasn1/description
This is an implementation of ASN.1 types and codecs in Python programming
language. It has been first written to support particular protocol (SNMP)
but then generalized to be suitable for a wide range of protocols
based on ASN.1 specification.
endef

$(eval $(call Py3Package,python3-ha-pyasn1))
$(eval $(call BuildPackage,python3-ha-pyasn1))
