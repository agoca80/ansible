https://github.com/t-zuehlsdorff/gitlabhq/blob/master/doc/install/installation-freebsd.md

secret=$(</dev/random dd count=1 | base64 | cut -b-32)
