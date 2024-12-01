SMTP Tester
Overview


### Main Menu:
![Main Menu Screenshot](https://github.com/anniemoore19833/SMTP-TESTER/blob/main/Screenshot%202024-11-30%20162628.png)

git add README.md
git commit -m "Added screenshot to README"
git push origin main


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

DOWNLOAD AND RUN 

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


