pkgname=brew-wallpaper
pkgver=1.0
pkgrel=0
pkgdesc="Wallpapers for GNU/Linux"
arch=('any')
url="https://github.com/celestifyx/brew-wallpaper"
license=('GPL')
options=(!strip !emptydirs)

prepare() {
    cp -af ../files/. "$srcdir"
}

package() {
    local _dir="$pkgdir"/usr/share/wallpapers

    mkdir -p "$_dir"
    cp -r "$srcdir"/* "$_dir"
}