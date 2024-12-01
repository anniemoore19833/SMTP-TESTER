SMTP Tester
Overview

The SMTP Tester is a powerful and user-friendly tool to validate SMTP credentials. It allows users to test multiple SMTP servers quickly and efficiently while providing detailed results. The program is ideal for developers, system administrators, and email marketers.
Features

    SMTP Validation: Test multiple SMTP servers for valid credentials.
    Threaded Execution: Quickly process large lists of SMTP servers using multi-threading.
    Intuitive CLI Menu: User-friendly interface with clear options.
    Log Valid Credentials: Automatically saves working SMTP credentials to a file (smtp.txt).
    File Dialog Support: Select SMTP files via a graphical interface (Tkinter).
    Customizable Hidden Email: Sends hidden test emails for verification.

Requirements

    Python Version: Python 3.6 or above
    Dependencies:
        colorama (For colored terminal output)
        tkinter (For file dialog GUI, pre-installed in Python)
        smtplib (Built-in for email communication)
        concurrent.futures (For threading, built-in)

Installation

    Clone the Repository:

git clone https://github.com/yourusername/smtp-tester.git
cd smtp-tester

Install Dependencies:

pip install -r requirements.txt

Run the Script:

    python main.py

How to Use

    Prepare a file with SMTP credentials in the following format:

server|port|user|password|from_email (Optional: If `from_email` is not provided, `user` is used)

Example:

    smtp.mailgun.org|587|user1@example.com|password123|user1@example.com
    email-smtp.us-east-1.amazonaws.com|587|aws_access_key|aws_secret_key|noreply@example.com
    smtp-relay.sendinblue.com|587|apikey|api_secret_key

    Start the SMTP Tester:
        Select Option 2 (Normal SMTP Tester) to begin testing SMTPs.
        Choose the file containing SMTP credentials.
        Enter a test email address to validate the SMTP credentials.

    Results:
        Successful credentials are saved to smtp.txt in the same directory.


