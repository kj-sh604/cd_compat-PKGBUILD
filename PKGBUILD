pkgname=cd_compat
pkgver=1
pkgrel=1
pkgdesc="cd 'binary' from Fedora Workstation"
arch=('any')
license=('UNLICENSE')

package() {
    install -dm755 "${pkgdir}/usr/bin"
    cat <<EOF > "${pkgdir}/usr/bin/cd"
#!/bin/sh
builtin cd "\$@"
EOF
    chmod +x "${pkgdir}/usr/bin/cd"
}
