# Maintainer: @magitian <magitian@duck.com>
pkgname=stratos-waybar-niri-config
pkgver=1.1
pkgrel=0
pkgdesc="Waybar configuration for StratOS' Niri spin"
conflicts=('stratos-waybar-hyprland-config')
arch=('any')
license=('GPL3')
depends=(
    'waybar'
    'ttf-jetbrains-mono-nerd'
)
provides=('stratos-waybar-niri-config')
source=()
optdepends=('ttf-jetbrains-mono-nerd: Default nerd font')
install=stratos-waybar-niri-config.install
prepare() {
    cp -r "$startdir/.config/" "$srcdir/"
}
package() {
    install -d "$pkgdir/etc/skel/.config"
    cp -r "$srcdir/.config/waybar/" "$pkgdir/etc/skel/.config/"
}
