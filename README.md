# filter less

This is a C program for filtering BMP images. The program reads in a BMP file, applies a filter based on a command-line argument, and writes the filtered image to a new BMP file.

Dependencies

This program depends on the getopt.h, stdio.h, and stdlib.h libraries, as well as the helpers.h header file.

Installation

To compile the program, run the following command in your terminal:

css
Copy code
gcc -o filter filter.c helpers.c -lm
Usage

The program takes three command-line arguments:

css
Copy code
./filter [flag] infile outfile
where flag is the filter to be applied (b, g, r, or s), infile is the input BMP file, and outfile is the output BMP file.

Filters

The program supports the following filters:

b: Blur
g: Grayscale
r: Reflection
s: Sepia
Example

To apply the sepia filter to an input BMP file called input.bmp and save the result to a file called output.bmp, run the following command:

css
Copy code
./filter s input.bmp output.bmp
License

This program is licensed under the MIT License. See the LICENSE file for more information.
