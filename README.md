#checkerupper

A simple bash command to check up on sites;

#TO DO:

Add ease of use commands;

Look into better handling of responses from curl;

Add a sufficient number of test sites with varying response codes;

Allow files to be passed as arguments, may require switches or even....reading user input...my god..;

Include what each error code means at the bottom of the email, only once;

Only send one mail with multiple recipients instead of one mail for each;

#USAGE:

Populate a sites.txt file with the sites you wish to check in the same directory as auto_checker.sh;

If you want to send to a number of emails you may populate a file email_list.txt;

Basic usage from command line:
./auto_checker.sh email@domain.com;
\#This will run the command and send the output only to the email specified in the argument;

Advanced usage reading from the email_list.txt:
./auto_checker.sh
\#This will run the command and send the output to the emails located in the email_list.txt file, note currently this sends separate mails for each user but not each site;

For email_list.txt make sure the emails are on separate lines:
```
Good:
yes@domain.com
this@domain.com
works@domain.com
```

```
Bad:
nope@domain.com, fail@domain.com, lol@domain.com
```
\#This may be implemented later depending on my laziness factor;
