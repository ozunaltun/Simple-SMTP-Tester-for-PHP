# :email: SMTP Testing Tool with PHP

![PHP Version](https://img.shields.io/badge/PHP-7.4%2B-blue)
![License](https://img.shields.io/badge/License-MIT-green)

This repository contains a simple yet powerful PHP script designed specifically for SMTP testing. The script enables you to configure various SMTP settings including the server, sender email, and more. It's intended to assist developers and testers in configuring and verifying SMTP servers.

:warning: **Please note**: This tool is intended for testing purposes and should not be deployed in production environments.

## :sparkles: Features

- :satellite: Easily specify SMTP server.
- :envelope: Define sender email.
- :key: Simple HTML authentication for security during testing.
- :outbox_tray: Seamlessly send test emails through the specified SMTP server.

## :gear: Prerequisites

- PHP 7.4 or later.
- Web Server (e.g. Apache, Nginx).
- PHPMailer library files.

## :rocket: Getting Started

1. Clone this repository:
    ```sh
    git clone <repository-url>
    ```

2. Place the PHP script in your web server directory.

3. Access the script through your web browser.

## :package: Using PHPMailer

This script employs the PHPMailer library for sending emails. Make sure to adhere to the licensing terms of PHPMailer.

### Including PHPMailer

You need to include the PHPMailer library in your project. PHPMailer is under the LGPL license, and you can find a copy of this license in the PHPMailer directory.

### Attribution

PHPMailer is a third-party library used in this script for sending emails. The original project source is available on [PHPMailer's GitHub repository](https://github.com/PHPMailer/PHPMailer).

## :closed_lock_with_key: Security Notice

This tool uses simple HTML authentication with hardcoded passwords in the PHP script. While this approach might be acceptable for testing, it is inherently insecure and should not be used in a production environment.

### Recommendations:
- Avoid storing passwords and sensitive data in the script.
- Implement robust authentication mechanisms.
- Ensure the use of secure connections (SSL/TLS) for SMTP communication.

## :page_with_curl: License

This script is provided under the MIT License. However, PHPMailer is licensed under LGPL, which you can find in the PHPMailer directory.

## :raising_hand: Contributions

Contributions to improve this tool are always welcome! Feel free to fork the repository and send pull requests, or open issues if you find any problems or have suggestions.
