
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
         'default-jdk'
         'gcc'
         'boost'
         'gmp'
         'mpfr'
         'perl'
         'perl-term-readline-gnu'
         'perl-xml-libxml'
         'perl-xml-xslt'
         'perl-xml-writer'
         'w3c-dtd-xhtml'
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
md5sums=()
validpgpkeys=()

build() {
	cd "$pkgname-$pkgver"
	./configure --prefix=/usr
	make
}

package() {
	cd "$pkgname-$pkgver"
	make DESTDIR="$pkgdir/" install
}
