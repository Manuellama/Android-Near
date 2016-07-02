# Android-Near

<?xml version="1.0" encoding="UTF-8"?>
<manifest>
  <remote  name="aosp"
           fetch=".." />
  <default revision="refs/tags/android-n-preview-4"
           remote="aosp"
           sync-j="4" />
  <project path="build" name="platform/build" groups="pdk,tradefed" >
    <copyfile src="core/root.mk" dest="Makefile" />
  </project>
  <project path="build/blueprint" name="platform/build/blueprint" groups="pdk,tradefed" />
  <project path="build/kati" name="platform/build/kati" groups="pdk,tradefed" />
  <project path="build/soong" name="platform/build/soong" groups="pdk,tradefed" >
    <linkfile src="root.bp" dest="Android.bp" />
    <linkfile src="bootstrap.bash" dest="bootstrap.bash" />
  </project>
  <project path="art" name="platform/art" groups="pdk" />
  <project path="bionic" name="platform/bionic" groups="pdk" />
  <project path="bootable/recovery" name="platform/bootable/recovery" groups="pdk" />
  <project path="cts" name="platform/cts" groups="cts,pdk-cw-fs,pdk-fs" />
  <project path="dalvik" name="platform/dalvik" groups="pdk-cw-fs,pdk-fs" />
  <project path="developers/build" name="platform/developers/build" />
  <project path="developers/demos" name="platform/developers/demos" />
  <project path="developers/samples/android" name="platform/developers/samples/android" />
  <project path="development" name="platform/development" groups="pdk-cw-fs,pdk-fs" />
  <project path="device/asus/deb" name="device/asus/deb" groups="device,flo" />
  <project path="device/asus/flo" name="device/asus/flo" groups="device,flo" />
  <project path="device/asus/flo-kernel" name="device/asus/flo-kernel" groups="device,flo" />
  <project path="device/asus/fugu" name="device/asus/fugu" groups="device,fugu,broadcom_pdk" />
  <project path="device/asus/fugu-kernel" name="device/asus/fugu-kernel" groups="device,fugu,broadcom_pdk" />
  <project path="device/common" name="device/common" groups="pdk-cw-fs,pdk-fs" />
  <project path="device/generic/arm64" name="device/generic/arm64" groups="pdk" />
  <project path="device/generic/armv7-a-neon" name="device/generic/armv7-a-neon" groups="pdk" />
  <project path="device/generic/common" name="device/generic/common" groups="pdk" />
  <project path="device/generic/goldfish" name="device/generic/goldfish" groups="pdk" />
  <project path="device/generic/mips" name="device/generic/mips" groups="pdk" />
  <project path="device/generic/mini-emulator-arm64" name="device/generic/mini-emulator-arm64" groups="pdk" />
  <project path="device/generic/mini-emulator-armv7-a-neon" name="device/generic/mini-emulator-armv7-a-neon" groups="pdk" />
  <project path="device/generic/mini-emulator-mips" name="device/generic/mini-emulator-mips" groups="pdk" />
  <project path="device/generic/mini-emulator-x86" name="device/generic/mini-emulator-x86" groups="pdk" />
  <project path="device/generic/mini-emulator-x86_64" name="device/generic/mini-emulator-x86_64" groups="pdk" />
  <project path="device/generic/qemu" name="device/generic/qemu" />
  <project path="device/generic/x86" name="device/generic/x86" groups="pdk" />
  <project path="device/generic/x86_64" name="device/generic/x86_64" groups="pdk" />
  <project path="device/google/accessory/arduino" name="device/google/accessory/arduino" groups="device" />
  <project path="device/google/accessory/demokit" name="device/google/accessory/demokit" groups="device" />
  <project path="device/google/atv" name="device/google/atv" groups="device,fugu,broadcom_pdk,generic_fs" />
  <project path="device/google/contexthub" name="device/google/contexthub" groups="device" />
  <project path="device/htc/flounder" name="device/htc/flounder" groups="device,flounder,broadcom_pdk" />
  <project path="device/htc/flounder-kernel" name="device/htc/flounder-kernel" groups="device,flounder,broadcom_pdk" />
  <project path="device/huawei/angler" name="device/huawei/angler" groups="device,angler,broadcom_pdk" />
  <project path="device/huawei/angler-kernel" name="device/huawei/angler-kernel" groups="device,angler,broadcom_pdk" />
  <project path="device/lge/bullhead" name="device/lge/bullhead" groups="device,bullhead" />
  <project path="device/lge/bullhead-kernel" name="device/lge/bullhead-kernel" groups="device,bullhead" />
  <project path="device/lge/hammerhead" name="device/lge/hammerhead" groups="device,hammerhead,broadcom_pdk,generic_fs" />
  <project path="device/lge/hammerhead-kernel" name="device/lge/hammerhead-kernel" groups="device,hammerhead,broadcom_pdk,generic_fs" />
  <project path="device/linaro/hikey" name="device/linaro/hikey" />
  <project path="device/linaro/hikey-kernel" name="device/linaro/hikey-kernel" clone-depth="1" />
  <project path="device/moto/shamu" name="device/moto/shamu" groups="device,shamu,broadcom_pdk" />
  <project path="device/moto/shamu-kernel" name="device/moto/shamu-kernel" groups="device,shamu,broadcom_pdk" />
  <project path="device/sample" name="device/sample" groups="pdk" />
  <project path="docs/source.android.com" name="platform/docs/source.android.com" groups="pdk-cw-fs,pdk-fs" />
  <project path="external/aac" name="platform/external/aac" groups="pdk" />
  <project path="external/adt-infra" name="platform/external/adt-infra" groups="adt-infra,notdefault" />
  <project path="external/android-clat" name="platform/external/android-clat" groups="pdk-cw-fs,pdk-fs" />
  <project path="external/android-mock" name="platform/external/android-mock" groups="pdk-cw-fs,pdk-fs" />
  <project path="external/androidplot" name="platform/external/androidplot" groups="pdk-cw-fs,pdk-fs" />
  <project path="external/ant-glob" name="platform/external/ant-glob" groups="pdk-cw-fs,pdk-fs" />
  <project path="external/antlr" name="platform/external/antlr" groups="pdk-cw-fs,pdk-fs" />
  <project path="external/apache-commons-math" name="platform/external/apache-commons-math" groups="pdk-cw-fs,pdk-fs" />
  <project path="external/apache-harmony" name="platform/external/apache-harmony" groups="pdk-cw-fs,pdk-fs" />
  <project path="external/apache-http" name="platform/external/apache-http" groups="pdk" />
  <project path="external/apache-xml" name="platform/external/apache-xml" groups="pdk" />
  <project path="external/autotest" name="platform/external/autotest" />
  <project path="external/avahi" name="platform/external/avahi" />
  <project path="external/bison" name="platform/external/bison" groups="pdk" />
  <project path="external/blktrace" name="platform/external/blktrace" groups="pdk-cw-fs,pdk-fs" />
  <project path="external/boringssl" name="platform/external/boringssl" groups="pdk" />
  <project path="external/bouncycastle" name="platform/external/bouncycastle" groups="pdk" />
  <project path="external/bsdiff" name="platform/external/bsdiff" groups="pdk" />
  <project path="external/bzip2" name="platform/external/bzip2" groups="pdk" />
  <project path="external/c-ares" name="platform/external/c-ares" />
  <project path="external/caliper" name="platform/external/caliper" />
  <project path="external/cblas" name="platform/external/cblas" groups="pdk" />
  <project path="external/ceres-solver" name="platform/external/ceres-solver" groups="pdk-cw-fs,pdk-fs" />
  <project path="external/chromium-libpac" name="platform/external/chromium-libpac" groups="pdk-fs" />
  <project path="external/chromium-trace" name="platform/external/chromium-trace" groups="pdk" />
  <project path="external/chromium-webview" name="platform/external/chromium-webview" groups="pdk" />
  <project path="external/clang" name="platform/external/clang" groups="pdk" />
  <project path="external/cmockery" name="platform/external/cmockery" groups="pdk-fs" />
  <project path="external/compiler-rt" name="platform/external/compiler-rt" groups="pdk" />
  <project path="external/conscrypt" name="platform/external/conscrypt" groups="pdk-cw-fs,pdk-fs" />
  <project path="external/crcalc" name="platform/external/crcalc" groups="pdk-fs" />
  <project path="external/cros/system_api" name="platform/external/cros/system_api" />
  <project path="external/curl" name="platform/external/curl" />
  <project path="external/dagger2" name="platform/external/dagger2" />
  <project path="external/dbus" name="platform/external/dbus" />
  <project path="external/dbus-binding-generator" name="platform/external/dbus-binding-generator" />
  <project path="external/deqp" name="platform/external/deqp" groups="pdk-fs" />
  <project path="external/dexmaker" name="platform/external/dexmaker" groups="pdk-cw-fs,pdk-fs" />
  <project path="external/dhcpcd" name="platform/external/dhcpcd" groups="pdk-cw-fs,pdk-fs" />
  <project path="external/dhcpcd-6.8.2" name="platform/external/dhcpcd-6.8.2" />
  <project path="external/dlmalloc" name="platform/external/dlmalloc" />
  <project path="external/dng_sdk" name="platform/external/dng_sdk" />
  <project path="external/dnsmasq" name="platform/external/dnsmasq" groups="pdk" />
  <project path="external/doclava" name="platform/external/doclava" groups="pdk-cw-fs,pdk-fs" />
  <project path="external/donuts" name="platform/external/donuts" groups="pdk-fs" />
  <project path="external/drm_gralloc" name="platform/external/drm_gralloc" groups="drm_gralloc" />
  <project path="external/drm_hwcomposer" name="platform/external/drm_hwcomposer" groups="drm_hwcomposer" />
  <project path="external/droiddriver" name="platform/external/droiddriver" groups="pdk-cw-fs,pdk-fs" />
  <project path="external/e2fsprogs" name="platform/external/e2fsprogs" groups="pdk" />
  <project path="external/dtc" name="platform/external/dtc" />
  <project path="external/easymock" name="platform/external/easymock" groups="pdk-cw-fs,pdk-fs" />
  <project path="external/eclipse-basebuilder" name="platform/external/eclipse-basebuilder" groups="pdk-cw-fs,pdk-fs" />
  <project path="external/eclipse-windowbuilder" name="platform/external/eclipse-windowbuilder" groups="pdk-cw-fs,pdk-fs" />
  <project path="external/eigen" name="platform/external/eigen" groups="pdk" />
  <project path="external/elfutils" name="platform/external/elfutils" groups="pdk" />
  <project path="external/embunit" name="platform/external/embunit" groups="pdk-cw-fs,pdk-fs" />
  <project path="external/emma" name="platform/external/emma" groups="pdk-cw-fs,pdk-fs" />
  <project path="external/esd" name="platform/external/esd" groups="pdk-cw-fs,pdk-fs" />
  <project path="external/expat" name="platform/external/expat" groups="pdk" />
  <project path="external/eyes-free" name="platform/external/eyes-free" groups="pdk-cw-fs,pdk-fs" />
  <project path="external/f2fs-tools" name="platform/external/f2fs-tools" groups="pdk" />
  <project path="external/fdlibm" name="platform/external/fdlibm" groups="pdk" />
  <project path="external/fec" name="platform/external/fec" />
  <project path="external/fio" name="platform/external/fio" groups="pdk-fs" />
  <project path="external/flac" name="platform/external/flac" groups="pdk" />
  <project path="external/fonttools" name="platform/external/fonttools" groups="pdk-fs" />
  <project path="external/freetype" name="platform/external/freetype" groups="pdk" />
  <project path="external/fsck_msdos" name="platform/external/fsck_msdos" groups="pdk-cw-fs,pdk-fs" />
  <project path="external/gemmlowp" name="platform/external/gemmlowp" />
  <project path="external/giflib" name="platform/external/giflib" groups="pdk,qcom_msm8x26" />
  <project path="external/glide" name="platform/external/glide" groups="pdk-fs" />
  <project path="external/gmock" name="platform/external/gmock" groups="pdk" />
  <project path="external/google-benchmark" name="platform/external/google-benchmark" groups="pdk" />
  <project path="external/google-breakpad" name="platform/external/google-breakpad" groups="dragon" />
  <project path="external/google-fonts/carrois-gothic-sc" name="platform/external/google-fonts/carrois-gothic-sc" groups="pdk-cw-fs,pdk-fs" />
  <project path="external/google-fonts/coming-soon" name="platform/external/google-fonts/coming-soon" groups="pdk-cw-fs,pdk-fs" />
  <project path="external/google-fonts/cutive-mono" name="platform/external/google-fonts/cutive-mono" groups="pdk-cw-fs,pdk-fs" />
  <project path="external/google-fonts/dancing-script" name="platform/external/google-fonts/dancing-script" groups="pdk-cw-fs,pdk-fs" />
  <project path="external/google-tv-pairing-protocol" name="platform/external/google-tv-pairing-protocol" groups="pdk-fs" />
  <project path="external/gptfdisk" name="platform/external/gptfdisk" groups="pdk-fs" />
  <project path="external/gtest" name="platform/external/gtest" groups="pdk" />
  <project path="external/guava" name="platform/external/guava" groups="pdk-cw-fs,pdk-fs" />
  <project path="external/guice" name="platform/external/guice" groups="pdk" />
  <project path="external/hamcrest" name="platform/external/hamcrest" groups="pdk-cw-fs,pdk-fs" />
  <project path="external/harfbuzz_ng" name="platform/external/harfbuzz_ng" groups="pdk,qcom_msm8x26" />
  <project path="external/hyphenation-patterns" name="platform/external/hyphenation-patterns" groups="pdk-fs" />
  <project path="external/icu" name="platform/external/icu" groups="pdk" />
  <project path="external/iproute2" name="platform/external/iproute2" groups="pdk" />
  <project path="external/ipsec-tools" name="platform/external/ipsec-tools" groups="pdk-cw-fs,pdk-fs" />
  <project path="external/iptables" name="platform/external/iptables" groups="pdk-cw-fs,pdk-fs" />
  <project path="external/iputils" name="platform/external/iputils" groups="pdk-cw-fs,pdk-fs" />
  <project path="external/iw" name="platform/external/iw" />
  <project path="external/jacoco" name="platform/external/jacoco" />
  <project path="external/jarjar" name="platform/external/jarjar" groups="pdk" />
  <project path="external/javasqlite" name="platform/external/javasqlite" groups="pdk-cw-fs,pdk-fs" />
  <project path="external/javassist" name="platform/external/javassist" groups="pdk-cw-fs,pdk-fs" />
  <project path="external/jcommander" name="platform/external/jcommander" groups="pdk" />
  <project path="external/jdiff" name="platform/external/jdiff" groups="pdk-cw-fs,pdk-fs" />
  <project path="external/jemalloc" name="platform/external/jemalloc" groups="pdk" />
  <project path="external/jetty" name="platform/external/jetty" groups="pdk-fs" />
  <project path="external/jhead" name="platform/external/jhead" groups="pdk" />
  <project path="external/jline" name="platform/external/jline" groups="notdefault,tradefed" />
  <project path="external/jmdns" name="platform/external/jmdns" groups="pdk-cw-fs,pdk-fs" />
  <project path="external/jmonkeyengine" name="platform/external/jmonkeyengine" groups="pdk-cw-fs,pdk-fs" />
  <project path="external/jpeg" name="platform/external/jpeg" groups="pdk" />
  <project path="external/jsilver" name="platform/external/jsilver" groups="pdk-cw-fs,pdk-fs" />
  <project path="external/jsmn" name="platform/external/jsmn" groups="pdk" />
  <project path="external/jsoncpp" name="platform/external/jsoncpp" groups="pdk-cw-fs,pdk-fs" />
  <project path="external/jsr305" name="platform/external/jsr305" groups="pdk-cw-fs,pdk-fs" />
  <project path="external/jsr330" name="platform/external/jsr330" groups="pdk" />
  <project path="external/junit" name="platform/external/junit" groups="pdk-cw-fs,pdk-fs" />
  <project path="external/kernel-headers" name="platform/external/kernel-headers" groups="pdk-cw-fs,pdk-fs" />
  <project path="external/ksoap2" name="platform/external/ksoap2" groups="pdk-cw-fs,pdk-fs" />
  <project path="external/libavc" name="platform/external/libavc" groups="pdk" />
  <project path="external/libbrillo" name="platform/external/libbrillo" />
  <project path="external/libcap" name="platform/external/libcap" />
  <project path="external/libcap-ng" name="platform/external/libcap-ng" groups="pdk-cw-fs,pdk-fs" />
  <project path="external/libchrome" name="platform/external/libchrome" />
  <project path="external/libconstrainedcrypto" name="platform/external/libconstrainedcrypto" groups="pdk" />
  <project path="external/libcxx" name="platform/external/libcxx" groups="pdk" />
  <project path="external/libcxxabi" name="platform/external/libcxxabi" groups="pdk" />
  <project path="external/libdivsufsort" name="platform/external/libdivsufsort" groups="pdk" />
  <project path="external/libdrm" name="platform/external/libdrm" groups="pdk" />
  <project path="external/libedit" name="platform/external/libedit" groups="pdk-fs" />
  <project path="external/libdaemon" name="platform/external/libdaemon" />
  <project path="external/libevent" name="platform/external/libevent" />
  <project path="external/libexif" name="platform/external/libexif" groups="pdk-cw-fs,pdk-fs" />
  <project path="external/libgsm" name="platform/external/libgsm" groups="pdk" />
  <project path="external/libhevc" name="platform/external/libhevc" groups="pdk-fs" />
  <project path="external/liblzf" name="platform/external/liblzf" groups="pdk" />
  <project path="external/libmicrohttpd" name="platform/external/libmicrohttpd" />
  <project path="external/libmpeg2" name="platform/external/libmpeg2" groups="pdk" />
  <project path="external/libmojo" name="platform/external/libmojo" />
  <project path="external/libmtp" name="platform/external/libmtp" groups="pdk-cw-fs,pdk-fs" />
  <project path="external/libnfc-nci" name="platform/external/libnfc-nci" groups="pdk" />
  <project path="external/libnfc-nxp" name="platform/external/libnfc-nxp" groups="pdk" />
  <project path="external/libnl" name="platform/external/libnl" groups="pdk" />
  <project path="external/libogg" name="platform/external/libogg" groups="pdk" />
  <project path="external/libopus" name="platform/external/libopus" groups="pdk" />
  <project path="external/libpcap" name="platform/external/libpcap" groups="pdk,pdk-cw-fs,pdk-fs" />
  <project path="external/libphonenumber" name="platform/external/libphonenumber" groups="pdk-cw-fs,pdk-fs" />
  <project path="external/libpng" name="platform/external/libpng" groups="pdk" />
  <project path="external/libselinux" name="platform/external/libselinux" groups="pdk" />
  <project path="external/libunwind" name="platform/external/libunwind" groups="pdk" />
  <project path="external/libunwind_llvm" name="platform/external/libunwind_llvm" />
  <project path="external/libusb" name="platform/external/libusb" groups="pdk-cw-fs,pdk-fs" />
  <project path="external/libusb-compat" name="platform/external/libusb-compat" groups="pdk-cw-fs,pdk-fs" />
  <project path="external/libutf" name="platform/external/libutf" groups="pdk-cw-fs,pdk-fs" />
  <project path="external/libvncserver" name="platform/external/libvncserver" groups="pdk-cw-fs,pdk-fs" />
  <project path="external/libvorbis" name="platform/external/libvorbis" groups="pdk-cw-fs,pdk-fs" />
  <project path="external/libvpx" name="platform/external/libvpx" groups="pdk" />
  <project path="external/libvterm" name="platform/external/libvterm" groups="pdk-cw-fs,pdk-fs" />
  <project path="external/libweave" name="platform/external/libweave" />
  <project path="external/libxml2" name="platform/external/libxml2" groups="pdk-cw-fs,pdk-fs,libxml2" />
  <project path="external/libyuv" name="platform/external/libyuv" groups="libyuv,pdk-cw-fs,pdk-fs" />
  <project path="external/littlemock" name="platform/external/littlemock" groups="pdk-cw-fs,pdk-fs" />
  <project path="external/lld" name="platform/external/lld" groups="pdk-fs" />
  <project path="external/lldb" name="platform/external/lldb" groups="pdk-cw-fs,pdk-fs" />
  <project path="external/llvm" name="platform/external/llvm" groups="pdk" />
  <project path="external/ltrace" name="platform/external/ltrace" groups="pdk-cw-fs,pdk-fs" />
  <project path="external/lz4" name="platform/external/lz4" groups="pdk-cw-fs,pdk-fs" />
  <project path="external/lzma" name="platform/external/lzma" groups="pdk" />
  <project path="external/marisa-trie" name="platform/external/marisa-trie" groups="pdk-cw-fs,pdk-fs" />
  <project path="external/markdown" name="platform/external/markdown" groups="pdk-cw-fs,pdk-fs" />
  <project path="external/mdnsresponder" name="platform/external/mdnsresponder" groups="pdk" />
  <project path="external/mesa3d" name="platform/external/mesa3d" groups="pdk-cw-fs,pdk-fs" />
  <project path="external/messageformat" name="platform/external/messageformat" groups="pdk-cw-fs,pdk-fs" />
  <project path="external/minijail" name="platform/external/minijail" />
  <project path="external/mksh" name="platform/external/mksh" groups="pdk" />
  <project path="external/mmc-utils" name="platform/external/mmc-utils" groups="pdk-cw-fs,pdk-fs" />
  <project path="external/mockftpserver" name="platform/external/mockftpserver" groups="pdk-fs" />
  <project path="external/mockito" name="platform/external/mockito" groups="pdk-cw-fs,pdk-fs" />
  <project path="external/mockwebserver" name="platform/external/mockwebserver" groups="pdk-cw-fs,pdk-fs" />
  <project path="external/modp_b64" name="platform/external/modp_b64" />
  <project path="external/mp4parser" name="platform/external/mp4parser" groups="pdk-cw-fs,pdk-fs" />
  <project path="external/mtpd" name="platform/external/mtpd" groups="pdk-cw-fs,pdk-fs" />
  <project path="external/nanohttpd" name="platform/external/nanohttpd" groups="pdk-fs" />
  <project path="external/nanopb-c" name="platform/external/nanopb-c" groups="pdk" />
  <project path="external/naver-fonts" name="platform/external/naver-fonts" groups="pdk-cw-fs,pdk-fs" />
  <project path="external/netcat" name="platform/external/netcat" groups="pdk-cw-fs,pdk-fs" />
  <project path="external/netperf" name="platform/external/netperf" groups="pdk-cw-fs,pdk-fs" />
  <project path="external/neven" name="platform/external/neven" groups="pdk-cw-fs,pdk-fs" />
  <project path="external/nfacct" name="platform/external/nfacct" groups="pdk-cw-fs,pdk-fs" />
  <project path="external/nist-pkits" name="platform/external/nist-pkits" groups="pdk-cw-fs,pdk-fs" />
  <project path="external/nist-sip" name="platform/external/nist-sip" groups="pdk-cw-fs,pdk-fs" />
  <project path="external/noto-fonts" name="platform/external/noto-fonts" groups="pdk" />
  <project path="external/oauth" name="platform/external/oauth" groups="pdk-cw-fs,pdk-fs" />
  <project path="external/objenesis" name="platform/external/objenesis" groups="pdk-cw-fs,pdk-fs" />
  <project path="external/okhttp" name="platform/external/okhttp" groups="pdk-cw-fs,pdk-fs" />
  <project path="external/opencv" name="platform/external/opencv" groups="pdk-cw-fs,pdk-fs" />
  <project path="external/opencv3" name="platform/external/opencv3" />
  <project path="external/openfst" name="platform/external/openfst" groups="pdk-cw-fs,pdk-fs" />
  <project path="external/openssh" name="platform/external/openssh" groups="pdk-cw-fs,pdk-fs" />
  <project path="external/owasp/sanitizer" name="platform/external/owasp/sanitizer" groups="pdk-fs" />
  <project path="external/parameter-framework" name="platform/external/parameter-framework" groups="pdk-fs" />
  <project path="external/pcre" name="platform/external/pcre" groups="pdk" />
  <project path="external/pdfium" name="platform/external/pdfium" groups="pdk" />
  <project path="external/piex" name="platform/external/piex" />
  <project path="external/ppp" name="platform/external/ppp" groups="pdk-cw-fs,pdk-fs" />
  <project path="external/proguard" name="platform/external/proguard" groups="pdk" />
  <project path="external/protobuf" name="platform/external/protobuf" groups="pdk" />
  <project path="external/regex-re2" name="platform/external/regex-re2" groups="pdk-cw-fs,pdk-fs" />
  <project path="external/replicaisland" name="platform/external/replicaisland" groups="pdk-cw-fs,pdk-fs" />
  <project path="external/rmi4utils" name="platform/external/rmi4utils" />
  <project path="external/robolectric" name="platform/external/robolectric" groups="pdk-cw-fs,pdk-fs" />
  <project path="external/roboto-fonts" name="platform/external/roboto-fonts" groups="pdk-cw-fs,pdk-fs" />
  <project path="external/rootdev" name="platform/external/rootdev" />
  <project path="external/safe-iop" name="platform/external/safe-iop" groups="pdk" />
  <project path="external/scrypt" name="platform/external/scrypt" groups="pdk" />
  <project path="external/selinux" name="platform/external/selinux" groups="pdk" />
  <project path="external/shflags" name="platform/external/shflags" groups="pdk" />
  <project path="external/sfntly" name="platform/external/sfntly" groups="pdk,qcom_msm8x26" />
  <project path="external/skia" name="platform/external/skia" groups="pdk,qcom_msm8x26" />
  <project path="external/sl4a" name="platform/external/sl4a" />
  <project path="external/slf4j" name="platform/external/slf4j" groups="pdk-fs" />
  <project path="external/smali" name="platform/external/smali" groups="pdk-cw-fs,pdk-fs" />
  <project path="external/snakeyaml" name="platform/external/snakeyaml" groups="pdk" />
  <project path="external/sonic" name="platform/external/sonic" groups="pdk" />
  <project path="external/sonivox" name="platform/external/sonivox" groups="pdk" />
  <project path="external/speex" name="platform/external/speex" groups="pdk" />
  <project path="external/sqlite" name="platform/external/sqlite" groups="pdk" />
  <project path="external/squashfs-tools" name="platform/external/squashfs-tools" groups="pdk" />
  <project path="external/srtp" name="platform/external/srtp" groups="pdk-cw-fs,pdk-fs" />
  <project path="external/strace" name="platform/external/strace" groups="pdk-cw-fs,pdk-fs" />
  <project path="external/svox" name="platform/external/svox" groups="pdk-cw-fs,pdk-fs" />
  <project path="external/tagsoup" name="platform/external/tagsoup" groups="pdk-cw-fs,pdk-fs" />
  <project path="external/testng" name="platform/external/testng" groups="pdk" />
  <project path="external/tcpdump" name="platform/external/tcpdump" groups="pdk,pdk-cw-fs,pdk-fs" />
  <project path="external/timezonepicker-support" name="platform/external/timezonepicker-support" groups="pdk-cw-fs,pdk-fs" />
  <project path="external/tinyalsa" name="platform/external/tinyalsa" groups="pdk" />
  <project path="external/tinycompress" name="platform/external/tinycompress" groups="pdk" />
  <project path="external/tinyxml" name="platform/external/tinyxml" groups="pdk" />
  <project path="external/tinyxml2" name="platform/external/tinyxml2" groups="pdk" />
  <project path="external/tlsdate" name="platform/external/tlsdate" />
  <project path="external/toybox" name="platform/external/toybox" groups="pdk" />
  <project path="external/tpm2" name="platform/external/tpm2" />
  <project path="external/tremolo" name="platform/external/tremolo" groups="pdk" />
  <project path="external/v8" name="platform/external/v8" groups="pdk" />
  <project path="external/valgrind" name="platform/external/valgrind" groups="pdk" />
  <project path="external/vboot_reference" name="platform/external/vboot_reference" groups="vboot" />
  <project path="external/vixl" name="platform/external/vixl" groups="pdk" />
  <project path="external/vogar" name="platform/external/vogar" groups="pdk" />
  <project path="external/webp" name="platform/external/webp" groups="pdk,qcom_msm8x26" />
  <project path="external/webrtc" name="platform/external/webrtc" groups="pdk" />
  <project path="external/wpa_supplicant_8" name="platform/external/wpa_supplicant_8" groups="pdk" />
  <project path="external/xmlrpcpp" name="platform/external/xmlrpcpp" groups="pdk" />
  <project path="external/xmlwriter" name="platform/external/xmlwriter" groups="pdk-cw-fs,pdk-fs" />
  <project path="external/xmp_toolkit" name="platform/external/xmp_toolkit" groups="pdk-cw-fs,pdk-fs" />
  <project path="external/zlib" name="platform/external/zlib" groups="pdk" />
  <project path="external/zopfli" name="platform/external/zopfli" groups="pdk-cw-fs,pdk-fs" />
  <project path="external/zxing" name="platform/external/zxing" groups="pdk-cw-fs,pdk-fs" />
  <project path="frameworks/av" name="platform/frameworks/av" groups="pdk" />
  <project path="frameworks/base" name="platform/frameworks/base" groups="pdk-cw-fs,pdk-fs" />
  <project path="frameworks/compile/libbcc" name="platform/frameworks/compile/libbcc" groups="pdk" />
  <project path="frameworks/compile/mclinker" name="platform/frameworks/compile/mclinker" groups="pdk" />
  <project path="frameworks/compile/slang" name="platform/frameworks/compile/slang" groups="pdk" />
  <project path="frameworks/ex" name="platform/frameworks/ex" groups="pdk-cw-fs,pdk-fs" />
  <project path="frameworks/minikin" name="platform/frameworks/minikin" groups="pdk-cw-fs,pdk-fs" />
  <project path="frameworks/ml" name="platform/frameworks/ml" groups="pdk-cw-fs,pdk-fs" />
  <project path="frameworks/multidex" name="platform/frameworks/multidex" groups="pdk-cw-fs,pdk-fs" />
  <project path="frameworks/native" name="platform/frameworks/native" groups="pdk" />
  <project path="frameworks/opt/bitmap" name="platform/frameworks/opt/bitmap" groups="pdk-fs" />
  <project path="frameworks/opt/bluetooth" name="platform/frameworks/opt/bluetooth" groups="pdk-cw-fs,pdk-fs" />
  <project path="frameworks/opt/calendar" name="platform/frameworks/opt/calendar" groups="pdk-cw-fs,pdk-fs" />
  <project path="frameworks/opt/chips" name="platform/frameworks/opt/chips" groups="pdk-cw-fs,pdk-fs" />
  <project path="frameworks/opt/colorpicker" name="platform/frameworks/opt/colorpicker" groups="pdk-cw-fs,pdk-fs" />
  <project path="frameworks/opt/datetimepicker" name="platform/frameworks/opt/datetimepicker" groups="pdk-cw-fs,pdk-fs" />
  <project path="frameworks/opt/emoji" name="platform/frameworks/opt/emoji" groups="pdk-cw-fs,pdk-fs" />
  <project path="frameworks/opt/inputconnectioncommon" name="platform/frameworks/opt/inputconnectioncommon" groups="pdk-fs" />
  <project path="frameworks/opt/inputmethodcommon" name="platform/frameworks/opt/inputmethodcommon" groups="pdk-cw-fs,pdk-fs" />
  <project path="frameworks/opt/net/ethernet" name="platform/frameworks/opt/net/ethernet" groups="pdk-fs" />
  <project path="frameworks/opt/net/ims" name="platform/frameworks/opt/net/ims" groups="frameworks_ims,pdk-cw-fs,pdk-fs" />
  <project path="frameworks/opt/net/voip" name="platform/frameworks/opt/net/voip" groups="pdk-cw-fs,pdk-fs" />
  <project path="frameworks/opt/net/wifi" name="platform/frameworks/opt/net/wifi" groups="pdk" />
  <project path="frameworks/opt/photoviewer" name="platform/frameworks/opt/photoviewer" groups="pdk-cw-fs,pdk-fs" />
  <project path="frameworks/opt/setupwizard" name="platform/frameworks/opt/setupwizard" groups="pdk-cw-fs,pdk-fs" />
  <project path="frameworks/opt/telephony" name="platform/frameworks/opt/telephony" groups="pdk" />
  <project path="frameworks/opt/timezonepicker" name="platform/frameworks/opt/timezonepicker" groups="pdk-cw-fs,pdk-fs" />
  <project path="frameworks/opt/vcard" name="platform/frameworks/opt/vcard" groups="pdk-cw-fs,pdk-fs" />
  <project path="frameworks/rs" name="platform/frameworks/rs" groups="pdk" />
  <project path="frameworks/support" name="platform/frameworks/support" groups="pdk-cw-fs,pdk-fs" />
  <project path="frameworks/data-binding" name="platform/frameworks/data-binding" groups="pdk-cw-fs,pdk-fs" />
  <project path="frameworks/volley" name="platform/frameworks/volley" groups="pdk-cw-fs,pdk-fs" />
  <project path="frameworks/webview" name="platform/frameworks/webview" groups="pdk-cw-fs,pdk-fs" />
  <project path="frameworks/wilhelm" name="platform/frameworks/wilhelm" groups="pdk-cw-fs,pdk-fs" />
  <project path="hardware/akm" name="platform/hardware/akm" />
  <project path="hardware/broadcom/libbt" name="platform/hardware/broadcom/libbt" groups="pdk" />
  <project path="hardware/broadcom/wlan" name="platform/hardware/broadcom/wlan" groups="pdk,broadcom_wlan" />
  <project path="hardware/intel/audio_media" name="platform/hardware/intel/audio_media" groups="intel" />
  <project path="hardware/intel/bootstub" name="platform/hardware/intel/bootstub" groups="intel" />
  <project path="hardware/intel/common/bd_prov" name="platform/hardware/intel/common/bd_prov" groups="intel" />
  <project path="hardware/intel/common/libmix" name="platform/hardware/intel/common/libmix" groups="intel" />
  <project path="hardware/intel/common/libstagefrighthw" name="platform/hardware/intel/common/libstagefrighthw" groups="intel" />
  <project path="hardware/intel/common/libva" name="platform/hardware/intel/common/libva" groups="intel" />
  <project path="hardware/intel/common/libwsbm" name="platform/hardware/intel/common/libwsbm" groups="intel" />
  <project path="hardware/intel/common/omx-components" name="platform/hardware/intel/common/omx-components" groups="intel" />
  <project path="hardware/intel/common/utils" name="platform/hardware/intel/common/utils" groups="intel" />
  <project path="hardware/intel/common/wrs_omxil_core" name="platform/hardware/intel/common/wrs_omxil_core" groups="intel" />
  <project path="hardware/intel/img/hwcomposer" name="platform/hardware/intel/img/hwcomposer" groups="intel" />
  <project path="hardware/intel/img/psb_headers" name="platform/hardware/intel/img/psb_headers" groups="intel" />
  <project path="hardware/intel/img/psb_video" name="platform/hardware/intel/img/psb_video" groups="intel" />
  <project path="hardware/intel/sensors" name="platform/hardware/intel/sensors" groups="intel_sensors" />
  <project path="hardware/invensense" name="platform/hardware/invensense" groups="invensense" />
  <project path="hardware/libhardware" name="platform/hardware/libhardware" groups="pdk" />
  <project path="hardware/libhardware_legacy" name="platform/hardware/libhardware_legacy" groups="pdk" />
  <project path="hardware/marvell/bt" name="platform/hardware/marvell/bt" groups="marvell_bt" />
  <project path="hardware/mediatek" name="platform/hardware/mediatek" groups="mediatek,mediatek_wear" />
  <project path="hardware/qcom/audio" name="platform/hardware/qcom/audio" groups="qcom,qcom_audio" />
  <project path="hardware/qcom/bt" name="platform/hardware/qcom/bt" groups="qcom" />
  <project path="hardware/qcom/camera" name="platform/hardware/qcom/camera" groups="qcom" />
  <project path="hardware/qcom/display" name="platform/hardware/qcom/display" groups="pdk,qcom,qcom_display" />
  <project path="hardware/qcom/gps" name="platform/hardware/qcom/gps" groups="qcom,qcom_gps" />
  <project path="hardware/qcom/keymaster" name="platform/hardware/qcom/keymaster" groups="qcom,qcom_keymaster" />
  <project path="hardware/qcom/media" name="platform/hardware/qcom/media" groups="qcom" />
  <project path="hardware/qcom/msm8960" name="platform/hardware/qcom/msm8960" groups="qcom_msm8960" />
  <project path="hardware/qcom/msm8994" name="platform/hardware/qcom/msm8994" groups="qcom_msm8994" />
  <project path="hardware/qcom/msm8x26" name="platform/hardware/qcom/msm8x26" groups="qcom_msm8x26" />
  <project path="hardware/qcom/msm8x27" name="platform/hardware/qcom/msm8x27" groups="qcom_msm8x27" />
  <project path="hardware/qcom/msm8x74" name="platform/hardware/qcom/msm8x74" groups="pdk,qcom_msm8x74" />
  <project path="hardware/qcom/msm8x84" name="platform/hardware/qcom/msm8x84" groups="qcom_msm8x84" />
  <project path="hardware/qcom/power" name="platform/hardware/qcom/power" groups="qcom" />
  <project path="hardware/qcom/wlan" name="platform/hardware/qcom/wlan" groups="qcom_wlan" />
  <project path="hardware/ril" name="platform/hardware/ril" groups="pdk" />
  <project path="hardware/ti/omap3" name="platform/hardware/ti/omap3" groups="omap3" />
  <project path="hardware/ti/omap4-aah" name="platform/hardware/ti/omap4-aah" groups="omap4-aah" />
  <project path="hardware/ti/omap4xxx" name="platform/hardware/ti/omap4xxx" groups="omap4" />
  <project path="kernel/tests" name="kernel/tests" />
  <project path="libcore" name="platform/libcore" groups="pdk" />
  <project path="libnativehelper" name="platform/libnativehelper" groups="pdk" />
  <project path="ndk" name="platform/ndk" groups="generic_fs" />
  <project path="packages/apps/BasicSmsReceiver" name="platform/packages/apps/BasicSmsReceiver" groups="pdk-cw-fs,pdk-fs" />
  <project path="packages/apps/Bluetooth" name="platform/packages/apps/Bluetooth" groups="pdk-cw-fs,pdk-fs" />
  <project path="packages/apps/Browser2" name="platform/packages/apps/Browser2" />
  <project path="packages/apps/Calculator" name="platform/packages/apps/Calculator" groups="pdk-fs" />
  <project path="packages/apps/Calendar" name="platform/packages/apps/Calendar" groups="pdk-fs" />
  <project path="packages/apps/Camera" name="platform/packages/apps/Camera" groups="pdk-fs" />
  <project path="packages/apps/Camera2" name="platform/packages/apps/Camera2" groups="pdk-fs" />
  <project path="packages/apps/CarrierConfig" name="platform/packages/apps/CarrierConfig" groups="pdk-fs" />
  <project path="packages/apps/CellBroadcastReceiver" name="platform/packages/apps/CellBroadcastReceiver" groups="pdk-fs" />
  <project path="packages/apps/CertInstaller" name="platform/packages/apps/CertInstaller" groups="pdk-cw-fs,pdk-fs" />
  <project path="packages/apps/Contacts" name="platform/packages/apps/Contacts" groups="pdk-fs" />
  <project path="packages/apps/ContactsCommon" name="platform/packages/apps/ContactsCommon" groups="pdk-fs"/>
  <project path="packages/apps/DeskClock" name="platform/packages/apps/DeskClock" groups="pdk-fs" />
  <project path="packages/apps/Dialer" name="platform/packages/apps/Dialer" groups="pdk-fs" />
  <project path="packages/apps/Email" name="platform/packages/apps/Email" groups="pdk-fs" />
  <project path="packages/apps/EmergencyInfo" name="platform/packages/apps/EmergencyInfo" />
  <project path="packages/apps/ExactCalculator" name="platform/packages/apps/ExactCalculator" groups="pdk-fs" />
  <project path="packages/apps/FMRadio" name="platform/packages/apps/FMRadio" groups="pdk-fs" />
  <project path="packages/apps/Gallery" name="platform/packages/apps/Gallery" groups="pdk-fs" />
  <project path="packages/apps/Gallery2" name="platform/packages/apps/Gallery2" groups="pdk-fs" />
  <project path="packages/apps/HTMLViewer" name="platform/packages/apps/HTMLViewer" groups="pdk-fs" />
  <project path="packages/apps/InCallUI" name="platform/packages/apps/InCallUI" groups="pdk-fs" />
  <project path="packages/apps/KeyChain" name="platform/packages/apps/KeyChain" groups="pdk-fs" />
  <project path="packages/apps/Launcher2" name="platform/packages/apps/Launcher2" groups="pdk-fs" />
  <project path="packages/apps/Launcher3" name="platform/packages/apps/Launcher3" groups="pdk-fs" />
  <project path="packages/apps/LegacyCamera" name="platform/packages/apps/LegacyCamera" groups="pdk-fs" />
  <project path="packages/apps/ManagedProvisioning" name="platform/packages/apps/ManagedProvisioning" groups="pdk-fs" />
  <project path="packages/apps/Messaging" name="platform/packages/apps/Messaging" groups="pdk-fs" />
  <project path="packages/apps/Music" name="platform/packages/apps/Music" groups="pdk-fs" />
  <project path="packages/apps/MusicFX" name="platform/packages/apps/MusicFX" groups="pdk-fs" />
  <project path="packages/apps/Nfc" name="platform/packages/apps/Nfc" groups="apps_nfc,pdk-fs" />
  <project path="packages/apps/OneTimeInitializer" name="platform/packages/apps/OneTimeInitializer" groups="pdk-fs" />
  <project path="packages/apps/PackageInstaller" name="platform/packages/apps/PackageInstaller" groups="pdk-fs" />
  <project path="packages/apps/Phone" name="platform/packages/apps/Phone" groups="pdk-fs" />
  <project path="packages/apps/PhoneCommon" name="platform/packages/apps/PhoneCommon" groups="pdk-cw-fs,pdk-fs"/>
  <project path="packages/apps/Protips" name="platform/packages/apps/Protips" groups="pdk-fs" />
  <project path="packages/apps/Provision" name="platform/packages/apps/Provision" groups="pdk-fs" />
  <project path="packages/apps/QuickSearchBox" name="platform/packages/apps/QuickSearchBox" groups="pdk-fs" />
  <project path="packages/apps/Settings" name="platform/packages/apps/Settings" groups="pdk-fs" />
  <project path="packages/apps/SoundRecorder" name="platform/packages/apps/SoundRecorder" groups="pdk-fs" />
  <project path="packages/apps/SpareParts" name="platform/packages/apps/SpareParts" groups="pdk-fs" />
  <project path="packages/apps/SpeechRecorder" name="platform/packages/apps/SpeechRecorder" groups="pdk-fs" />
  <project path="packages/apps/Stk" name="platform/packages/apps/Stk" groups="apps_stk,pdk-fs" />
  <project path="packages/apps/Tag" name="platform/packages/apps/Tag" groups="pdk-fs" />
  <project path="packages/apps/Terminal" name="platform/packages/apps/Terminal" groups="pdk-fs" />
  <project path="packages/apps/Test/connectivity" name="platform/packages/apps/Test/connectivity" />
  <project path="packages/apps/TvSettings" name="platform/packages/apps/TvSettings" groups="generic_fs" />
  <project path="packages/apps/UnifiedEmail" name="platform/packages/apps/UnifiedEmail" groups="pdk-fs" />
  <project path="packages/experimental" name="platform/packages/experimental" />
  <project path="packages/inputmethods/LatinIME" name="platform/packages/inputmethods/LatinIME" groups="pdk-fs" />
  <project path="packages/inputmethods/OpenWnn" name="platform/packages/inputmethods/OpenWnn" groups="pdk-fs" />
  <project path="packages/providers/ApplicationsProvider" name="platform/packages/providers/ApplicationsProvider" groups="pdk-fs" />
  <project path="packages/providers/BookmarkProvider" name="platform/packages/providers/BookmarkProvider" groups="pdk-fs" />
  <project path="packages/providers/CalendarProvider" name="platform/packages/providers/CalendarProvider" groups="pdk-cw-fs,pdk-fs" />
  <project path="packages/providers/CallLogProvider" name="platform/packages/providers/CallLogProvider" groups="pdk-fs" />
  <project path="packages/providers/ContactsProvider" name="platform/packages/providers/ContactsProvider" groups="pdk-cw-fs,pdk-fs" />
  <project path="packages/providers/DownloadProvider" name="platform/packages/providers/DownloadProvider" groups="pdk-cw-fs,pdk-fs" />
  <project path="packages/providers/MediaProvider" name="platform/packages/providers/MediaProvider" groups="pdk-cw-fs,pdk-fs" />
  <project path="packages/providers/PartnerBookmarksProvider" name="platform/packages/providers/PartnerBookmarksProvider" groups="pdk-fs" />
  <project path="packages/providers/TelephonyProvider" name="platform/packages/providers/TelephonyProvider" groups="pdk-cw-fs,pdk-fs" />
  <project path="packages/providers/TvProvider" name="platform/packages/providers/TvProvider" groups="pdk-fs" />
  <project path="packages/providers/UserDictionaryProvider" name="platform/packages/providers/UserDictionaryProvider" groups="pdk-cw-fs,pdk-fs" />
  <project path="packages/screensavers/Basic" name="platform/packages/screensavers/Basic" groups="pdk-fs" />
  <project path="packages/screensavers/PhotoTable" name="platform/packages/screensavers/PhotoTable" groups="pdk-fs" />
  <project path="packages/screensavers/WebView" name="platform/packages/screensavers/WebView" groups="pdk-fs" />
  <project path="packages/services/Mms" name="platform/packages/services/Mms" groups="pdk-cw-fs,pdk-fs" />
  <project path="packages/services/Telecomm" name="platform/packages/services/Telecomm" groups="pdk-cw-fs,pdk-fs" />
  <project path="packages/services/Telephony" name="platform/packages/services/Telephony" groups="pdk-cw-fs,pdk-fs" />
  <project path="packages/wallpapers/LivePicker" name="platform/packages/wallpapers/LivePicker" groups="pdk-fs" />
  <project path="pdk" name="platform/pdk" groups="pdk" />
  <project path="platform_testing" name="platform/platform_testing" />
  <project path="prebuilts/android-emulator" name="platform/prebuilts/android-emulator" groups="pdk-fs" />
  <project path="prebuilts/build-tools" name="platform/prebuilts/build-tools" groups="pdk" clone-depth="1" />
  <project path="prebuilts/clang/darwin-x86/host/3.6" name="platform/prebuilts/clang/darwin-x86/host/3.6" groups="pdk,darwin" />
  <project path="prebuilts/clang/linux-x86/host/3.6" name="platform/prebuilts/clang/linux-x86/host/3.6" groups="pdk,linux" />
  <project path="prebuilts/clang/host/darwin-x86" name="platform/prebuilts/clang/host/darwin-x86" groups="pdk,darwin" />
  <project path="prebuilts/clang/host/linux-x86" name="platform/prebuilts/clang/host/linux-x86" groups="pdk" />
  <project path="prebuilts/devtools" name="platform/prebuilts/devtools" groups="pdk-fs" />
  <project path="prebuilts/eclipse" name="platform/prebuilts/eclipse" groups="pdk" />
  <project path="prebuilts/eclipse-build-deps" name="platform/prebuilts/eclipse-build-deps" groups="notdefault,eclipse" />
  <project path="prebuilts/gcc/darwin-x86/aarch64/aarch64-linux-android-4.9" name="platform/prebuilts/gcc/darwin-x86/aarch64/aarch64-linux-android-4.9" groups="pdk,darwin,arm" />
  <project path="prebuilts/gcc/darwin-x86/arm/arm-linux-androideabi-4.9" name="platform/prebuilts/gcc/darwin-x86/arm/arm-linux-androideabi-4.9" groups="pdk,darwin,arm" />
  <project path="prebuilts/gcc/darwin-x86/host/i686-apple-darwin-4.2.1" name="platform/prebuilts/gcc/darwin-x86/host/i686-apple-darwin-4.2.1" groups="pdk,darwin" />
  <project path="prebuilts/gcc/darwin-x86/mips/mips64el-linux-android-4.9" name="platform/prebuilts/gcc/darwin-x86/mips/mips64el-linux-android-4.9" groups="pdk,darwin,mips" />
  <project path="prebuilts/gcc/darwin-x86/x86/x86_64-linux-android-4.9" name="platform/prebuilts/gcc/darwin-x86/x86/x86_64-linux-android-4.9" groups="pdk,darwin,x86" />
  <project path="prebuilts/gcc/linux-x86/aarch64/aarch64-linux-android-4.9" name="platform/prebuilts/gcc/linux-x86/aarch64/aarch64-linux-android-4.9" groups="pdk,linux,arm" />
  <project path="prebuilts/gcc/linux-x86/arm/arm-linux-androideabi-4.9" name="platform/prebuilts/gcc/linux-x86/arm/arm-linux-androideabi-4.9" groups="pdk,linux,arm" />
  <project path="prebuilts/gcc/linux-x86/host/x86_64-linux-glibc2.11-4.8" name="platform/prebuilts/gcc/linux-x86/host/x86_64-linux-glibc2.11-4.8" groups="pdk,linux" />
  <project path="prebuilts/gcc/linux-x86/host/x86_64-linux-glibc2.15-4.8" name="platform/prebuilts/gcc/linux-x86/host/x86_64-linux-glibc2.15-4.8"  groups="pdk,linux" />
  <project path="prebuilts/gcc/linux-x86/host/x86_64-w64-mingw32-4.8" name="platform/prebuilts/gcc/linux-x86/host/x86_64-w64-mingw32-4.8" groups="pdk-fs" />
  <project path="prebuilts/gcc/linux-x86/mips/mips64el-linux-android-4.9" name="platform/prebuilts/gcc/linux-x86/mips/mips64el-linux-android-4.9" groups="pdk,linux,mips" />
  <project path="prebuilts/gcc/linux-x86/x86/x86_64-linux-android-4.9" name="platform/prebuilts/gcc/linux-x86/x86/x86_64-linux-android-4.9" groups="pdk,linux,x86" />
  <project path="prebuilts/gdb/darwin-x86" name="platform/prebuilts/gdb/darwin-x86" groups="darwin" />
  <project path="prebuilts/gdb/linux-x86" name="platform/prebuilts/gdb/linux-x86" groups="linux" />
  <project path="prebuilts/go/darwin-x86" name="platform/prebuilts/go/darwin-x86" groups="darwin,tradefed" />
  <project path="prebuilts/go/linux-x86" name="platform/prebuilts/go/linux-x86" groups="linux,tradefed" />
  <project path="prebuilts/gradle-plugin" name="platform/prebuilts/gradle-plugin" groups="pdk-cw-fs,pdk-fs" />
  <project path="prebuilts/libs/libedit" name="platform/prebuilts/libs/libedit" groups="pdk-cw-fs,pdk-fs" />
  <project path="prebuilts/maven_repo/android" name="platform/prebuilts/maven_repo/android" groups="pdk-cw-fs,pdk-fs" />
  <project path="prebuilts/misc" name="platform/prebuilts/misc" groups="pdk" />
  <project path="prebuilts/ndk" name="platform/prebuilts/ndk" groups="pdk" />
  <project path="prebuilts/ninja/darwin-x86" name="platform/prebuilts/ninja/darwin-x86" groups="darwin,pdk,tradefed" />
  <project path="prebuilts/ninja/linux-x86" name="platform/prebuilts/ninja/linux-x86" groups="linux,pdk,tradefed" />
  <project path="prebuilts/python/darwin-x86/2.7.5" name="platform/prebuilts/python/darwin-x86/2.7.5" groups="darwin,pdk,pdk-cw-fs,pdk-fs" />
  <project path="prebuilts/python/linux-x86/2.7.5" name="platform/prebuilts/python/linux-x86/2.7.5" groups="linux,pdk,pdk-cw-fs,pdk-fs" />
  <project path="prebuilts/qemu-kernel" name="platform/prebuilts/qemu-kernel" groups="pdk" />
  <project path="prebuilts/sdk" name="platform/prebuilts/sdk" groups="pdk" />
  <project path="prebuilts/tools" name="platform/prebuilts/tools" groups="pdk,tools" />
  <project path="sdk" name="platform/sdk" groups="pdk-cw-fs,pdk-fs" />
  <project path="system/bt" name="platform/system/bt" groups="pdk" />
  <project path="system/ca-certificates" name="platform/system/ca-certificates" groups="pdk" />
  <project path="system/connectivity/apmanager" name="platform/system/connectivity/apmanager" />
  <project path="system/connectivity/dhcp_client" name="platform/system/connectivity/dhcp_client" />
  <project path="system/connectivity/shill" name="platform/system/connectivity/shill" />
  <project path="system/core" name="platform/system/core" groups="pdk" />
  <project path="system/extras" name="platform/system/extras" groups="pdk" />
  <project path="system/firewalld" name="platform/system/firewalld" />
  <project path="system/gatekeeper" name="platform/system/gatekeeper" groups="pdk" />
  <project path="system/keymaster" name="platform/system/keymaster" groups="pdk" />
  <project path="system/media" name="platform/system/media" groups="pdk" />
  <project path="system/nativepower" name="platform/system/nativepower" />
  <project path="system/netd" name="platform/system/netd" groups="pdk" />
  <project path="system/nvram" name="platform/system/nvram" />
  <project path="system/sepolicy" name="platform/system/sepolicy" groups="pdk" />
  <project path="system/security" name="platform/system/security" groups="pdk" />
  <project path="system/tools/aidl" name="platform/system/tools/aidl" groups="pdk-cw-fs,pdk-fs" />
  <project path="system/tpm" name="platform/system/tpm" />
  <project path="system/update_engine" name="platform/system/update_engine" />
  <project path="system/vold" name="platform/system/vold" groups="pdk" />
  <project path="system/weaved" name="platform/system/weaved" />
  <project path="system/webservd" name="platform/system/webservd" />
  <project path="toolchain/binutils" name="toolchain/binutils" />
  <project path="tools/adt/idea" name="platform/tools/adt/idea" groups="notdefault,tools" />
  <project path="tools/base" name="platform/tools/base" groups="notdefault,tools" />
  <project path="tools/build" name="platform/tools/build" groups="notdefault,tools" />
  <project path="tools/external/fat32lib" name="platform/tools/external/fat32lib" groups="tools" />
  <project path="tools/external/gradle" name="platform/tools/external/gradle" groups="tools" />
  <project path="tools/idea" name="platform/tools/idea" groups="notdefault,tools" />
  <project path="tools/loganalysis" name="platform/tools/loganalysis" groups="notdefault,tradefed" />
  <project path="tools/motodev" name="platform/tools/motodev" groups="notdefault,motodev" />
  <project path="tools/studio/cloud" name="platform/tools/studio/cloud" groups="notdefault,tools" />
  <project path="tools/swt" name="platform/tools/swt" groups="notdefault,tools" />
  <project path="tools/test/connectivity" name="platform/tools/test/connectivity" />
  <project path="tools/tradefederation" name="platform/tools/tradefederation" groups="notdefault,tradefed" />
</manifest>
