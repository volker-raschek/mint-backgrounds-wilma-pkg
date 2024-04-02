# Maintainer: Markus Pesch <markus.pesch@cryptic.systems>

pkgname=mint-backgrounds-wilma
pkgver=1.0
pkgrel=1
pkgdesc="The backgrounds included in Linux Mint 21.3 wilma"
license=('Various')
arch=('any')
url="http://packages.linuxmint.com/pool/main/m/${pkgname}"
source=("${url}/${pkgname}_$pkgver.tar.gz")
sha256sums=('ef5a4edc7010d7ada5733c72c89570c22c1795b8f4c8cd6dbfd1509c482a37b5')

package() {
  mkdir --parents ${pkgdir}/usr/share/backgrounds/linuxmint-wilma
  mkdir --parents ${pkgdir}/usr/share/{cinnamon-background-properties,gnome-background-properties,mate-background-properties}

  cp --archive ${srcdir}/${pkgname}/backgrounds/linuxmint-wilma ${pkgdir}/usr/share/backgrounds
  cp --archive ${srcdir}/${pkgname}/cinnamon-background-properties/* ${pkgdir}/usr/share/cinnamon-background-properties
  cp --archive ${srcdir}/${pkgname}/gnome-background-properties/* ${pkgdir}/usr/share/gnome-background-properties
  cp --archive ${srcdir}/${pkgname}/mate-background-properties/* ${pkgdir}/usr/share/mate-background-properties
}
