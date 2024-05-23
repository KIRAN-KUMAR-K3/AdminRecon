
```markdown
# AdminRecon

AdminRecon is a simple Python script that attempts to discover admin panels on a target website by brute-forcing common admin panel paths.

## Features

- Checks for admin panels using a predefined list of common paths.
- Provides colored output for different HTTP response statuses.
- Allows customization of request delay and output file via command-line arguments.

## Requirements

- Python 3.x
- `requests` library
- `colorama` library

## Installation

1. Clone the repository:
    ```sh
    git clone https://github.com/KIRAN-KUMAR-K3/AdminRecon.git
    cd AdminRecon
    ```

2. Install the required Python libraries:
    ```sh
    pip install -r requirements.txt
    ```

## Usage

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

## Output

The script will print the results in the terminal with different colors for different HTTP statuses:
- **200**: Blue - Admin panel found.
- **403**: Red - Access forbidden.
- **404**: Default - Not found.
- **302**: Yellow - Redirecting.
- Other statuses will be printed in blue with their status code.

The results will also be saved to the specified output file.

## Disclaimer

This script is for educational purposes only. Use it responsibly and do not use it to target websites without permission. The author is not responsible for any misuse of this tool.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Author

- Created by Kiran Kumar K

## Acknowledgements

- Thanks to the contributors of the `requests` and `colorama` libraries.

---

Feel free to contribute to this project by submitting issues or pull requests.
```
