#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-pycognito
PKG_VERSION:=2021.3.1
PKG_RELEASE:=1

PYPI_NAME:=pycognito
PKG_HASH:=3a496364b697d744b37187d0ca3d950abc7540653455240477e4a41c3ba887a1

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_LICENSE:=MIT
PKG_LICENSE_FILES:=LICENSE

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-pycognito
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=AWS Cognito for Python developers.
  URL:=https://pypi.org/project/pycognito/
  DEPENDS:= \
	+python3-ha-boto3 \
	+python3-ha-envs \
	+python3-ha-jose \
	+python3-ha-requests
endef

define Package/python3-ha-pycognito/description
 Python class to integrate Boto3's Cognito client so it is easy to login users.
 With SRP support.
endef

$(eval $(call Py3Package,python3-ha-pycognito))
$(eval $(call BuildPackage,python3-ha-pycognito))