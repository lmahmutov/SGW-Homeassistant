#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-typing-extensions
PKG_VERSION:=3.10.0.2
PKG_RELEASE:=1

PYPI_NAME:=typing-extensions
PYPI_SOURCE_NAME:=typing_extensions
PKG_HASH:=49f75d16ff11f1cd258e1b988ccff82a3ca5570217d7ad8c5f48205dd99a677e

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_LICENSE:=PSF-2.0
PKG_LICENSE_FILES:=LICENSE

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-typing-extensions
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=Module with type hints for Python
  URL:=https://github.com/python/typing
  DEPENDS:= \
	+python3-light
endef

define Package/python3-ha-typing-extensions/description
  Backported and Experimental Type Hints for Python.
endef

$(eval $(call Py3Package,python3-ha-typing-extensions))
$(eval $(call BuildPackage,python3-ha-typing-extensions))
