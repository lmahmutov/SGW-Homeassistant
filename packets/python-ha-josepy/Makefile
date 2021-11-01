#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-josepy
PKG_VERSION:=1.4.0
PKG_RELEASE:=1

PYPI_NAME:=josepy
PKG_HASH:=c37ff4b93606e6a452b72cdb992da5e0544be12912fac01b31ddbdd61f6d5bd0

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_LICENSE:=Apache-2.0
PKG_LICENSE_FILES:=LICENSE

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-josepy
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=JOSE protocol implementation in Python.
  URL:=https://pypi.org/project/josepy/
  DEPENDS:= \
	+python3-ha-cryptography \
	+python3-ha-pyopenssl \
	+python3-setuptools \
	+python3-ha-six
endef

define Package/python3-ha-josepy/description
 JOSE protocol implementation in Python using cryptography.
endef

$(eval $(call Py3Package,python3-ha-josepy))
$(eval $(call BuildPackage,python3-ha-josepy))
