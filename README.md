# Information Disclosure

This repository contains a Python script designed to interact with the Wayback Machine's CDX API. The script fetches archived URLs for a given domain or pattern, filters the results based on file types, and saves the filtered URLs to a file. Additionally, it can download the last saved archived page for a user-selected URL.

## Features
- **Fetch Archived URLs**: Uses the Wayback Machine's CDX API to search for archived URLs matching a user-defined domain or pattern.
- **Regex Filtering**: Filters results for specific file types, such as `.pdf`, `.json`, `.docx`, `.sql`, and many more.
- **Save Results**: Saves filtered URLs to a file named `filtered.txt`.
- **Download Archived Page**: Allows the user to download the last saved version of an archived page directly from the Wayback Machine.

## Supported File Types for Filtering
The script filters URLs containing the following file extensions:
- `.xls`, `.xml`, `.xlsx`, `.json`, `.pdf`, `.sql`, `.doc`, `.docx`, `.pptx`
- `.txt`, `.zip`, `.tar`, `.gz`, `.tgz`, `.bak`, `.7z`, `.rar`, `.log`, `.cache`
- `.secret`, `.db`, `.backup`, `.yml`, `.config`, `.csv`, `.yaml`, `.md`, `.md5`
- `.exe`, `.dll`, `.bin`, `.ini`, `.bat`, `.sh`, `.deb`, `.rpm`, `.iso`, `.img`
- `.apk`, `.msi`, `.dmg`, `.tmp`, `.crt`, `.pem`, `.key`, `.pub`, `.asc`

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/andrei2308/Information-Disclosure.git
   cd Information-Disclosure
   ```

2. Ensure you have Python 3 installed.

3. Install required dependencies:
   ```bash
   pip install requests
   ```

## Usage
1. Run the script:
   ```bash
   python script_name.py
   ```

2. Follow the prompts:
   - Enter the domain or pattern to search for archived URLs.
   - Review the output saved to `out.txt` (all URLs) and `filtered.txt` (filtered URLs).
   - Optionally, download the last saved version of a selected archived page.

### Example
**Input:**
```
Enter a domain or pattern to search for: example.com
```

**Output:**
- `out.txt`: Contains all retrieved URLs from the Wayback Machine.
- `filtered.txt`: Contains filtered URLs matching predefined file extensions.
- If a page is downloaded, it will be saved as `downloaded_page.html`.

## Notes
- Ensure you have an active internet connection to interact with the Wayback Machine API.
- This script is designed for cross-platform compatibility and does not require Unix commands.

## Contributing
Contributions are welcome! Feel free to fork the repository, make your changes, and submit a pull request. For issues or feature requests, open an issue in the repository.

## License
This project is licensed under the [MIT License](LICENSE).

---

### Disclaimer
This script is intended for research and educational purposes only. Use responsibly and ensure compliance with applicable laws and regulations.

