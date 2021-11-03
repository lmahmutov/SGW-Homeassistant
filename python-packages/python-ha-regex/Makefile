#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-regex
PKG_VERSION:=2021.8.28
PKG_RELEASE:=1

PYPI_NAME:=regex
PKG_HASH:=f585cbbeecb35f35609edccb95efd95a3e35824cd7752b586503f7e6087303f1

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_LICENSE:=Apache-2.0
PKG_LICENSE_FILES:=LICENSE

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-regex
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=Alternative regular expression module, to replace re.
  URL:=https://pypi.org/project/regex/
  DEPENDS:= +python3-light
endef

define Package/python3-ha-regex/description
  This regex implementation is backwards-compatible with the standard ‘re’ module, but offers additional functionality.
endef

$(eval $(call Py3Package,python3-ha-regex))
$(eval $(call BuildPackage,python3-ha-regex))
