# Maintainer: Sam Clark <sam@samhclark.com>
pkgname=ttf-ibm-plex
pkgver=6.4.0
pkgrel=1
pkgdesc="IBM's font family designed to work well in user interface (UI) environments and other mediums. Contains sans-serif, serif, monospace, and condensed subfamilies."
arch=('any')
url="https://www.ibm.com/plex/"
license=('LicenseRef-OFL-1.1-RFN')
source=("$pkgname-$pkgver.zip::https://github.com/IBM/plex/releases/download/v${pkgver}/TrueType.zip")
sha256sums=('7e4f80047782fe9eb74cd0b63019da283a15db98942da476fee46098633a083c')

package() {
    install -D --mode=644 --target-directory="${pkgdir}/usr/share/fonts/ibm-plex" TrueType/IBM-Plex-Mono/*.ttf
    install -D --mode=644 --target-directory="${pkgdir}/usr/share/fonts/ibm-plex" TrueType/IBM-Plex-Sans/*.ttf
    install -D --mode=644 --target-directory="${pkgdir}/usr/share/fonts/ibm-plex" TrueType/IBM-Plex-Sans-Condensed/*.ttf
    install -D --mode=644 --target-directory="${pkgdir}/usr/share/fonts/ibm-plex" TrueType/IBM-Plex-Serif/*.ttf
    install -D --mode=644  TrueType/IBM-Plex-Sans/license.txt "${pkgdir}/usr/share/licenses/${pkgname}/LICENSE"
}
