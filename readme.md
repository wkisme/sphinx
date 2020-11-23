
This is sphinx tool for llvm use.
! Other zip file except  sphinx will be not used, because dot2tex has other packages to rely on. And i also don't use doxygen here, for reason in here https://github.com/llvm/llvm-project/blob/master/llvm/docs/README.txt.

Doxygen page Output
==============

Install doxygen <http://www.stack.nl/~dimitri/doxygen/download.html> and dot2tex <https://dot2tex.readthedocs.io/en/latest>.

    cd <build-dir>
    cmake -DLLVM_ENABLE_DOXYGEN=On <llvm-top-src-dir>
    make doxygen-llvm # for LLVM docs
    make doxygen-clang # for clang docs

It will generate html in

    <build-dir>/docs/doxygen/html # for LLVM docs
    <build-dir>/tools/clang/docs/doxygen/html # for clang docs
