# Maintainer: Giovanni Scafora <giovanni@archlinux.org>
# Contributor: Matteo Mattei <matteo.mattei@gmail.com>

pkgname=libasecnsp11
pkgver=1
pkgrel=3
pkgdesc="Software for Carta Nazionale dei Servizi"
arch=('i686' 'x86_64')
url="https://tscns.regione.sardegna.it/"
license=('GPL')
depends=('pcsclite')
source=("https://tscns.regione.sardegna.it/sites/default/files/2017-11/linux_driver_Athena.zip")
md5sums=('26dee77a9e75088143cc62a3fbf8017c')

package() {
  cd "${srcdir}"

  install -d ${pkgdir}/usr/lib
  if [ "`uname -m`" = "i686" ]
    then
      cp -a x86/libaseCnsP11.so ${pkgdir}/usr/lib/libaseCnsP11.so
    else
      cp -a x64/libaseCnsP11.so ${pkgdir}/usr/lib/libaseCnsP11.so
  fi
}
