## Get yourself a note about the size of your OneNote book. 

![Checking your OneNote book size](/images/01.png)
The formula for the file size conversion:

*div(div(outputs('Get_file_metadata_using_path')?['body/Size'],1024),1024)*

In this simple flow, a notification via Teams will be sent in regular intervals. If the OneNote book queried grows beyond 2 GB in size you should consider splitting it up into multiple OneNote books, for performance and efficiency reasons. (Depends on your client hardware, however. Assuming you are using OneNote maybe via the fat client for your OS, be it Windows or MacOS.)

