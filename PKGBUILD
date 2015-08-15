# Maintainer: Maxwell Pray a.k.a. Synthead <synthead@gmail.com>
# Contributor: TheGrudge <andi.clemens@gmx.net>

pkgname=gimp-plugin-plasma2
pkgver=2.11
pkgrel=4
arch=('i686' 'x86_64')
license=('GPL')
pkgdesc='Generates cloud-like structures, known as "plasma fractals"'
url="http://www.t2-project.org/packages/plasma2.html"
depends=('gimp')
makedepends=('pkgconfig')
source="http://dl.dropbox.com/u/24716740/mirror/plasma2-$pkgver.tar.bz2"
md5sums=('8a4cb3bab1756920ab2dadb4e32b79c5')

build() {
	cd "$srcdir/plasma2-$pkgver"
	make
}

package() {
	install -Dm 755 "$srcdir/plasma2-$pkgver/plasma2" "$pkgdir/usr/lib/gimp/2.0/plug-ins/plasma2"
}
