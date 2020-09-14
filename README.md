# awscli-keepalive
AWS CLI keeping alive for gitlab-ci

## Gitlab CLI Usage example :
```
variables:
  REGION: eu-west-1
  AWS_ACCOUNT: XXXXXXXX

default:
  before_script:
    - export AWS_ACCESS_KEY_ID=$AWS_ACCESS_KEY_ID
    - export AWS_SECRET_ACCESS_KEY=$AWS_SECRET_ACCESS_KEY

dev_deploy_codebuild:
  image: dropteam/awscli-keepalive
  script:
    - aws help
```
