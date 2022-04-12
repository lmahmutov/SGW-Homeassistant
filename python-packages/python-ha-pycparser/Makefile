#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-pycparser
PKG_VERSION:=2.21
PKG_RELEASE:=1

PYPI_NAME:=pycparser
PKG_HASH:=e644fdec12f7872f86c58ff790da456218b10f863970249516d60a5eaca77206

PKG_LICENSE:=BSD-3-Clause
PKG_LICENSE_FILES:=LICENSE
PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>

HOST_PYTHON3_PACKAGE_BUILD_DEPENDS:=ply  # ply==3.10

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-pycparser
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=C parser in Python
  URL:=https://github.com/eliben/pycparser
  DEPENDS:= \
      +python3-light \
      +python3-ha-ply
endef

define Package/python3-ha-pycparser/description
pycparser is a parser for the C language, written in pure Python. It is a
module designed to be easily integrated into applications that need to parse
C source code.
endef

$(eval $(call Py3Package,python3-ha-pycparser))
$(eval $(call BuildPackage,python3-ha-pycparser))
