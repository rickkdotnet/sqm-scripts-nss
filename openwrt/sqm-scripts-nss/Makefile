include $(TOPDIR)/rules.mk
 
PKG_NAME:=sqm-scripts-nss
PKG_VERSION:=20230217a
PKG_RELEASE:=2
 
include $(INCLUDE_DIR)/package.mk
 
define Package/sqm-scripts-nss
  TITLE:=SQM scripts for NSS enabled builds
  DEPENDS:=+sqm-scripts
  PKGARCH:=all
  SECTION:=base
endef
 
define Package/sqm-scripts-nss/description
  Smart Queue Management Scripts for OpenWRT for use with NSS enabled builds.
endef
 
define Build/Configure
endef

define Build/Compile
endef

define Build/Prepare
	mkdir -p $(PKG_BUILD_DIR)
	$(CP) $(CURDIR)/../../src/ $(PKG_BUILD_DIR)
endef

define Package/sqm-scripts-nss/install
        $(INSTALL_DIR) $(1)
				$(CP) $(PKG_BUILD_DIR)/src/* $(1)/
endef
 
$(eval $(call BuildPackage,sqm-scripts-nss))
