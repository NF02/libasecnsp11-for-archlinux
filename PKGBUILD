# Maintainer: Giovanni Scafora <giovanni@archlinux.org>
# Maintainer: Nicola Ferrru <nicoferru centonovanta at gmail dot com>
# Contributor: Matteo Mattei <matteo.mattei@gmail.com>

pkgname=libasecnsp11
pkgver=1
pkgrel=3
pkgdesc="Software for Carta Nazionale dei Servizi"
arch=('i686' 'x86_64')
url="https://www.bit4id.com/it/?option=com_zoo&ta"
license=('GPL')
depends=('pcsclite')
source=("http://resources.bit4id.com/files/drivers/linux/dr_minilector_evo_it_linux.zip")
md5sums=('913db070c3b677fc5c4ff08c874781c7')

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
