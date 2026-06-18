File Organizer

Overview:
The File Organizer is a Python automation script that organizes files in a directory into separate folders based on their file extensions. It automatically categorizes files such as images, documents, videos, audio files, archives, source code, executables, and unknown file types.

This project demonstrates the use of Python’s os and shutil modules for file and directory management.

Features:
* Automatically organizes files by type
* Creates folders if they do not already exist
* Supports multiple file categories
* Moves unknown file types into an Others folder
* Easy to customize by adding new file extensions
* Beginner-friendly automation project

Technologies Used:
* Python 3.x
* os module
* shutil module
No external libraries are required.

Project Structure:

File-Organizer
│
├── file_organizer.py
├── test_files/
│   ├── image.jpg
│   ├── document.pdf
│   ├── video.mp4
│   └── ...
└── README.md

Supported File Categories:
* Folder	Supported Extensions:
* Images -	.jpg, .jpeg, .png, .gif, .bmp, .tiff, .webp
* Docs - .pdf, .doc, .docx, .txt, .rtf, .xls, .xlsx, .ppt, .pptx
* Videos -	.mp4, .mkv, .avi, .mov, .flv, .wmv
* Audio -	.mp3, .wav, .aac, .flac
* Archives -	.zip, .rar, .tar, .gz, .7z
* Executables -	.exe, .dmg, .app, .deb, .rpm
* Code -	.py, .java, .c, .cpp, .html, .css, .js
* Others -	Any unsupported file type

How It Works:
1. The program creates folders for each file category.
2. It scans all files in the selected directory.
3. It identifies the extension of each file.
4. The file is moved to its corresponding folder.
5. Unsupported file types are moved to the Others folder.

Example:

Before Organization:

test_files
│
├── image.jpg
├── document.pdf
├── video.mp4
├── music.mp3
├── archive.zip
├── script.py
└── other.xyz

After Organization:

test_files/
│
├── Images/
│     └── image.jpg
│
├── Docs/
│     └── document.pdf
│
├── Videos/
│     └── video.mp4
│
├── Audio/
│     └── music.mp3
│
├── Archives/
│     └── archive.zip
│
├── Code/
│     └── script.py
│
└── Others/
      └── other.xyz

How to Run:

1. Install Python 3.
2. Save the script as file_organizer.py.
3. Set the directory you want to organize:

source_directory = "./test_files"

4. Run the script:
python file_organizer.py
or
python3 file_organizer.py

Sample Output:
Creating dummy files in ./test_files...
Organizing files...
Moved 'image.jpg' to 'Images'
Moved 'document.pdf' to 'Docs'
Moved 'video.mp4' to 'Videos'
Moved 'archive.zip' to 'Archives'
Moved 'music.mp3' to 'Audio'
Moved 'script.py' to 'Code'
Moved 'other.xyz' to 'Others'
File organization complete!
