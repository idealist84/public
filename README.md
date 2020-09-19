# CME Tracker: readme.md

## Synopsis
This is a web application for physicians in the United States to track their personal Continuing Medical Education (CME) credits and generate activity reports against our database of state medical board requirements.

## Prerequisites
- You have downloaded the latest version of Chrome, Firefox, IE/Edge, or Opera. Sorry, Safari is not supported.
- You are a physician in the United States with an MD license. DO licenses are sometimes governed by a separate medical board within the same state.
- You have an National Provider Identifier (NPI) registered and up to date with the National Plan & Provider Enumeration System (NPPES).
- Your CME activity sponsor is accredited by the Accreditation Council for Continuing Medical Education.
- You have read this readme.

## Motivation
As a physician who has had to submit reports and evidence of my continuing education to a number of medical boards and privileging offices, it has been an annoying administrative task to try to recall the conferences, lectures, and other activities I had completed over the last several years. Additionally, being licensed in multiple states meant I had to keep track of what the requirements were for each state. Having an application that can keep track of the various requirements and compare my current credits helps me ensure I will be in compliance when it is time to renew my license, and it can help generate reports when requested.

## Installation
Using `flask run` in the CS50 IDE, click on the generated link.

## Using CME Tracker
On the landing page, you can click on the Register link to get started, or log in if you've already created an account.

### Register
You'll need to use your *full legal name as it is registered in NPPES* to create an account.
1. Have your NPI number and each state medical license number handy. You do not need your DEA number.
2. Choose a unique username.
3. Choose a unique password that you do not use for other accounts.
4. Enter your email, date of birth and NPI.
5. Choose the state where you are licensed, enter your license number, and date of next renewal.
6. Click the "+" to add more licenses.
7. Click Register and you're done!

### Home page
If you have license information on your profile, this page will display information on how many CME credits you will need for your next renewal, how many you've earned, and how many more you will need to log.
If you have CME activities logged, this page will also display the most recent ten activities.

### Add
Add CME activities here. You'll need:
- Sponsoring organization (which must be accredited by ACCME)
- Title of activity
- Short topic
- Date of activity (or date when activity was completed for multi-day activities)
- Hours of AMA PRA 1 credits claimed
- Whether the activity satisfies state requirements for specific topics, such as pain or geriatrics.

### Reports
Specify:
- state or organization receiving the report
- start and end dates (inclusive) of the report

Report will include:
- physician name and state medical license number
- date report was generated
- activity list, including the city and state of the sponsoring organization's headquarters
- summary of total credit hours completed during the specified time period

## Future
- add upload capability, to have a central repository for CME certificates.
- generate PDFs for easy printing.
- create API for medical boards to obtain this information digitally

## Contributors
[@idealist84](https://github.com/idealist84)

## License
[MIT](https://opensource.org/licenses/MIT)
