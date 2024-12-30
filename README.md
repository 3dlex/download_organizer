# Organize Downloads

`organize_downloads.py` is a Python script to help you organize files in your downloads folder by categorizing them into folders based on file types such as images, documents, audio, videos, and more.

## Features

- Automatically categorizes files into predefined folders:
  - **Images**: `.jpg`, `.jpeg`, `.png`, `.gif`, `.tiff`, `.bmp`, `.svg`
  - **Documents**: `.pdf`, `.docx`, `.xlsx`, `.pptx`, `.txt`, `.md`
  - **Audio**: `.mp3`, `.wav`, `.aac`, `.flac`
  - **Videos**: `.mp4`, `.mov`, `.avi`, `.mkv`
  - **Archives**: `.zip`, `.rar`, `.tar.gz`
  - **Others**: Any file types not covered above
- Creates folders automatically if they don't exist.
- Moves files into the appropriate folders, keeping your downloads directory tidy.

## Prerequisites

- Python 3.x

## Installation

1. Clone this repository or download the script directly:
   ```bash
   git clone https://github.com/yourusername/organize-downloads.git
   cd organize-downloads
   ```

2. Ensure Python is installed on your system. You can check by running:
   ```bash
   python --version
   ```

## Usage

1. Open the script `org_downloads.py` in a text editor.

2. Replace the placeholder path `/path/2/downloads/` in the `downloads_path` variable with the path to your downloads folder. For example:
   ```python
   downloads_path = '/home/username/Downloads/'
   ```

3. Run the script:
   ```bash
   python org_downloads.py
   ```

4. Once executed, the script will organize files in your downloads folder into subfolders based on their file types.

## Example

### Before Running the Script:
```
Downloads/
|-- image1.jpg
|-- document1.pdf
|-- song.mp3
|-- video.mp4
```

### After Running the Script:
```
Downloads/
|-- Images/
|   |-- image1.jpg
|-- Documents/
|   |-- document1.pdf
|-- Audio/
|   |-- song.mp3
|-- Videos/
|   |-- video.mp4
```

## Customization

You can modify the `file_types` dictionary in the script to include additional file extensions or create new categories. For example:
```python
file_types = {
    'Code': ['.py', '.js', '.html', '.css'],
    'Images': ['.jpg', '.jpeg', '.png']
}
```

## Contributing

Contributions are welcome! If you have suggestions for improvements or new features, feel free to open an issue or submit a pull request.

## License

This project is licensed under the MIT License.

## Acknowledgments

Inspired by the need to keep downloads folders clutter-free.
