# Maintainer: Robert Orzanna <orschiro at gmail dot com>

pkgname=image-clipboard-to-file
pkgver=1.0
pkgrel=2
pkgdesc="Python script that saves an image from clipboard to a file"
arch=('any')
url="https://gist.github.com/orschiro/8b9a1ddadb696c2b4587"
license=('GPL2')
depends=('python2' 'pygtk')
source=('https://gist.githubusercontent.com/orschiro/8b9a1ddadb696c2b4587/raw/dce3cb421a71e31ee8177b5047bc76e4045d7102/image-clipboard-to-file.py')
md5sums=('aa1044daed2a5dd2d75d7ddb8d758121')

prepare() {
    sed -i 's/python/python2/g' "$srcdir/$pkgname.py"
}

package() {
    install -d -m755 "$pkgdir/usr/bin"
    install -m755 "$srcdir/$pkgname.py" "$pkgdir/usr/bin/$pkgname"
}

