#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-cryptography
PKG_VERSION:=3.4.8
PKG_RELEASE:=1

PYPI_NAME:=cryptography
PKG_HASH:=94cc5ed4ceaefcbe5bf38c8fba6a21fc1d365bb8fb826ea1688e3370b2e24a1c

PKG_LICENSE:=Apache-2.0 BSD-3-Clause
PKG_LICENSE_FILES:=LICENSE.APACHE LICENSE.BSD
PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>

PKG_BUILD_DEPENDS:=libffi/host

HOST_PYTHON3_PACKAGE_BUILD_DEPENDS:=cffi  # cffi>=1.12

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-cryptography
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=Cryptographic recipes and primitives
  URL:=https://github.com/pyca/cryptography
  DEPENDS:= \
      +libopenssl \
      +python3-light \
      +python3-email \
      +python3-openssl \
      +python3-urllib \
      +python3-ha-cffi \
      +python3-ha-six
endef

define Package/python3-ha-cryptography/description
cryptography is a package which provides cryptographic recipes and
primitives to Python developers.  Our goal is for it to be your "cryptographic
standard library". It supports Python 2.6-2.7, Python 3.3+, and PyPy 2.6+.
endef

$(eval $(call Py3Package,python3-ha-cryptography))
$(eval $(call BuildPackage,python3-ha-cryptography))
