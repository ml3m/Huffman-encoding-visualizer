# Huffman Encoding Visualizer

The Huffman Encoding Visualizer is a Go-based tool designed to visualize the Huffman encoding process. Utilizing the `treedrawer` library by m1gwings, this project allows users to explore the intricacies of Huffman coding, a popular algorithm for data compression.

## Example Usage
<p align="center"><img src="./photos-docs/s2.png" /></a></p>

## Usage

To run the Huffman Encoding Visualizer, execute the following command in your terminal:

```bash
go run main.go <input_file> [--codes | --count | --tree]
Arguments
<input_file>: The path to a text file that contains the input data. The first line of the file will be read as the input string for Huffman encoding.
Flags
--codes: Displays the Huffman codes for each character in the input text.

--count: Displays the occurrence count of each character in the input text.

--tree: Visualizes the Huffman tree structure.

Example Commands
Display Huffman Codes:

bash
Copy code
go run main.go input.txt --codes
This command will output the Huffman codes generated for each character based on the input text in input.txt.

Display Character Occurrences:

bash
Copy code
go run main.go input.txt --count
This command will print the frequency of each character present in the input text.

Visualize the Huffman Tree:

bash
Copy code
go run main.go input.txt --tree
This command will create a visual representation of the Huffman tree based on the input text.

Combine Flags:

bash
Copy code
go run main.go input.txt --codes --tree
This command will display both the Huffman codes and visualize the Huffman tree.

Requirements
Go 1.16 or later
The github.com/m1gwings/treedrawer/tree package for visualizing the Huffman tree.
Example Input File
Make sure your input file (e.g., input.txt) contains text formatted as follows:

Copy code
Hello, Huffman encoding!
