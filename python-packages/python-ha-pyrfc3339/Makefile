#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-pyrfc3339
PKG_VERSION:=1.1
PKG_RELEASE:=1

PYPI_NAME:=pyRFC3339
PKG_HASH:=81b8cbe1519cdb79bed04910dd6fa4e181faf8c88dff1e1b987b5f7ab23a5b1a

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_LICENSE:=Apache-2.0
PKG_LICENSE_FILES:=LICENSE

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-pyrfc3339
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=Generate and parse RFC 3339 timestamps.
  URL:=https://pypi.org/project/pyRFC3339/
  DEPENDS:=+python3-ha-pytz
endef

define Package/python3-ha-pyrfc3339/description
  pyRFC3339 parses and generates RFC 3339-compliant timestamps using Python datetime.datetime objects.
endef

$(eval $(call Py3Package,python3-ha-pyrfc3339))
$(eval $(call BuildPackage,python3-ha-pyrfc3339))
