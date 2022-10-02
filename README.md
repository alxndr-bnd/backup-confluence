# backup-confluence

This project is for perform regular backup of your Confluence.
You need the script `Confluence-backup.sh`. It is a bit
changed https://bitbucket.org/atlassianlabs/automatic-cloud-backup/src/master/

What is changed: variable moved to another file, see below about `api-token.sh`

Add a file `api-token.sh` in same directory with desired folder name for
results, your email, API token & Confluence instance URL. Here is an example of
the file:

```
#!/bin/bash

folder="result"
email="xxx@yyy.zzz"
token="abcd"
instance="yyy.atlassian.net"
```

The file 'api-token' MUST NOT upload to GitHub for security reasons, to prevent leak of API
token, so exclude from git
