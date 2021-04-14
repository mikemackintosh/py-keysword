# Keysword
Automated method of retrieving Filevault2 keys from JAMF

### Usage:

There are two search methods for returning a filevault key, using a computer ID or a computer name:

    python3 keysword.py -id <jss_id>
    python3 keysword.py -name <computer_name>

### Configuring

There are three fields required to be exported in your environment in order to authenticate:

  - `JAMF_HOST`: Should be the URL to the JAMF host, ex: `https://examplejss.com`
  - `JAMF_USERNAME`: Should be the username to the JAMF host
  - `JAMF_PASSWORD`: Should be the password to the JAMF host

Additionally, there is a dependency on the `requests` library, simply use pip or [pipenv](http://pipenv.org/) to install:

``` {.sourceCode .bash}
$ pip install requests
```
