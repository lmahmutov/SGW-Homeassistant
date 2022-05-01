#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-pypng
PKG_VERSION:=0.0.20
PKG_RELEASE:=1

PYPI_NAME:=pypng
PKG_HASH:=1032833440c91bafee38a42c38c02d00431b24c42927feb3e63b104d8550170b

PKG_LICENSE:=MIT
PKG_LICENSE_FILES:=LICENSE
PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

PYTHON3_PKG_SETUP_ARGS:=

define Package/python3-ha-pypng
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=Pure Python PNG image encoder/decoder
  URL:=https://github.com/drj11/pypng
  DEPENDS:=+python3-light
endef

define Package/python3-ha-pypng/description
  PyPNG allows PNG image files to be read and written using pure Python.
endef

$(eval $(call Py3Package,python3-ha-pypng))
$(eval $(call BuildPackage,python3-ha-pypng))
