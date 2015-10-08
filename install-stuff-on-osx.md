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
opam switch 4.02.3
# install camlzip + ocsigen + eliom
opam install camlzip ocsigenserver eliom
###### Installation of 
# pin specific dev versions
opam pin -n -y add eliom https://github.com/ocsigen/eliom.git
opam pin -n -y add eliom-base-app https://github.com/ocsigen/eliom-base-app.git
opam pin -n -y add js_of_ocaml https://github.com/ocsigen/js_of_ocaml.git
opam pin -n -y add ocsigen-toolkit https://github.com/ocsigen/ocsigen-toolkit.git
opam pin -n -y add ocsigen-widgets https://github.com/ocsigen/ocsigen-widgets.git
opam pin -n -y add ocsigenserver https://github.com/ocsigen/ocsigenserver.git
opam pin -n -y add ojquery https://github.com/ocsigen/ojquery.git
opam pin -n -y add reactiveData https://github.com/hhugo/reactiveData.git
opam pin -n -y add tyxml https://github.com/ocsigen/tyxml.git
# install them
opam install re aws eliom-base-app ocsigen-toolkit
```

## OS X Emacs stuff

```bash
opam install merlin ocp-indent

```


## Terminal prompt

```
PS1='\[\e[1;32m\][\u \t \W]\$\[\e[0m\] '
```
