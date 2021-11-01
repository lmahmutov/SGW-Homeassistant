#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-yaml
PKG_VERSION:=5.4.1
PKG_RELEASE:=1

PYPI_NAME:=PyYAML
PKG_HASH:=607774cbba28732bfa802b54baa7484215f530991055bb562efbed5b2f20a45e

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_LICENSE:=MIT
PKG_LICENSE_FILES:=LICENSE
PKG_CPE_ID:=cpe:/a:pyyaml_project:pyyaml

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-yaml
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=(HA CORE) YAML parser and emitter for Python
  URL:=https://github.com/yaml/pyyaml
  DEPENDS:=+libyaml +python3-light
endef

define Package/python3-ha-yaml/description
  PyYAML is a YAML parser and emitter for the Python programming language.
endef

PYTHON3_PKG_SETUP_GLOBAL_ARGS:=
PYTHON3_PKG_SETUP_ARGS:=

$(eval $(call Py3Package,python3-ha-yaml))
$(eval $(call BuildPackage,python3-ha-yaml))

