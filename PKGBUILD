# Maintainer: John Hall <hall.john.wesley@gmail.com>
pkgname=fdnsc
pkgver=1.0
pkgrel=2
epoch=
pkgdesc="A freedns.afraid.org dynamic DNS update client"
arch=(any)
url="http://freedns.afraid.org/scripts/freedns.clients.php"
license=('GPL')
groups=()
depends=('wget' 'sed' 'coreutils' 'util-linux')
makedepends=()
checkdepends=()
optdepends=()
provides=()
conflicts=()
replaces=()
backup=('etc/fdnsc.conf')
options=()
install=
changelog=
source=(fdnsc fdnsc.service fdnsc.conf fdnsc.logrotate)
noextract=(fdnsc fdnsc.service fdnsc.conf fdnsc.logrotate)
md5sums=('4d9ffb55599e016ecb6afac1c63efa20'
         'a0a2cd726b0e2d9c04c4c805b988f615'
         '5124ae0377b2737864a972306fb70464'
         '75c54f21ac72649db5e05a06d8d684dc')

#build() {
#}

#check() {
#}

package() {
  mkdir -p $pkgdir/usr/bin
  cp -p fdnsc $pkgdir/usr/bin/fdnsc
  mkdir -p $pkgdir/usr/lib/systemd/system
  cp -p fdnsc.service $pkgdir/usr/lib/systemd/system/fdnsc.service
  mkdir -p $pkgdir/etc
  cp -p fdnsc.conf $pkgdir/etc/fdnsc.conf
  mkdir -p $pkgdir/etc/logrotate.d
  cp -p fdnsc.logrotate $pkgdir/etc/logrotate.d/fdnsc
}
