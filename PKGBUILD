# Maintainer: Nicola Ferru <nico ferru 190 at gmail dot com>
# Contributor: Nicola Ferru <nico ferru 190 at gmail dot com>

pkgname=libACR38Driver
pkgver=2008
pkgrel=1009
pkgdesc="Driver miniLector EVO"
arch=('i686' 'x86_64')
url="http://resources.bit4id.com/"
license=('GPL')
depends=('pcsclite')
source=("http://resources.bit4id.com/files/drivers/linux/dr_minilector_evo_it_linux.zip")
md5sums=('913db070c3b677fc5c4ff08c874781c7')

package() {
  cd "${srcdir}"
  unzip 2008_10_09_linux_ACR38Driver.bundle.zip
  install -d ${pkgdir}/usr/lib
  cp ACR38Driver.bundle/Contents/Linux/libACR38Driver ${pkgdir}/usr/lib/libACR38Driver

}
