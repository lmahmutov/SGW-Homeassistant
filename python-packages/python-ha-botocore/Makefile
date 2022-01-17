#
# Copyright (C) 2021 @lmahmutov (https://smartgateway.ru/)
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=python-ha-botocore
PKG_VERSION:=1.19.63
PKG_RELEASE:=2

PYPI_NAME:=botocore
PKG_HASH:=d3694f6ef918def8082513e5ef309cd6cd83b612e9984e3a66e8adc98c650a92

PKG_MAINTAINER:=Lenar Mahmutov <lenz1986@gmail.com>
PKG_LICENSE:=MIT

include $(TOPDIR)/feeds/packages/lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include $(TOPDIR)/feeds/packages/lang/python/python3-package.mk

define Package/python3-ha-botocore
  CATEGORY:=Homeassistant
  SUBMENU:=Python packages
  TITLE:=botocore
  URL:=https://github.com/boto/botocore
  DEPENDS:=+python3 \
	+python3-ha-urllib3 \
	+python3-ha-docutils \
	+python3-ha-dateutil \
	+python3-ha-jmespath \
	+python3-ha-requests
endef

define Package/python3-ha-botocore/description
A low-level interface to a growing number of Amazon Web Services.
The botocore package is the foundation for the AWS CLI as well as boto3.
endef

define Build/Prepare
	$(call Build/Prepare/Default)
	# Remove data folder
	cd $(PKG_BUILD_DIR)/botocore/ && rm -rf data && mkdir data
endef


$(eval $(call Py3Package,python3-ha-botocore))
$(eval $(call BuildPackage,python3-ha-botocore))
