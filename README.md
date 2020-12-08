# Asterisk 18 Extensions

On this GitHub page, you can find the basic configuration settings for an Asterisk 18 server with 50 extensions. 

Requirements

- Linux Server
- Asterisk 18 installed

# How to setup Extensions for Asterisk 18

To set up the extensions for your Asterisk server do the following:

- Add the GitHub files to your Asterisk directory ["etc/asterisk"]
- Update the pjsip.conf file with; [your server public ip], [your server private ip], [the extension passwords]

After this, restart your Asterisk 18

```
systemctl restart asterisk
```

The extensions for your Asterisk 18 has now been installed.

# How many extensions have we added?

We have added the extension numbers 1000 till 1050.

# How to add more extensions

Adding more extensions to the configuration files can be done by adding the following lines to the pjsip.conf [etc/asterisk/pjsip.conf] file.

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

For this example, we have used extension 1051.
After you have set the new settings you'll need to restart your Asterisk.

```
systemctl restart asterisk
```

# I need help with my Asterisk 18

Need help with your Asterisk, or have any questions. 
You can contact us directly through our Asterisk Cloud homepage on www.sipwebclient.com.






