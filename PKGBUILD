# Contributor: Kamil Cukrowski <kamil@dyzio.pl>
# Original work by: Ciriaco Garcia de Celis
# Build with 

# build: makepkg --skipinteg
# clean: makepkg --clean --nobuild --nodeps  --noextract

pkgname=xfce-hkmon
pkgver=2.0
pkgrel=1
pkgdesc=""
arch=('any')
depends=('glibc')
source=(xfce-hkmon.cpp)

build() {
	g++ -std=c++0x -O3 -lrt xfce-hkmon.cpp -o xfce-hkmon
}

package() {
	mkdir -p $pkgdir/usr/local/bin/
	cp xfce-hkmon $pkgdir/usr/local/bin/
}

