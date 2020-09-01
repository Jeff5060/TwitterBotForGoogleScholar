# TwitterBotForGoogleScholar
Using Python 3, Twitter Bot automatically turns Google Scholar Alerts from Gmail Inbox into Twitter feeds to keep the public informed of the new discoveries.

## Author: 
Haojie Xu (B.S. Architectural Engineering, Re-AIM Undegraduate Researcher, The Pennsylvania State University)

## Credits
Juan Pablo Gevaudan, Ph.D., (Architectural Engineering Assistant Professor, Re-AIM PI, The Pennsylvania State University)
Responsive and Adaptive Infrastructure Materials (Re-AIM) research group (https://sites.psu.edu/reaim/)

## Logical Structure of Twitter Bot Code:
  Access and login to Gmail and Twitter > Check for new label specified email(Google Scholar Alerts) > If new mail is found, retrive the HTML body and parse unwanted characters, left with href links and titles > Attributes are converted and sent as Tweeter messages > Next iteration repeats > If no email is detected, program sleeps for 24 hours before restarting again

## Package installed:
  -email API
  -Beautiful
  -email parser
  -tweepy
  -time
  
## Additional steps taken before using the code:
  ### -enable Gmail IMAP for imaplib access
        -Gmail account setting > Forwarding and POP/IMAP > enable IMAP
  ### -Authorize app with Gmail
        -Can be done through this link: https://developers.google.com/gmail/api/auth/about-auth
  ### -Categorize incoming emails with tag
        -Gmail account setting > Labels > Create new label > Enter a new label name > Nest label under another label if needed >          specify label attributes
  ### -Apply for Twitter Developer Account for access to Twitter API and application token
        - link: https://developer.twitter.com/en/apply-
        
## Contribute
This code can be improved by increasing the time-processing performance. As a suggestion, users are encouraged to contribute by further functionalizing sections of the code. 
