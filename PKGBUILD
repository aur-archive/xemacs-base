# Contributor: Juergen Hoetzel <juergen@archlinux.org>

pkgname=xemacs-base
pkgver=2.19
pkgrel=1
pkgdesc="Fundamental XEmacs support, you almost certainly need this"
arch=(i686 x86_64)
url="http://www.xemacs.org"
license=('GPL')
depends=('xemacs')
conflicts=('xemacs-sumo')
source=(http://ftp.xemacs.org/pub/xemacs/packages/$pkgname-$pkgver-pkg.tar.gz)
md5sums=('b11cf876d7719567d624ab8f331df50a')

package() {
  cd $srcdir
  for subdir in etc lisp; do 
      install -d $pkgdir/usr/lib/xemacs/xemacs-packages/${subdir}
      cp -a ${subdir}/*  $pkgdir/usr/lib/xemacs/xemacs-packages/${subdir}
  done
}
