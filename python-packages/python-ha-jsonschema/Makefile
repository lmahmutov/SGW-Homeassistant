#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-jsonschema
PKG_VERSION:=3.2.0
PKG_RELEASE:=5

PYPI_NAME:=jsonschema
PKG_HASH:=c8a85b28d377cc7737e46e2d9f2b4f44ee3c0e1deac6bf46ddefc7187d30797a

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_LICENSE:=MIT
PKG_LICENSE_FILES:=COPYING

HOST_PYTHON3_PACKAGE_BUILD_DEPENDS:=setuptools-scm

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-jsonschema
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=An implementation of JSON Schema validation
  URL:=https://github.com/Julian/jsonschema
  DEPENDS:= \
	+python3-light \
	+python3-ha-attrs \
	+python3-urllib \
	+python3-ha-six \
	+python3-ha-pyrsistent \
	+python3-setuptools
endef

define Package/python3-ha-jsonschema/description
  jsonschema is an implementation of JSON Schema validation for Python.
endef

$(eval $(call Py3Package,python3-ha-jsonschema))
$(eval $(call BuildPackage,python3-ha-jsonschema))
