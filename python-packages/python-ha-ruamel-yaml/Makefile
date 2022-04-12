#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=ha-ruamel-yaml
PKG_VERSION:=0.17.17
PKG_RELEASE:=1

PYPI_NAME:=ruamel.yaml
PKG_HASH:=9751de4cbb57d4bfbf8fc394e125ed4a2f170fbff3dc3d78abf50be85924f8be

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_LICENSE:=MIT
PKG_LICENSE_FILES:=LICENSE

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-ruamel-yaml
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=YAML 1.2 loader/dumper package for Python
  URL:=https://bitbucket.org/ruamel/yaml
  DEPENDS:= \
      +python3-light
endef

define Package/python3-ha-ruamel-yaml/description
ruamel-yaml is a YAML parser/emitter that supports roundtrip preservation of comments, seq/map flow style, and map key order
endef

$(eval $(call Py3Package,python3-ha-ruamel-yaml))
$(eval $(call BuildPackage,python3-ha-ruamel-yaml))
