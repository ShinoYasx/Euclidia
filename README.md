# Euclidia

I (Yasx pronounced "Yasix") am developping a bunch of libraries for mathemacical operations on prime numbers.

For the time being this draft (when compiled) asks for a number (a 64 bits unsigned integer, so it cannot exceed (2^64)-1) and gives you the dividers of this number and the prime factors with their respective exponent.
E.g. 4213 returns 11 and 383 for both dividers and prime factors.

Thanks to AeroStun who helps me to optimize the code.

## Build

If you're on a Linux or \*nix system you juste have to run :

```
git clone https://github.com/ShinoYasx/Euclidia.git
cd Euclidia
mkdir build
cd build
cmake ..
cmake --build .
```

And then you get an executable called "Euclidia" that you can launch using a terminal.

## Usage

In the same directory as the binary, with a console :

```
$ ./Euclidia //this launches the program
Enter a number
456132 //if you enter a number too large it will take a very long time
456132 is dividable by 2; 3; 4; 6; 12; 38011; 76022; 114033; 152044; 228066; 
Prime factors of 456132 : 2 pow 2; 3 pow 1; 38011 pow 1;
```

When I entered 54564156151 it took me over than 9 minutes to finish computing, with an i7 4790k overclocked at 5.0GHz, and the (anticipated) results are :

```
54564156151 is dividable by 37; 1474706923; 
Prime factors of 54564156151 : 37 pow 1; 1474706923 pow 1; 
```

## Built with

* [Ninja](https://ninja-build.org) - Optimized build system
* [CMake](https://cmake.org) - A cross-platform build tool
