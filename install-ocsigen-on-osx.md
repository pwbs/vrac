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
# install opam and ocaml ## not sure installing ocaml is absolutely necessary but it's convenient to have a system installation of ocaml anyhow
port install opam ocaml
# init opam
opam init
## use a new terminal, or type
eval `opam config env`
# opam-switch to latest version of ocaml ## building using the system installation of ocaml will likely fail for many obscur reasons (like a ± corrupted camlp4)
opam switch 4.02.3
# install ocsigen + eliom
opam install ocsigenserver eliom
######
# install specific dev versions
opam pin add eliom https://github.com/ocsigen/eliom.git
opam pin add eliom-base-app https://github.com/ocsigen/eliom-base-app.git
opam pin add js_of_ocaml https://github.com/ocsigen/js_of_ocaml.git
opam pin add ocsigen-toolkit https://github.com/ocsigen/ocsigen-toolkit.git
opam pin add ocsigen-widgets https://github.com/ocsigen/ocsigen-widgets.git
opam pin add ocsigenserver https://github.com/ocsigen/ocsigenserver.git
opam pin add ojquery https://github.com/ocsigen/ojquery.git
opam pin add reactiveData https://github.com/hhugo/reactiveData.git
opam pin add tyxml https://github.com/ocsigen/tyxml.git
```
