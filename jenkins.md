# Jenkins

- build on trigger

```shell
#!/bin/bash
set -e
set -x

CRUMB=$(curl -s -u "{UID:TOKEN}" '{JENKINS_URL}/crumbIssuer/api/xml?xpath=concat(//crumbRequestField,":",//crumb)') ;
curl -X POST -u "{UID:TOKEN}" -H "$CRUMB" "{JENKINS_URL}/job/{JOB_NAME}/build?token=TRIGGER_TOKEN"
