#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-cffi
PKG_VERSION:=1.15.0
PKG_RELEASE:=1

PYPI_NAME:=cffi
PKG_HASH:=920f0d66a896c2d99f0adbb391f990a84091179542c205fa53ce5787aff87954

PKG_LICENSE:=MIT
PKG_LICENSE_FILES:=LICENSE
PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-cffi
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=C Foreign Function Interface
  URL:=https://cffi.readthedocs.org/
  DEPENDS:= \
      +libffi \
      +python3-light \
      +python3-ha-pycparser
endef

define Package/python3-ha-cffi/description
Foreign Function Interface for Python calling C code.
endef

$(eval $(call Py3Package,python3-ha-cffi))
$(eval $(call BuildPackage,python3-ha-cffi))
