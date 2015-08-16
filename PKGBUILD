#Autor: Alexandre Minoshi(Almin-Soft Group)
#Maintainer: Alexandre Minoshi

pkgname=libsystemdx
pkgver=0.17.1
pkgrel=1
pkgdesc="A library for systemdx, systemdx-gtk, systemdx-qt"
options=('!strip')
arch=('i686' 'x86_64')
url="http://almin-soft.fsay.net/index.php?systemdx-hide/tags/systemdx"
license=('GPL2')
if [ "${CARCH}" = 'x86_64' ]; then
depends=('lib32-libx11' 'lib32-gcc-libs')
elif [ "${CARCH}" = 'i686' ]; then
depends=('libx11' 'gcc-libs')
fi

source=("libsystemdx.so.tar.bz2::http://almin-soft.fsay.net/data/files/systemdx/download.php?get=libsystemdx.so.tar.bz2")

package() {
if [ "${CARCH}" = 'x86_64' ]; then
  install -Dm755 libsystemdx.so $pkgdir/usr/lib32/libsystemdx.so
elif [ "${CARCH}" = 'i686' ]; then
  install -Dm755 libsystemdx.so $pkgdir/usr/lib/libsystemdx.so
fi
}
md5sums=('fae7de9fd2a036d849962d870e50cf14')
