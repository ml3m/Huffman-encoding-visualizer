# Huffman Encoding Visualizer

The Huffman Encoding Visualizer is a Go-based tool designed to visualize the Huffman encoding process. Utilizing the `treedrawer` library by m1gwings, this project allows users to explore the intricacies of Huffman coding, a popular algorithm for data compression.

## Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Getting Started](#getting-started)
- [Usage](#usage)
- [Input Format](#input-format)
- [Visualization](#visualization)
- [How Huffman Encoding Works](#how-huffman-encoding-works)
- [Contributing](#contributing)
- [License](#license)

## Overview

Huffman coding is a method used for lossless data compression. This visualizer allows users to input a text string, which is then processed to generate a Huffman tree and corresponding codes. The tree is visualized, providing insights into the encoding mechanism.

## Features

- **Huffman Tree Visualization**: Displays the Huffman tree structure for the given input.
- **Huffman Code Generation**: Generates Huffman codes for each character in the input text.
- **Frequency Analysis**: Prints a frequency array showing the number of occurrences of each character.
- **User-Friendly Interface**: Simple command-line interface for easy input and output.

## Getting Started

### Prerequisites

- Go programming language (version 1.16 or higher)
- Git

### Installation

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/ml3m/Huffman-encoding-visualizer.git
Navigate to the Project Directory:

'''bash
cd Huffman-encoding-visualizer
'''
Build the Project:

'''bash
go build -o huffman_visualizer
'''

Install Dependencies: Make sure to get the required dependencies using:

'''bash
go get
'''

Usage
To run the Huffman Encoding Visualizer, provide an input file containing text. The program reads the first line of the file as the input string.

Command to Run the Visualizer
bash
Copy code
./huffman_visualizer input.txt
Example
To see how the program works, you can create an input file input.txt with the following content:

Copy code
hello world
Then run:

bash
Copy code
./huffman_visualizer input.txt
Input Format
The input file should contain text on the first line. The program reads this line to perform Huffman encoding.

Example Input
Example 1:

Copy code
hello world
Example 2:

Copy code
huffman coding
Visualization
The program visualizes the Huffman tree using the treedrawer library. The tree representation shows how characters are encoded, with each branch representing a binary decision (0 or 1) leading to a character.

How Huffman Encoding Works
Frequency Calculation: The program calculates the frequency of each character in the input string.
Tree Construction: A priority queue (min-heap) is used to build the Huffman tree based on character frequencies.
Code Generation: Each leaf node in the tree corresponds to a character, with the path from the root to the leaf determining the Huffman code.
Output: The generated Huffman codes and the frequency array are printed to the console, and the Huffman tree is displayed.
Code Structure
HuffmanNode: Struct representing each node in the Huffman tree, containing character, frequency, and pointers to left and right child nodes.
PriorityQueue: Implementation of a min-heap to facilitate tree construction.
Functions:
BuildHuffmanTree(input string): Constructs the Huffman tree from the input string.
GenerateHuffmanCodes(node *HuffmanNode, code string, codes map[rune]string): Generates the Huffman codes recursively.
DrawHuffmanTree(node *HuffmanNode, parent *tree.Tree, freqMap map[rune]int): Visualizes the Huffman tree.
Contributing
Contributions to the Huffman Encoding Visualizer are welcome! If you would like to contribute, please follow these steps:

Fork the repository.
Create a new branch for your feature or bug fix.
Make your changes and commit them.
Push your changes to your forked repository.
Submit a pull request with a description of your changes.
License
This project is licensed under the MIT License - see the LICENSE file for details.

sql
Copy code

Feel free to modify any sections or add more details as needed!
