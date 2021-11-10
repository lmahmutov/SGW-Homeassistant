#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-pre-commit
PKG_VERSION:=2.15.0
PKG_RELEASE:=1

PYPI_NAME:=pre_commit
PKG_HASH:=3c25add78dbdfb6a28a651780d5c311ac40dd17f160eb3954a0c59da40a505a7

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_LICENSE:=MIT
PKG_LICENSE_FILES:=LICENSE

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-pre-commit
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=A framework for managing and maintaining multi-language pre-commit hooks.
  URL:=https://pypi.org/project/pre-commit/
  DEPENDS:= +python3-light
endef

define Package/python3-ha-pre-commit/description
 Framework for managing and maintaining multi-language pre-commit hooks.
endef

$(eval $(call Py3Package,python3-ha-pre-commit))
$(eval $(call BuildPackage,python3-ha-pre-commit))
