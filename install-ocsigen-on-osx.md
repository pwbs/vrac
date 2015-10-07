```bash
# install mac ports <https://www.macports.org/install.php>
open https://www.macports.org/install.php
# install pkg-config
sudo port install pkgconfig
# install sqlite
port install sqlite3
# install ocaml and camlp4
sudo port install ocaml ocaml-camlp4
# install pcre
sudo port install pcre
# install opam
port install opam
# init opam
opam init
## use a new terminal, or type
eval `opam config env`
# install ocsigen + eliom
opam install ocsigenserver eliom

```
