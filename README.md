# baruchMFECPP_AdvHW8
# Final Project Advanced C++ Certification Baruch

This final project is focused on the Monte Carlo method of derivative pricing. The project begins by taking the code as it was in the last level section 7.7 and expanding on it slowly by making it more general and more abstract with every iteration.  You will see five folders in the directory: LastHW, P1, P2, P3, and P4. I now describe below what is in each folder.


The LastHW folder has the code as it was in the previous level 7.7.  This code started the process of creating objects from the original code that was just one giant procedural blob.  I stripped out the drift and diffusion parts of the SDE in its own class SDEGBM, and I also tinkered a bit with creating another class that would support Poisson jumps. That went into another class called SDEGBMPoisson.  Not a bad start but still majority of the code and logic was in the main() part.

In the P1 folder is arguably where the most work was done, and we are asked to implement the Monte Carlo pricing as in the context diagram below.  The finite difference scheme , Random number generation, SDE, Option Pricer, and input data needed are all stripped out and put into its own separate class. You then have a central mediator (central hub as I called it) that then pulls from each class and creates an object that ultimately kicks off the simulation.

image.png


-----------------------------------------------------


## Technologies and Installation Guide

I have Visual Studio 2022 Community Edition installed on a laptop running windows 10 pro. I also have the ISO C++20 Standard (/std:c++20) setting selected in the C++ language standard section under Properties.

Everything else should work as is since the necessary #include commands are in the relevant .hpp and .cpp files.

(General question for Avi would be what other things would I need to include here? Boost or other external libraries
if necessary right? Like GTest version if I had a separate test scenario train.yaml file or something if I were
compiling/running in Linux. Maybe a small blurb on CMake files and how they were organized. Just wanted your input on that.)
 
------

## Usage

Load the .sln file from the appropriate folder, make sure your language setting is on C++ 20, and you
are good to go!


------

## Contributors
Paul Lopez, and a ton and a half of documentation provided by Professor Duffy.

The most helpful document for me was "Application Design in C# The Monte Carlo Method for Option 
Pricing" which gave me a better handle on how I was to design this project.

------

## License
No licenses required. Just install everything for free, load the .sln solution file you need, and enjoy!
