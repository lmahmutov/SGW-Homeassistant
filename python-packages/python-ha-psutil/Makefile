#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-psutil
PKG_VERSION:=5.8.0
PKG_RELEASE:=1a

PYPI_NAME:=psutil
PKG_HASH:=0c9ccb99ab76025f2f0bbecf341d4656e9c1351db8cc8a03ccd62e318ab4b5c6

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_LICENSE:=BSD 3-Clause
PKG_LICENSE_FILES:=LICENSE

HOST_PYTHON3_PACKAGE_BUILD_DEPENDS:=setuptools-scm

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-psutil
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=psutil (process and system utilities)
  URL:=https://github.com/giampaolo/psutil
  DEPENDS:=+python3
endef

define Package/python3-ha-psutil/description
  psutil is a cross-platform library for retrieving information
  on running processes and system utilization.
endef

$(eval $(call Py3Package,python3-ha-psutil))
$(eval $(call BuildPackage,python3-ha-psutil))
