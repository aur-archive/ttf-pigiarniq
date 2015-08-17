# Maintainer: Mike Redd <mredd@0tue0.com>
# Contributor: Mike Redd <mredd@0tue0.com>
pkgname=ttf-pigiarniq
_pkgname=Pigiarniq
pkgver=2
pkgrel=1
pkgdesc="The Pigiarniq fonts were created as a joint project of the Government of Nunavut"
arch=('any')
license=('custom')
url="http://www.tiro.com/syllabics/resources/index.html"
_url="http://www.tiro.com/syllabics/resources/compiled_data_sources/Fonts/${_pkgname}/${_pkgname}1.2.zip"
depends=('fontconfig' 'xorg-fonts-encodings' 'xorg-font-utils')
install=ttf.install
source=("$_url" "LICENSE.txt")

md5sums=('f3be07af70e53b4c6805d260ae6e1918'
         '71c25abe45f3298f33f9a707a7c6bdee')

build() {
  cd $srcdir
  install -d $pkgdir/usr/share/fonts/TTF/
  install -m644 *.ttf $pkgdir/usr/share/fonts/TTF/ || return 1
  install -Dm644 *.txt $pkgdir/usr/share/licenses/$pkgname/LICENSE
}
