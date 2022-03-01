How to build MoCHi
==================

 Install the required tools/libraries listed below,
 and run "bash build", which generates "src/mochi.exe".


What do you need?
=================

- OCaml 4.09, 4.10, or 4.11
- Tools/Libraries available via opam 2
  (Run "opam install z3 dune batteries ocamlfind ppx_deriving yojson camlp5 zarith apron menhir")
    - Z3 4.8.9
    - dune 2.5
    - batteries 3.0.0
    - ocamlfind/findlib
    - ppx_deriving
    - Yojson
    - camlp5
    - zarith
    - apron
    - Menhir
- Standard system tools (See the Dockerfile or run "apt-get install -y git make gcc m4 opam libgmp-dev libmpfr-dev libglpk-dev autoconf")
- HorSat2 binary (https://github.com/hopv/horsat2)
- HoIce binary (https://github.com/hopv/hoice)
    - HoIce is not necessary to run MoCHi, but the lack of HoIce may degrade the performance. (See [Sato+ PEPM2019])

Dockerfile
==========

 There is a Dockerfile for compiling MoCHi.
 Dockerfile assumes the HorSat2 binary is in the same directory.


Licenses
========

 This software is licensed under the Apache License, Version2.0 (http://www.apache.org/licenses/LICENSE-2.0.txt).

 The software uses the following libraries/tools.
 Please also confirm each license of the library/tool.
- CSIsat (https://github.com/dzufferey/csisat)
- ATP (http://www.cl.cam.ac.uk/~jrh13/atp/)


Author
=======

 MoCHi is developed/maintained by Ryosuke SATO <rsato@is.s.u-tokyo.ac.jp>


Contributors
============

- Hiroshi Unno
- Takuya Kuwahara
- Keiichi Watanabe
- Naoki Iwayama
