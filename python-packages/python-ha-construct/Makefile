#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-construct
PKG_VERSION:=2.10.67
PKG_RELEASE:=1

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_LICENSE:=MIT
PKG_LICENSE_FILES:=LICENSE.txt

PYPI_NAME:=construct
PKG_HASH:=730235fedf4f2fee5cfadda1d14b83ef1bf23790fb1cc579073e10f70a050883

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-construct
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=symmetric parser/builder for binary data
  URL:=https://pypi.org/project/construct/
  DEPENDS:=+python3-light
endef

define Package/python3-ha-construct/description
 A powerful declarative symmetric parser/builder for binary data.
endef

$(eval $(call Py3Package,python3-ha-construct))
$(eval $(call BuildPackage,python3-ha-construct))
