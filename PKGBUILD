
# Maintainer: Sebastian Gutsche <sebastian.gutsche@gmail.com>
pkgname=polymake
pkgver=3.0r2
pkgrel=1
epoch=
pkgdesc="A tool for convex geometry"
arch=('x86_64')
url="www.polymake.org"
license=('GPL')
groups=()
depends=('apache-ant'
         'jdk7-openjdk'
         'gcc'
         'boost'
         'gmp'
         'mpfr'
         'perl'
         'perl-term-readline-gnu'
         'perl-xml-libxml'
         'perl-xml-libxslt'
         'perl-xml-writer'
         'libxslt' )
makedepends=()
checkdepends=()
optdepends=()
provides=()
conflicts=()
replaces=()
backup=()
options=()
install=
changelog=
source=("https://polymake.org/lib/exe/fetch.php/download/$pkgname-$pkgver.tar.bz2")
noextract=()
md5sums=( '08584547589f052ea50e2148109202ab' )
validpgpkeys=()

build() {
	cd polymake-3.0
	./configure --prefix=/usr
	make
}

package() {
	cd polymake-3.0
	make DESTDIR="$pkgdir/" install
}
