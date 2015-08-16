# Maintainer: Evan Teitelman <teitelmanevan@gmail.com>
# Contributor: Sébastien Luttringer <seblu@aur.archlinux.org>

pkgname=netmask
pkgver=2.3.12
pkgrel=2
pkgdesc='Helps determine network masks'
arch=('i686' 'x86_64')
url='http://packages.qa.debian.org/n/netmask.html'
license=('GPL2')
source=("http://cdn.debian.net/debian/pool/main/n/${pkgname}/${pkgname}_${pkgver}.tar.gz")
md5sums=('802cf8e2a310aaee367bda930b048520')

build() {
  cd $pkgname-$pkgver
  ./configure --prefix=/usr --mandir=/usr/share/man
  make
}

package() {
  cd $pkgname-$pkgver
  make DESTDIR="$pkgdir" install
}

# vim:set ts=2 sw=2 ft=sh et:
