# Asterisk 18 Extensions

On this GitHub page, you can find the basic configuration settings for an Asterisk 18 server with 50 extensions. 

# How to setup Extensions for Asterisk 18

To setup, the configurations for your Asterisk server do the following:

- Add the files to your Asterisk directory
- Update the pjsip.conf file with; [your server public ip], [your server private ip], [the extension passwords]

After you have set the configurations files, restart your Asterisk 18 with the following command

```
systemctl restart asterisk
```

You Asterisk has been installed and you can now use the extensions feature.

# How many extensions are there in configurations files

We have setup the extensions 1000 till 1050.

# How to add more extensions

Adding more extensions to the configurations files can be done by adding the following lines to the pjsip.conf file.

```
;==========Extension
[1051](aor-single-reg)
[1051](auth-userpass)
username=1051

[1051](endpoint-basic)
auth=1051
outbound_auth=1051
aors=1051
```

For this example we have used the extension 1051 to give you an idea.
After you have set the new settings you'll need to restart your Asterisk with the following command.

```
systemctl restart asterisk
```

# I need help with my Asterisk 18

Need help with your Asterisk, or have any questions. 
You can contact us directly through our Asterisk cloud homepage on www.sipwebclient.com.





