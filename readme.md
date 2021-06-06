
This is a good C++ starting point for TDD and refactoring Katas. Requires CMake and toolchain (gcc, MingW, etc..) to be installed.

### To Use:
- Clone this repo somewhere
- Edit CMakeLists.txt and change `<<TargetName>>` into something meaningful
- Probably change directory name as well
- Maybe delete .git directory to detach from github
- Clone google test in project directory
```
git clone https://github.com/google/googletest.git
```
That should be enough to use project in CLion or or the shell.

### To Use CLion

Execute the following in project directory to install google test:
- Open project in CLion (Select directory then open)
- Create two `Run Configurations` as follows:
  - Main Target: runs your `main` production code
    blah
    blah
  - Test Target: runs your unit tests
    blah
    blah

## To Use the Shell
- Make sure cmake and toolchain are installed

- From project folder execute this once:
```
cmake -Bbuild -H.
```

- To build both targets: 
```
cmake --build build --target all
```
Targets will be placed in build directory.

- To build a single target:
```
cmake --build build --target <<TargetName>>
```
