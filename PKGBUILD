# Maintainer: @magitian <magitian@duck.com>
pkgname=stratos-waybar-config
pkgver=1.1
pkgrel=0
pkgdesc="Waybar configuration for StratOS"
conflicts=('stratos-waybar-hyprland-config' 'stratos-waybar-niri-config')
arch=('any')
license=('GPL3')
depends=(
    'waybar'
    'ttf-jetbrains-mono-nerd'
)
provides=('stratos-waybar-config')
source=()
optdepends=('ttf-jetbrains-mono-nerd: Default nerd font')
install=stratos-waybar-config.install
prepare() {
    cp -r "$startdir/.config/" "$srcdir/"
}
package() {
    install -d "$pkgdir/etc/skel/.config"
    cp -r "$srcdir/.config/waybar/" "$pkgdir/etc/skel/.config/"
}
