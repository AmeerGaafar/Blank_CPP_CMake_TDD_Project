
This is a good C++ starting point for TDD and refactoring Katas. Requires CMake and toolchain (gcc, MingW, etc..) to be installed.

### To Use:
- Clone this repo somewhere
- Edit CMakeLists.txt and change `TargetName` into something meaningfull
- Probably change directory name as well
- Maybe delete .git directory to detach from github
- Clone google test in project directory
```
git clone https://github.com/google/googletest.git
```
That should be enough to use project in CLion or or the shell.

### To Use CLion

## Execute the following in project directory to install google test:
- Open project in CLion (Select directory then open)
- Create two configurations, one that targets `TargetName` and the other `TargetName_Test`

## To Use the Shell
1- Make sure cmake and toolchain are installed

2- from project folder execute this once:
```
cmake -Bbuild -H.
```

3-to build both targets: 
```
cmake --build build --target all
```
Targets will be placed in build directory.

4- to build a single target:
```
cmake --build build --target <<TargetName>>
```
