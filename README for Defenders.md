README for Defendors: Fidan Karimova, Shahzeb Khalid, Raba Al-Eryani, Eital Schattner-Elmaleh, Nediyana Daskalova

As defenders we categorically went through all the javascripts files which handle the processing including the server and found various CSRF flaws as well as XSS flaws as well as javacripts injections. 

The first file that we started editing was contribution. We proceeded to remove all possible javascript injections by removing eval() and replacing it with parseFloat.

In the allocations file, a user can be logged on with a simple request to the userID field. This makes it easy for attacks to evade our security structure and therefore we should have extra check to prevent this from happening. 

In secession.js we use a much stronger regex which checks that there is at least one lower case, one upper case, one digit and least least 8 characters. This will make sure that secure enough passwords are being created to prevent attacks from easily accessing the website. 

In server.js, in order to set html flags for cookies sent to the clients, we would import an express module that would help us verify the cookies. However, we have been unable to locate this module 

