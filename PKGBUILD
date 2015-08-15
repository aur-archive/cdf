# Maintainer:  TDY <tdy@archlinux.info>
# Contributor: Ricardo Martins <ricardo@scarybox.net>

pkgname=cdf
pkgver=0.2
pkgrel=1
pkgdesc="Colorized df"
arch=('i686' 'x86_64')
url="http://sourceforge.net/projects/bmp-plugins.berlios/"
license=('GPL')
depends=('glibc')
source=(http://downloads.sourceforge.net/project/bmp-plugins.berlios/$pkgname-$pkgver.tar.gz)
sha256sums=('3659ed779ec335c572f9ccec437469fc9c0e5c193f6b58f9e935bf337a080874')

build() {
  cd "$srcdir/$pkgname-$pkgver"
  ./configure --prefix=/usr
  make
}

package() {
  cd "$srcdir/$pkgname-$pkgver"
  make DESTDIR="$pkgdir" install
}

# vim:set ts=2 sw=2 et:
