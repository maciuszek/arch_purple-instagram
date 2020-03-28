# Maintainer: Matt Kuzminski <mattkuzminski at gmail dot com>

pkgname=purple-instagram-git
pkgver=master
pkgrel=1
pkgdesc="Instagram protocol plugin for libpurple (Pidgin)"
arch=('any')
url="https://github.com/EionRobb/purple-instagram/${pkgname}"
#license=("GPL")
makedepends=("git")
depends=("libpurple" "freeimage")
source=("purple-instagram-${pkgver}.tar.gz::https://github.com/EionRobb/purple-instagram/archive/master.zip")
sha256sums=('SKIP')

build() {
  cd "${srcdir}/purple-instagram-${pkgver}"
  make
}

package() {
  cd "${srcdir}/purple-instagram-${pkgver}"
  make DESTDIR="${pkgdir}/" install
}

