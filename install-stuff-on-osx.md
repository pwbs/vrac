# setup dev env for os x

## Install ocsigen & utils

```bash
# install mac ports <https://www.macports.org/install.php>
open https://www.macports.org/install.php
# install pkg-config
sudo port install pkgconfig
# install sqlite
port install sqlite3
####### # install ocaml and camlp4
####### sudo port install ocaml ocaml-camlp4
# install pcre
sudo port install pcre
# install ImageMagick
sudo port install ImageMagick
# install sass
sudo gem install sass
# install md5sum
sudo port install md5sha1sum
# install opam and ocaml ## not sure installing ocaml is absolutely necessary but it's convenient to have a system installation of ocaml anyhow
port install opam ocaml
# init opam
opam init
## use a new terminal, or type
eval `opam config env`
# opam-switch to latest version of ocaml ## building using the system installation of ocaml will likely fail for many obscur reasons (like a ± corrupted camlp4)
opam switch 4.04.0


# install
opam install camlzip re  
```

## OS X Emacs stuff

```bash
opam install merlin ocp-indent

```


## Terminal prompt

```
PS1='\[\e[1;30m\][\u \t \[\e[0m\]\[\e[1;31m\] \w\[\e[0m\] \[\e[1;30m\]]\n\$\[\e[0m\] '
```

## Gnu stuff

```bash
sudo port install findutils coreutils diffutils 
export PATH=/opt/local/libexec/gnubin:$PATH
```

## Other stuff

```bash
opam install ocamlrss conf-gnutls ocamlnet.4.0.4

postgres -D local_db/ -p 3000
```

