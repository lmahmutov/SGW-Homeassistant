#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-docutils
PKG_VERSION:=0.14
PKG_RELEASE:=2

PYPI_NAME:=docutils
PKG_HASH:=51e64ef2ebfb29cae1faa133b3710143496eca21c530f3f71424d77687764274

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_LICENSE:=MIT

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-docutils
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=docutils
  URL:=http://docutils.sourceforge.net
  DEPENDS:=+python3
endef

define Package/python3-ha-docutils/description
Docutils is a modular system for processing documentation into useful formats,
such as HTML, XML, and LaTeX. For input Docutils supports reStructuredText,
an easy-to-read, what-you-see-is-what-you-get plaintext markup syntax.
endef

PYTHON3_PKG_SETUP_ARGS:=

$(eval $(call Py3Package,python3-ha-docutils))
$(eval $(call BuildPackage,python3-ha-docutils))
