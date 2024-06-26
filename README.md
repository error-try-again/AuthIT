# AuthIT

This project is a comprehensive and highly specialized system for managing, maintaining & distributing complex multi-stack architecture within AWS Cloud used for managing and orchestrating Cognito, Amplify, and many other services.    

*This script assumes you have already configured Access Keys/AWS CLI.*

## Building the project

### Step 1. 
Create a DNSSEC policy by modifying create_dnssec_policy_json.sh & updating the following policy fields.
These will likely be the same for your particular user.

principal_arn="arn:aws:iam::YOUR_PRINCIPAL_ID:root"
source_account="YOUR_SRC_ACCOUNT_NUMBER"

principal_arn="arn:aws:iam::222222222222:root"
source_account="222222222222"

### Step 2. 
`chmod +x aws_setup.sh`
`./aws_setup.sh`


### *Reference Links*

#### *Amplify auth headless schema configuration:*

[1] https://docs.amplify.aws/cli/usage/headless/#optional-ide-setup-for-headless-development

[2] https://github.com/aws-amplify/amplify-cli/blob/main/packages/amplify-headless-interface/schemas/auth/2/AddAuthRequest.schema.json

[3] https://github.com/aws-amplify/amplify-cli/blob/main/packages/amplify-headless-interface/src/interface/auth/add.ts

### *Issues*

##### Missing config\local-env-info.json error (requires amplify pull)
[1] https://github.com/aws-amplify/amplify-cli/issues/11245
