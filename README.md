# Project - Operating Systems II Module

This program handles the implementation of two tasks: tabulate and flatten, providing both single-process and multi-process versions.

## Features

The program mainly performs two tasks:

### Tabulate

Given a text, it produces a table containing, for each word in the text, the words that immediately follow it along with their frequency of occurrence.

Required parameters:
	- A text file in Unicode (UTF-8) encoding, structured in sentences ending with ., ?, or ! (other punctuation characters are ignored, except apostrophes).

Output is a CSV file containing a table where each row lists a word and its immediately following words with their frequencies.

### Flatten

Generates a text randomly using a frequency table in the same format produced by tabulate.

Required parameters:
	- A CSV file containing a table where each row lists a word and its immediately following words with their frequencies;
	-	The number of words to generate;
	-	An optional previous word from which to start the generation.

Output is a text file containing the randomly generated text.

## System Requirements

The program requires the following system components:
	-	GCC compiler (GNU Compiler Collection)
	-	GNU Scientific Library (GSL)

## Installation

The program can be installed using a simple make command:

```bash
make
```
## Usage

To run the tabulate task:

```bash
./bin/program tabulate input_file
```

To run the flatten task:

```bash
./bin/program flatten input_file words_to_generate -w previous_word
```


