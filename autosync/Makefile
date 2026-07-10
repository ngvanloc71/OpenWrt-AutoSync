include $(TOPDIR)/rules.mk

PKG_NAME:=autosync
PKG_VERSION:=0.1.0
PKG_RELEASE:=1

include $(INCLUDE_DIR)/package.mk

define Package/autosync
  SECTION:=utils
  CATEGORY:=Utilities
  TITLE:=OpenWrt AutoSync
  DEPENDS:=+lsyncd +rsync +inotify-tools
endef

define Package/autosync/install
    $(CP) ./files/* $(1)/
endef

$(eval $(call BuildPackage,autosync))
