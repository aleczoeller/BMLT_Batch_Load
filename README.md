# BMLT_Batch_Load
Jupyter Notebook for batch loading meeting information to BMLT root server.

This workflow is written to pull meetings data from a table, format all the meeting information,
and remotely insert it into BMLT MySQL database set up as new.  For testing, I manually entered
several meetings and queried them from the connections set up below in order to get the process
right. 

In order to enable remote SQL connections, you need to add your IP address under cPanel/Remote MySQL under the Advanced cPanel section. You can run an ipconfig command in command shell or Google what is my IP to get that - please note that your IP address might get changed each time you connect to a router, so you might want to use a wildcard % (so if your home is 222.333.23.213 you might put 222.333.23.%).  

The data you have might be in an Excel or CSV table, if so see the Pandas functions read_csv or
read_excel in order to pull into a DataFrame.  In my case, I had everything as a JSON saved on 
our website as a JavaScript file. I pull this, convert it, and insert it into the BMLT server.

Use freely, hopefully some portion of this might be helpful - if only pulling data remotely. For 
assistance, please email aleczoeller at gmail dot com, or call at Nine 1 two, 358 six 5 six 4.
