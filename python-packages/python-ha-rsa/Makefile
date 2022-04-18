#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-rsa
PKG_VERSION:=4.6
PKG_RELEASE:=1

PYPI_NAME:=rsa
PKG_HASH:=109ea5a66744dd859bf16fe904b8d8b627adafb9408753161e766a92e7d681fa

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_LICENSE:=MIT
PKG_CPE_ID:=cpe:/a:python-rsa_project:python-rsa

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-rsa
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=rsa
  URL:=https://stuvel.eu/rsa
  DEPENDS:= \
	+python3 \
	+python3-ha-pyasn1
endef

define Package/python3-ha-rsa/description
  Is a pure-Python RSA implementation. It supports encryption and decryption,
  signing and verifying signatures, and key generation according to PKCS#1 version 1.5.
  It can be used as a Python library as well as on the commandline. 
endef

$(eval $(call Py3Package,python3-ha-rsa))
$(eval $(call BuildPackage,python3-ha-rsa))
