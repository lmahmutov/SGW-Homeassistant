#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-gitpython
PKG_VERSION:=3.1.24
PKG_RELEASE:=1

PYPI_NAME:=GitPython
PKG_HASH:=df83fdf5e684fef7c6ee2c02fc68a5ceb7e7e759d08b694088d0cacb4eba59e5

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_LICENSE:=MIT
PKG_LICENSE_FILES:=LICENSE

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-gitpython
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:= library used to interact with Git
  URL:=https://pypi.org/project/GitPython/
  DEPENDS:=+python3-light \
	+python3-ha-gitdb
endef

define Package/python3-ha-gitpython/description
  GitPython is a python library used to interact with Git repositories.
endef

$(eval $(call Py3Package,python3-ha-gitpython))
$(eval $(call BuildPackage,python3-ha-gitpython))
