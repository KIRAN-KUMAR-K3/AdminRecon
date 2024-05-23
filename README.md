
# AdminRecon

<p align="center">
  <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTk9Kx0uPmIqifrh6xyTZL0mi86BdPF8cjWDF4qU_3lzA&s" alt="AdminRecon Logo" width="200"/>
</p>

<p align="center">
  <b>AdminRecon</b> is a powerful Python script designed to discover admin panels on target websites by brute-forcing common admin panel paths.
</p>

<p align="center">
  <img src="https://img.shields.io/badge/python-3.x-blue.svg" alt="Python 3.x">
  <img src="https://img.shields.io/badge/license-MIT-green.svg" alt="License: MIT">
</p>

## 🚀 Features

- 🔍 Checks for admin panels using a predefined list of common paths.
- 🎨 Colored output for different HTTP response statuses.
- ⚙️ Customizable request delay and output file via command-line arguments.

## 📋 Requirements

- Python 3.x
- `requests` library
- `colorama` library

## 📦 Installation

1. Clone the repository:
    ```sh
    git clone https://github.com/KIRAN-KUMAR-K3/AdminRecon.git
    cd AdminRecon
    ```

2. Install the required Python libraries:
    ```sh
    pip install -r requirements.txt
    ```

## 🛠️ Usage

```sh
python adminrecon.py -u <URL> [-d <delay>] [-o <output file>]
```

- `-u, --url`: The target URL to be checked for admin panels. (Required)
- `-d, --delay`: Delay between requests in seconds. Default is 0.5 seconds. (Optional)
- `-o, --output`: Output file to save results. Default is `results.txt`. (Optional)

### Example

```sh
python adminrecon.py -u http://example.com -d 1 -o output.txt
```

## 🖥️ Output

The script prints the results in the terminal with different colors for different HTTP statuses:
- **200**: 💙 Blue - Admin panel found.
- **403**: ❤️ Red - Access forbidden.
- **404**: 🚫 Default - Not found.
- **302**: 💛 Yellow - Redirecting.
- Other statuses will be printed in blue with their status code.

Results are also saved to the specified output file.

## ⚠️ Disclaimer

This script is for educational purposes only. Use it responsibly and do not use it to target websites without permission. The author is not responsible for any misuse of this tool.

## 📜 License

This project is licensed under the MIT License - see the [MIT LICENSE]([LICENSE](https://github.com/KIRAN-KUMAR-K3/AdminRecon?tab=MIT-1-ov-file#) file for details.

## 👤 Author

- Created by [Kiran Kumar K](https://github.com/KIRAN-KUMAR-K3)

## 🙏 Acknowledgements

- Thanks to the contributors of the `requests` and `colorama` libraries.

---

Feel free to contribute to this project by submitting issues or pull requests.

<p align="center">
  <a href="https://github.com/KIRAN-KUMAR-K3/AdminRecon">
    <img src="https://img.shields.io/github/stars/KIRAN-KUMAR-K3/AdminRecon?style=social" alt="GitHub Stars">
  </a>
  <a href="https://github.com/KIRAN-KUMAR-K3/AdminRecon/fork">
    <img src="https://img.shields.io/github/forks/KIRAN-KUMAR-K3/AdminRecon?style=social" alt="GitHub Forks">
  </a>
</p>
