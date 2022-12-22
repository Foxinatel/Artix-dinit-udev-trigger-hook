pkgname=dinit-udev-trigger-hook
pkgver=0.0.1
pkgrel=1
pkgdesc="Hook to replace waiting on udev-settle with udev-trigger for faster boot times"
arch=('any')
depends=('coreutils' 'findutils' 'sed')
source=('dinit-udev-trigger.hook' 'dinit-udev-trigger')
sha512sums=(
  '52ff6a148acedfc83d6f074f232b2528a9ecfa97a2152ee9d7b3d7ed82d4ab15af19d70ba34d40655f5b0b179546bc217ca31e3f0752d600edba299dce8eb092'
  'cfc034a0dea99f34f829ac4b18c492c9d45eb299d645c3e51611ce69ebbb7e54e83661f80c945387f3e549d17abbbbe538856a79152aba08f3c300f0a5e032dd'
)

package() {
  install -D -m644 dinit-udev-trigger.hook "$pkgdir/usr/share/libalpm/hooks/dinit-udev-trigger.hook"
  install -D -m755 dinit-udev-trigger "$pkgdir/usr/share/libalpm/scripts/dinit-udev-trigger"
}