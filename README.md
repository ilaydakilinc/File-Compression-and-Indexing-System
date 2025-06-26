# 📦 File Compression and Indexing System

A simplified file management system developed for the Computer Algorithms course. This project combines Huffman Coding, B+ Trees and Red-Black Trees to provide efficient file compression and directory indexing all through a user-friendly Command Line Interface (CLI).

## 🚀 Features

- 🔐 **File Compression & Decompression** using Huffman Coding (lossless)
- 🌲 **File Directory Indexing** using B+ Tree (efficient listing and range queries)
- 🌳 **File Search** using Red-Black Tree (fast exact-match lookups)
- 💻 **CLI Interface** for ease of use
- 💾 Persistent indexes stored and reloaded using JSON

## 🧠 Technologies & Concepts

- **Python 3.12.6**
- **Huffman Coding**: Frequency-based binary encoding for compression
- **B+ Tree**: Ordered, balanced tree structure for indexing
- **Red-Black Tree**: Balanced BST for fast searching
- **JSON**: For persistent index storage

## 🛠️ How to Use

1. **Compress a File**
   python main.py compress <path_to_file>
2. **Decompress a File**
   python main.py decompress <path_to_compressed_file>
3. **Insert File into Index**
   python main.py insert <file_name> <file_path>
4. **Search for File by Name**
   python main.py search <file_name>
5. **Delete File from Index**
   python main.py delete <file_name>
6. **List All Indexed Files**
   python main.py list

# 📌 Index data is stored in `bplus_index.json` and `rbt_index.json` and automatically reloaded on startup.

## 🧪 Testing and Edge Cases

- Compression of empty or single-character files
- Handling of UTF-8 and Latin-1 encodings
- Duplicate file insertions
- Searching for non-existent files
- Handling corrupted or incompatible `.compressed` files

## 📁 Project Structure

├── main.py
├── compression/
│ └── huffman.py
├── index/
│ ├── bplus_tree.py
│ └── red_black_tree.py
├── cli/
│ └── interface.py
├── data/
│ └── *.json
└── README.md


## 📚 Libraries Used

- `argparse` – Command-line parsing
- `heapq` – Priority queue for Huffman Tree
- `json` – Index persistence
- `os`, `shutil` – File operations

## 👥 Authors

- İlayda Kılınç


## 📌 License

This project was developed as part of a university course and is intended for educational use.









