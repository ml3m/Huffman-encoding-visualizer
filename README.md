# Huffman Encoding Visualizer

The Huffman Encoding Visualizer is a Go-based tool designed to visualize the Huffman encoding process. Utilizing the `treedrawer` library by m1gwings, this project allows users to explore the intricacies of Huffman coding, a popular algorithm for data compression.

## Example Usage
<p align="center"><img src="./photos-docs/s2.png" /></a></p>

## Usage

To run the Huffman Encoding Visualizer, execute the following command in your terminal:

```bash
go run main.go <input_file> [--codes | --count | --tree]
```
### Arguments
<input_file>: The path to a text file that contains the input data. The first line of the file will be read as the input string for Huffman encoding.

## Flags
--codes: Displays the Huffman codes for each character in the input text.

--count: Displays the occurrence count of each character in the input text.

--tree: Visualizes the Huffman tree structure.

## Requirements and Dependencies
Go 1.16 or later
The github.com/m1gwings/treedrawer/tree package for visualizing the Huffman tree.
Example Input File
Make sure your input file (e.g., input.txt) contains text formatted as follows:

### Make sure you add Dependencies:
```bash
go get github.com/m1gwings/treedrawer/tree
```

## Example Commands
Display Huffman Codes:

```bash
go run main.go input.in --codes
```
This command will output the Huffman codes generated for each character based on the input text in input.txt.

### Display Character Occurrences:

```bash
go run main.go input.in --count
```
This command will print the frequency of each character present in the input text.

### Visualize the Huffman Tree:

```bash
go run main.go input.in --tree
```
This command will create a visual representation of the Huffman tree based on the input text.
