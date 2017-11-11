# Jenkins

- build on trigger

```shell
#!/bin/bash
set -e
set -x

CRUMB=$(curl -s -u "uid:token" 'JENKINS_URL/crumbIssuer/api/xml?xpath=concat(//crumbRequestField,":",//crumb)') ;
curl -X POST -u "uid:token" -H "$CRUMB" "JENKINS_URL/job/shop.fengbao.com/build?token=nideyida"%