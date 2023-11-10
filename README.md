# Huffman Compression and Decompression in C

### Overview

This project implements the Huffman coding algorithm for lossless data compression and decompression in C. Huffman coding is a widely-used method of encoding data that assigns variable-length codes to input characters, with shorter codes assigned to more frequent characters. This is achieved by constructing a Huffman tree from the frequencies of the characters in the input data.

### What it does

The project reads an input message from the user and compresses it using Huffman encoding, then decompresses the encoded message back into the original text. The output shows the original message, the encoded binary string, the size comparison between the uncompressed and compressed data, and finally, the decompressed message.

### How It Works

1. **Frequency Analysis**: A frequency table is constructed from the input message to determine how often each character occurs.
2. **Huffman Tree Construction**: Based on the frequency table, a Huffman tree is built. Characters with higher frequencies are placed closer to the root, thereby getting shorter codes.
3. **Encoding**: The Huffman tree is traversed to assign codes to each character, which are then used to encode the message.
4. **Compression Output**: The encoded message and a dictionary mapping each character to its code are displayed. The amount of space saved by compression is also shown.
5. **Decompression**: The encoded message is decoded using the Huffman tree, reproducing the original message.

### Where It Is Used

Huffman coding is used in various applications, such as:

- File compression tools (e.g., ZIP, RAR, etc.).
- Media codecs for image (e.g., JPEG) and video compression.
- Data transmission protocols to reduce the size of data sent over a network.

### Build and Run

Make sure you have a C compiler installed on your system (e.g., `gcc`).

1. Save the source code to a file, e.g., `huffman.c`.
2. Compile the program:
```bash
gcc huffman.c -o huffman
```
3. Run the compiled executable:
```bash
./huffman
```
4. Follow the on-screen prompts to input a message for compression.

### Limitations

- The current implementation uses fixed-size arrays; for processing large datasets, consider modifying data structures to dynamically allocate memory as needed.
- The project does not provide file input/output capabilities; it reads and writes messages via the standard console.

### Author

[Sujay R](https://github.com/sujay1844)
