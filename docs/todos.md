# Best practices
1. Never use personal account
2. Activate billing access for IAM users
3. Setting up a password policy
4. Endpoints


1. Use cloudshell
2. Setting up IAM users and groups
3. https://workshop-aws-account-setup.fstehle.com/master-account/iam-users/

```
aws cloudformation deploy --no-fail-on-empty-changeset \
--template-file iam-users.yml --stack-name iam-users \
--capabilities CAPABILITY_NAMED_IAM --region sa-east-1 \
--parameter-overrides UserNameParameter=<user@example.com>
```

1. Assigning an MFA device for the created users
2. Enabling Console access for the created users
3. Logging to the AWS console

**Nao é possível criar ident center via cloudformation**
**Usar então a criação de usuário admin e organizações e contas usando cloudformation para documentar os passos**
Após criar na mão
1. Customize AWS access portal URL
2. Prevent creation of new account instances of IAM Identity Center
3. Enable Multi-factor authentication
4. 
Criar organização
1. criar arquivo organization.yaml
2. usar cloud shell para aplicar

```
aws cloudformation deploy --no-fail-on-empty-changeset \
--template-file organization.yaml --stack-name organization \
--capabilities CAPABILITY_NAMED_IAM --region sa-east-1
```

CONTINUAR AQUI
https://workshop-aws-account-setup.fstehle.com/master-account/aws-organization/






https://passwordless.id/usage/openid

https://docs.aws.amazon.com/organizations/latest/userguide/orgs_best-practices.html

Use a group email address for root accounts

# Recomended OUs
https://docs.aws.amazon.com/whitepapers/latest/organizing-your-aws-environment/recommended-ous-and-accounts.html

## Relação com os pilares
https://docs.aws.amazon.com/whitepapers/latest/organizing-your-aws-environment/appendix-a-relation-to-aws-well-architected.html

## Workshops
https://catalog.workshops.aws/control-tower/en-US

https://controltower.aws-management.tools/

https://getstarted.awsworkshop.io/00-intro/02-intended-audience.html

https://catalog.workshops.aws/cfn101/en-US/introduction


https://www.image-processing.serverlessworkshops.io/

https://v1.cicd.serverlessworkshops.io/

https://application-catalog.serverlessworkshops.io/040_pipeline/

https://chalice-workshop.readthedocs.io/en/latest/

https://github.com/aws-samples/aws-modern-application-workshop/tree/python-cdk

https://webapp.serverlessworkshops.io/

https://github.com/aws-samples/arc325-multiple-accounts-workshop/blob/master/docs/create-orgs.md
https://github.com/aws-samples/aws-serverless-workshops

https://catalog.us-east-1.prod.workshops.aws/workshops/fc36cb5a-de1b-403f-84dd-cc824390c548/en-US

https://github.com/aws-samples/aws-security-odyssey/tree/master

https://wellarchitectedlabs.com/

https://github.com/aws-samples/arc325-multiple-accounts-workshop

https://awsworkshop.io/categories/organizations/

https://catalog.us-east-1.prod.workshops.aws/workshops/d3f60827-89f2-46a8-9be7-6e7185bd7665/en-US

https://mng.workshop.aws/

https://github.com/hamidnazari/workshop-aws-org-scp

https://awssecworkshops.com/

https://getstarted.awsworkshop.io/
