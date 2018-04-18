## Description

Encodes text inside a textfile using UTF8 zero-width spaces.

Zero-width space is used to represent a '1' bit, and
zero-width non-joiner space is used to represent a '0'.
These are placed after a word followed by a space,
except if leading spaces or end of line.

Inspired by the [ZWFP](https://github.com/vedhavyas/zwfp) project,
the basic version of the encoder/decoder is less than 70 lines of
[Ruby](https://www.ruby-lang.org), including boilerplate code
and comments.

## Usage

Encoding:

    ./zerowidth --encode Super Secret Text 12345 < sample-normal.txt > sample-steg.txt

Decoding:

    ./zerowidth < sample-steg.txt

