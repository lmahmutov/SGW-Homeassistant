#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-acme
PKG_VERSION:=1.18.0
PKG_RELEASE:=1

PYPI_NAME:=acme
PKG_HASH:=9ae06031bbcc492d4ea20aec36bb2ead08b40ccb70d980ade8ecfe8a15d762af

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_LICENSE:=Apache-2.0 MIT
PKG_LICENSE_FILES:=LICENSE

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-acme
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=ACME in Python.
  URL:=https://pypi.org/project/acme/
  DEPENDS:= \
	+python3-ha-cryptography \
	+python3-ha-josepy \
	+python3-ha-pyopenssl \
	+python3-ha-pyrfc3339 \
	+python3-ha-pytz \
	+python3-ha-requests-toolbelt \
	+python3-ha-requests \
	+python3-setuptools \
	+python3-ha-six	
endef

define Package/python3-ha-acme/description
  ACME protocol implementation in Python.
endef

$(eval $(call Py3Package,python3-ha-acme))
$(eval $(call BuildPackage,python3-ha-acme))
