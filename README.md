# FileCompressor

FileCompressor is a simple project that demonstrates file compression and decompression using Huffman coding. It includes encoding and decoding functionalities, implemented in C++.

## Project Structure

- `encode.cpp`: Contains the code to compress (encode) the input file using Huffman coding.
- `decode.cpp`: Contains the code to decompress (decode) the encoded file.
- `huffman.cpp`: Implements the Huffman coding algorithm.
- `huffman.hpp`: Header file containing the declarations of the functions and classes used in `huffman.cpp`.
- `inputFile.txt`: A sample input file to be compressed.

## How to Run

### Prerequisites

To compile and run this project, you'll need:

- A C++ compiler (e.g., `g++`).

### Compilation

1. Compile the Huffman encoding and decoding programs using the following commands:

    ```sh
    g++ -o compress encode.cpp huffman.cpp
    g++ -o extract decode.cpp huffman.cpp
    ```

### Usage

#### Encoding (Compression)

Run the encoder to compress the `inputFile.txt`:

```sh
./compress inputFile.txt outputFile.bin
```

This will generate a binary file named `outputFile.bin` containing the compressed data.

#### Decoding (Decompression)

Run the decoder to decompress the `outputFile.bin`:

```sh
./extract outputFile.bin outputFile.txt
```

This will regenerate the original text in a file named `outputFile.txt`.

### Additional Usage

- To encode a different file, replace `inputFile.txt` with the path to your file.
- To specify the output of the encoding process, change `outputFile.bin` to your desired file name.
- Similarly, when decoding, use the encoded binary file as the input, and specify the output file for the decompressed text.

