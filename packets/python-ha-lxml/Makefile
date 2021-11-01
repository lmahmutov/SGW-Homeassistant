#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-lxml
PKG_VERSION:=4.6.3
PKG_RELEASE:=1

PYPI_NAME:=lxml
PKG_HASH:=39b78571b3b30645ac77b95f7c69d1bffc4cf8c3b157c435a34da72e78c82468

PKG_LICENSE:=BSD-3-Clause
PKG_LICENSE_FILES:=LICENSES.txt
PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_CPE_ID:=cpe:/a:lxml:lxml

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-lxml
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=Pythonic XML processing library
  URL:=https://lxml.de
  DEPENDS:=+libxml2 +libxslt +libexslt +python3-light
endef

define Package/python3-ha-lxml/description
  lxml is a Pythonic, mature binding for the libxml2 and libxslt
  libraries. It provides safe and convenient access to these libraries
  using the ElementTree API.

  It extends the ElementTree API significantly to offer support for
  XPath, RelaxNG, XML Schema, XSLT, C14N and much more.
endef

$(eval $(call Py3Package,python3-ha-lxml))
$(eval $(call BuildPackage,python3-ha-lxml))
