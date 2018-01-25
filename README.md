
This template's goal is to give me a lower barrier to writing unit tests for
C/C++ projects. I keep a clone of this repo in `~/src` and I have a function in
my `~/.bash_aliases` file like this:
```
function gtest() {
    cp -i ~/src/gtest_template/test/* .
    git submodule add git@github.com:google/googletest.git gtest
}
```

Then, after tailoring to suite the needs of a particular project (need to edit
`CMakeLists.txt`, starting with the project name), I run tests by calling
`./test`.
