# Maintainer: Limao Luo <luolimao+AUR@gmail.com>

pkgname=dropbox-light-panel-icons
pkgver=1.0
pkgrel=10
pkgdesc="Notification icons for Dropbox for themes with bright panels."
arch=(any)
url=https://forums.dropbox.com/topic.php?id=7818
license=(CCPL:by-3.0)
depends=(dropbox hicolor-icon-theme)
conflicts=(dropbox-{dark-panel,humanity{,-dark}}-icons)
install=icons.install
source=($pkgname.tar.gz::'https://dl.dropbox.com/u/62148/Misc/Dropbox Light Panel.tar.gz?dl=1')
sha256sums=('ddf634665612aa8dad6ca4a733286b4b4625e74beb71c6daa9bdd9ab15fbc39a')
sha512sums=('919a9bbffb6c4b0f1da1b85041bc5071bca42bdad122ad668509602e718be4301e590e8551d3c30226d9004a92fa629180c1c30bcdbba038269c04fccdb2b75c')

package() {
    cd "$srcdir"/icons/
    for i in *.png; do
        install -Dm644 $i "$pkgdir"/usr/share/icons/hicolor/16x16/statusdropboxstatus-$i
    done
}
