# Maintainer: Christoph Glaubitz <chris at chrigl dot de>

pkgname=ttf-ebgaramond
pkgver=0.016
pkgrel=1
pkgdesc="EB Garamond is an open source project to create a revival of Claude Garamont’s famous humanist typeface from the mid-16th century"
arch=('any')
url="http://www.georgduffner.at/ebgaramond/"
license=('custom:OFL')
depends=('fontconfig' 'xorg-font-utils')
conflicts=('otf-ebgaramond')
source=("https://bitbucket.org/georgd/eb-garamond/downloads/EBGaramond-${pkgver}.zip")
install=${pkgname}.install
md5sums=('ad76a14ea9b136557b474c3445caea08')
         
package() {
  cd "${srcdir}/EBGaramond-${pkgver}"
  install -d "${pkgdir}/usr/share/fonts/TTF"
  install -m644 ./otf/*.otf "${pkgdir}/usr/share/fonts/TTF/"
  install -Dm644 ./COPYING "${pkgdir}/usr/share/licenses/ttf-ebgaramond/COPYING"
}
