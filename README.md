Android device build for Rockchip RK3188 (MK908)
--------------

Device build files/information. Some CM specific structure
may be included at some point. This device build is specific
to MK908s and may not work in other RK3188 devices without
some modification. You do so of your own accord.

To be installed into: (android)/device/rockchip/rk3188/

Called from (android) via :
. build/envsetup.sh && brunch rk3188

**Revision history:**
- Initial commit, gotta start somewhere
- Merging in some of rkcrewtablets generic build
- More updates
- Initial mali gralloc, need to merge in properly now
- Pulled a bunch of prebuilt/proprietary down, moving into place
- Reorganizing the build structure to make more sense
- Kernel options moved to prebuilt to handle future kernel versions
(i.e. 720p, 1080p, kernels beyond 3.0.36, etc.)
- local_manifest.xml added for compile setup, move to (android)/.repo/
and then repo sync in the (android) directory (currently set to 
install my CWM recovery, device tree and kernel)
- variety of toolchains installed (for kernel build)
- updated Linaro toolchains to 2013.07 release
- lots of changes to reflect some of the stuff found in the MK908 SDK1 leak
- various changes to get things building nicer with CM versions
- some changes to replicate fun_'s generic rk3188 cwm for better input
