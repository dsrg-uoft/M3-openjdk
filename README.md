OpenJDK 8 M3
============

OpenJDK 8 uses mercurial instead of git, so we supply a patch instead.

### Instructions

1. Clone OpenJDK 8: `hg clone http://hg.openjdk.java.net/jdk8u/jdk8u`
1. Checkout tag: `hg up jdk8u172-b11`
1. Get source: `bash get_source.sh`
1. Apply patch: `patch -p1 < openjdk8.patch`
1. Configure: `bash configure`
1. Build: `make image`
1. Distribution is `build/linux-x86_64-normal-server-release/images/j2sdk-image`
