How to build Mobule for Platform
- It is only for modules are needed to using Android build system.
- Please check its own install information under its folder for other module.

[Step to build]
1. Get android open source.
    : version info - Android 5.0
    ( Download site : http://source.android.com )

2. Copy module that you want to build - to original android open source
   If same module exist in android open source, you should replace it. (no overwrite)
   
  # It is possible to build all modules at once.
  
3. You should add module name to 'PRODUCT_PACKAGES' in 'build\target\product\core.mk' as following case.
                  
ex.) [build\target\product\core.mk] - add below module name
# e2fsprog
PRODUCT_PACKAGES += \
    e2fsck \
    blkid \
    resize2fs

# libexifa, libjpega
PRODUCT_PACKAGES += \
    libexif \
    libexifa \
    libjpega \

# junit
PRODUCT_PACKAGES += \
    core-junit \

# KeyUtils
PRODUCT_PACKAGES += \
    libkeyutils

# brctl
PRODUCT_PACKAGES += \
    brctl 
    
# ebtables
PRODUCT_PACKAGES += \
    ebtables \
    ethertypes

4. Note : 
 You can download the Sbrowser source code from the site below: http://opensource.samsung.com.
 SBrowser Version : 3.0.38
    
