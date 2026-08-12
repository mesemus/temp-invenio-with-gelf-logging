# GELF test

Welcome to your InvenioRDM instance.

after the services setup, get the log from the graylog container. It will say something like:

```
========================================================================================================

It seems you are starting Graylog for the first time. To set up a fresh install, a setup interface has
been started. You must log in to it to perform the initial configuration and continue.

Initial configuration is accessible at 0.0.0.0:9000, with username 'admin' and password 'oxhOtpEypw'.
Try clicking on http://admin:oxhOtpEypw@0.0.0.0:9000

========================================================================================================
```

Go there and finish the initial configuration. After that, log in again to graylog with username 'admin' and password 'changeme'.
Go to system/inputs and configure the GELF TCP input on port 12201. Then run invenio-cli run and create a record.
