# Generated by gem2arch (https://github.com/anatol/gem2arch)
# Maintainer: Anatol Pomozov <anatol.pomozov@gmail.com>

_gemname=net-http-digest_auth
pkgname=ruby-$_gemname
pkgver=1.4
pkgrel=1
pkgdesc='An implementation of RFC 2617 - Digest Access Authentication'
arch=(any)
url='http://github.com/drbrain/net-http-digest_auth'
license=()
depends=(ruby)
options=(!emptydirs)
source=(https://rubygems.org/downloads/$_gemname-$pkgver.gem)
noextract=($_gemname-$pkgver.gem)
sha1sums=('2b2826cf85fe307c4b770de5c077880d8d8f1fe2')

package() {
  local _gemdir="$(ruby -e'puts Gem.default_dir')"
  gem install --ignore-dependencies --no-user-install -i "$pkgdir/$_gemdir" -n "$pkgdir/usr/bin" $_gemname-$pkgver.gem
  rm "$pkgdir/$_gemdir/cache/$_gemname-$pkgver.gem"
}
