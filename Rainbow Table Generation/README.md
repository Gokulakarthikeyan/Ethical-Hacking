# RainbowTable Generation using RainbowCrack

RainbowCrack is a general propose implementation of Philippe Oechslin’s faster time-memory trade-off technique. It crack hashes with rainbow tables.

RainbowCrack uses time-memory tradeoff algorithm to crack hashes. It differs from the hash crackers that use brute force algorithm.

Installed size: 494 KB
How to install:

    sudo apt update
    sudo apt install rainbowcrack

## Rainbow Tables for Hashing Algorithms Like MD5, SHA1

Step 1: Setup RainbowCrack

Step 2: create a new folder and navigate into it :

    cd ~
    mkdir RainbowTables
    cd RainbowTables

Step 3: View the Parameters

    rtgen -h

Step 4: Generate the Rainbow Tables

    sudo rtgen md5 loweralpha-numeric 1 7 0 2400 2465212 0
    sudo rtgen sha1 mixalpha-numeric 1 6 0 1600 3000000 0

Step 5: Sort the Rainbow Tables

    rtsort .
