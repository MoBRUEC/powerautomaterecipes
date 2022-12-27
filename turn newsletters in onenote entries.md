## Turn newsletters into OneNote entries 

Want to save newsletters or any other precious mails you receive to OneNote, where they're indexed?
Easy job with Power Automate:
![Time Zone Conversion in Power Automate](/images/03.png)

The compose step "peeked code" looks like this:

``` 
"inputs": "<html>\n<head>\n<title>@{triggerOutputs()?['body/subject']}</title>\n<meta name=\"created\" content=\"@{triggerOutputs()?['body/receivedDateTime']}\" />\n</head>\n<body data-absolute-enabled=\"true\" style=\"font-size:20px\">\n<br/>@{body('Convert_time_zone')}<br/>\n<br/>@{triggerOutputs()?['body/body']}<br/>\n</body>\n</html>"
```

![Composing content for a new (Microsoft) TODO](/images/04.png)

Adding a todo on top linking to the new OneNote entries ("web" and "client" links) is easy enough:
![OneNote web and client URIs](images/05.png)

The "Web client link" is the link to the web representation of your OneNote content. The client link will open up in your desktop application of OneNote.
And don't forget to clean up when everything is done and dusted ;):
![Delete the mail and handle errors](/images/06.png)