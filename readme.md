# Web Services and SOA Mini Project

This project is part of a course in which we practice the implementation of Web Services and Communication Protocols. The objective is to automate the generation and distribution of invitations for an online general assembly meeting for a large international company. Each participant will receive a personalized invitation with a copy of the company's yearly report attached.

## Requirements

- Python 3.11.x
- Libraries: requests, pandas, smtplib, ssl, bs4 (Beautiful Soup), email.message
- Access to external public web services for genderizing names (SOAP and REST)

## Project Structure

- `main.py`: The main Python script that generates and sends invitations.
- `guest_list.csv`: Contains a list of invitees with their names, email addresses and IP addresses.
- `yearly_growth_report.pdf`: The attachment to be sent with the invitations.

## Usage

1. Clone this repository.
2. Make sure you have Python 3.11.x installed.
3. Install the required libraries using `pip install requests pandas beautifulsoup4`.
4. Modify the `email_sender` and `email_password` variables with your email credentials.
5. Run the `main.py` script.

The script will extract gender information from names using external web services, generate titles (Mr., Ms., or blank) based on gender and location, and send personalized invitations to the list of guests.

## External Web Services

- IP Geolocation Service (SOAP): Used to identify the country of an IP address.
- Genderize Service (REST): Used to identify/predict gender based on names.

## Contributors

- Robert Pallesen
- Mathias Brix Drejer
- Tobias Linge Jensen