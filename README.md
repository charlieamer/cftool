# cftool
Get inputs and outputs for a specific problem on codeforces.

# Install

#### NPM
You need to have both `node js` and `npm` installed in order to use `cftool`.
```
npm install -g cftool
```

#### From source
```
wget https://raw.githubusercontent.com/guilhermeleobas/cftool/compile_and_test/install.sh
chmod +x
./install.sh
```

# Version
1.1

# Usage

### get
```
cftool get 550A # Download inputs and outputs for problem 550A
cftool get 600 # Download inputs and outputs for all problems on contest 600.
```

### compile
```
cftool compile code.cc # Compile code.cc using g++.
cftool compile -l c++11 code.cc  # Compile code.cc with g++ 11.
cftool compile code.py # nothing will happen.
```

### test
```
cftool test code.cc 620A # will run code.cc with 620 inputs and check if their outputs are correct.
```

To get full list of available commands run cftool with --help flag.

```
  Usage: cftool [options] [command]


  Commands:

    get <number>                     Get input/output for a problem or contest
    compile [options] <file>         compile your code
    test [options] <file> <problem>  Test your code against a problem

  Options:

    -h, --help     output usage information
    -V, --version  output the version number
```

# License
MIT
