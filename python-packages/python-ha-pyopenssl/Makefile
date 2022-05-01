#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-pyopenssl
PKG_VERSION:=20.0.1
PKG_RELEASE:=1

PYPI_NAME:=pyOpenSSL
PKG_HASH:=4c231c759543ba02560fcd2480c48dcec4dae34c9da7d3747c508227e0624b51

PKG_LICENSE:=Apache-2.0
PKG_LICENSE_FILES:=LICENSE
PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_CPE_ID:=cpe:/a:pyopenssl_project:pyopenssl

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-pyopenssl
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=OpenSSL wrapper
  URL:=https://pyopenssl.org/
  DEPENDS:= \
      +python3-light \
      +python3-ha-cryptography \
      +python3-ha-six
endef

define Package/python3-ha-pyopenssl/description
Python wrapper module around the OpenSSL library
endef

$(eval $(call Py3Package,python3-ha-pyopenssl))
$(eval $(call BuildPackage,python3-ha-pyopenssl))
