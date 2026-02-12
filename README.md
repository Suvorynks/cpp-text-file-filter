# Text File Filtering Utility (C++)

This C++ program is a practical tool for automated text processing. It reads content from a source file and selectively writes lines to a target file based on predefined logic, showcasing the power of file streams and string buffers.

###  Logic & Functionality
The application implements a "Read-Filter-Write" pipeline:
1. **Source Access:** Opens `file1.txt` for input (reading).
2. **Buffering:** Iteratively reads each line into a fixed-size character buffer (`MAX_LINE_LENGTH = 256`).
3. **Condition Check:** Validates the line content before processing.
4. **Data Persistence:** Writes the processed/selected lines into `file2.txt` for storage.



###  Key Features
* **File Stream Management:** Uses `std::ifstream` and `std::ofstream` to manage independent data streams.
* **Resource Safety:** Includes explicit error checking for file availability and ensures proper closing of handles.
* **Efficient String Handling:** Utilizes C-style character arrays for low-level memory control during text parsing.
* **Clean UI:** Provides clear console feedback during the process (e.g., notifying the user when the operation is complete).

###  Technical Stack
* **Language:** C++
* **Header:** `<fstream>` (File streams), `<iostream>`.
* **Concepts:** Stream redirection, Buffer management, Procedural programming.

###  How to Use
1. Place a text file named `file1.txt` in the same directory as the executable.
2. Run the program.
3. The utility will automatically generate `file2.txt` containing the filtered content.
4. Review the results in the console output.
