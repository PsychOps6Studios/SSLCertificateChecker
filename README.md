Features

Checks SSL certificates for multiple domains

Supports both HTTPS (port 443) and SMTP (port 25) certificates

Provides color-coded output for easy identification of issues

Calculates days remaining until expiration

Can read domains from a file or command line

Option to export results to CSV

Customizable warning threshold

Requirements

PowerShell 5.1 or later

Network connectivity to the target domains

Appropriate permissions to make outbound connections

The script will work on Windows, Linux, and macOS with PowerShell Core.

Basic Usage:
.\SSLCertificateChecker.ps1 -Domains "example.com"

Using Domains File:
.\SSLCertificateChecker.ps1 -DomainsFile "C:\path\to\domains.txt"

Check SMTP certificates:
.\SSLCertificateChecker.ps1 -Domains "example.com" -SMTP

Change warning threshold (default 30 days):
.\SSLCertificateChecker.ps1 -Domains "example.com" -DaysWarning 60

Export results to CSV:
.\SSLCertificateChecker.ps1 -Domains "example.com" -OutputCSV "C:\results.csv"

