# week02-class-project

# Ohm's law calculator 

## Purpose
A C++ program that calculates electrical current using Ohm's Law. It read a resistance, prints the current in A, and rejects invalid inputs

## Input Format
Two numbers are separated by a space. The voltage is in volts, and the resistance is in ohms. 

## Build and run
    mkdir -p build
    g++ -std=c++17 -Wall -Wextra -pedantic src/main.cpp -o build/app
    ./build/app

## Example output
    $ ./build/app
    12 4
    Current: 3 A

## Limitations
- Negative voltages are accepted (`-12 4` will print `Current: -3 A`).
- Any extra inputs after the two numbers is ignored.
- Results show about 6 significant digits (`10 3` prints `Current: 3.33333 A`).

## Debugging reflection
My tests passed locally but failed with 'bash: tesh.sh: No such file or directory'. This is because I named test.sh to tests.sh