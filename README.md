```
# DeltaSuite

DeltaSuite is a security tool designed to guard against unauthorized network access and alert users to potential intrusions on Windows systems. This program monitors network connections and sends alerts if suspicious activity is detected.

## Features

- Monitors network connections for unauthorized access.
- Sends email alerts when potential intrusions are detected.
- Logs all activities for further analysis.

## Requirements

- Python 3.x
- Internet access for sending email alerts.
- Access to the system's `netstat` command.

## Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/yourusername/deltasuite.git
   ```

2. Navigate to the directory:

   ```bash
   cd deltasuite
   ```

3. Install the required packages (if any):

   ```bash
   pip install -r requirements.txt
   ```

## Configuration

1. **Email Alerts**: Update the `EMAIL_ADDRESS`, `EMAIL_PASSWORD`, and `ALERT_EMAIL` in the `delta_suite.py` file with your email credentials and the recipient's email address.

2. **SMTP Server**: Ensure the SMTP server details in `send_alert` function are correctly set for your email provider.

## Usage

Run the script:

```bash
python delta_suite.py
```

The program will continuously monitor network connections and alert the specified email address if unauthorized access is detected.

## Logs

All activities, including checks and alerts, are logged in `delta_suite.log` for audit and analysis.

## Disclaimer

This tool is intended for educational and authorized network monitoring purposes only. Unauthorized use of this software is prohibited.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.