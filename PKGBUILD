pkgname=blockout2
pkgver=2.5
pkgrel=1
pkgdesc="3D tetris, free adaptation of the original BlockOut DOS game edited by California Dreams in 1989"
arch=("x86_64")
url="http://www.blockout.net/blockout2/"
depends=("libgl" "glu" "libxext" "sdl" "sdl_mixer")
license=("GPL")
source=("blockout2" "blockout2.desktop" "blockout2.png" "http://downloads.sourceforge.net/project/blockout/blockout/BlockOut%202.5/bl25-linux-x64.tar.gz")
md5sums=('130e2c10b68b41bf12e67a764a2ea4fb'
         'c3d7d196e4af7fabd287376988376fe4'
         '166642ab949cd145f6126857a5ac7e4f'
         '6155d0596d762852e3fbd1718d3d6455')
         
package() {
   install -d "$pkgdir"/{opt,usr/bin,usr/share/applications,usr/share/pixmaps}
	chmod -x "$srcdir"/blockout/README.txt "$srcdir"/blockout/images/background.png "$srcdir"/blockout/sounds/music.ogg
	mv "$srcdir"/blockout "$pkgdir"/opt/blockout2
	cp -L "$srcdir"/blockout2 "$pkgdir"/usr/bin/
	cp -L blockout2.desktop "$pkgdir"/usr/share/applications/
	cp -L blockout2.png "$pkgdir"/usr/share/pixmaps/
}

