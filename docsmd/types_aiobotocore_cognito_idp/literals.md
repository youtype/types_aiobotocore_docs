# Literals

> [Index](../README.md) > [CognitoIdentityProvider](./README.md) > Literals

!!! note ""

    Auto-generated documentation for [CognitoIdentityProvider](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider)
    type annotations stubs module [types-aiobotocore-cognito-idp](https://pypi.org/project/types-aiobotocore-cognito-idp/).

## AccountTakeoverEventActionTypeType

```python
# AccountTakeoverEventActionTypeType usage example

from types_aiobotocore_cognito_idp.literals import AccountTakeoverEventActionTypeType

def get_value() -> AccountTakeoverEventActionTypeType:
    return "BLOCK"
```

```python
# AccountTakeoverEventActionTypeType definition

AccountTakeoverEventActionTypeType = Literal[
    "BLOCK",
    "MFA_IF_CONFIGURED",
    "MFA_REQUIRED",
    "NO_ACTION",
]
```
## AdminListGroupsForUserPaginatorName

```python
# AdminListGroupsForUserPaginatorName usage example

from types_aiobotocore_cognito_idp.literals import AdminListGroupsForUserPaginatorName

def get_value() -> AdminListGroupsForUserPaginatorName:
    return "admin_list_groups_for_user"
```

```python
# AdminListGroupsForUserPaginatorName definition

AdminListGroupsForUserPaginatorName = Literal[
    "admin_list_groups_for_user",
]
```
## AdminListUserAuthEventsPaginatorName

```python
# AdminListUserAuthEventsPaginatorName usage example

from types_aiobotocore_cognito_idp.literals import AdminListUserAuthEventsPaginatorName

def get_value() -> AdminListUserAuthEventsPaginatorName:
    return "admin_list_user_auth_events"
```

```python
# AdminListUserAuthEventsPaginatorName definition

AdminListUserAuthEventsPaginatorName = Literal[
    "admin_list_user_auth_events",
]
```
## AdvancedSecurityModeTypeType

```python
# AdvancedSecurityModeTypeType usage example

from types_aiobotocore_cognito_idp.literals import AdvancedSecurityModeTypeType

def get_value() -> AdvancedSecurityModeTypeType:
    return "AUDIT"
```

```python
# AdvancedSecurityModeTypeType definition

AdvancedSecurityModeTypeType = Literal[
    "AUDIT",
    "ENFORCED",
    "OFF",
]
```
## AliasAttributeTypeType

```python
# AliasAttributeTypeType usage example

from types_aiobotocore_cognito_idp.literals import AliasAttributeTypeType

def get_value() -> AliasAttributeTypeType:
    return "email"
```

```python
# AliasAttributeTypeType definition

AliasAttributeTypeType = Literal[
    "email",
    "phone_number",
    "preferred_username",
]
```
## AttributeDataTypeType

```python
# AttributeDataTypeType usage example

from types_aiobotocore_cognito_idp.literals import AttributeDataTypeType

def get_value() -> AttributeDataTypeType:
    return "Boolean"
```

```python
# AttributeDataTypeType definition

AttributeDataTypeType = Literal[
    "Boolean",
    "DateTime",
    "Number",
    "String",
]
```
## AuthFlowTypeType

```python
# AuthFlowTypeType usage example

from types_aiobotocore_cognito_idp.literals import AuthFlowTypeType

def get_value() -> AuthFlowTypeType:
    return "ADMIN_NO_SRP_AUTH"
```

```python
# AuthFlowTypeType definition

AuthFlowTypeType = Literal[
    "ADMIN_NO_SRP_AUTH",
    "ADMIN_USER_PASSWORD_AUTH",
    "CUSTOM_AUTH",
    "REFRESH_TOKEN",
    "REFRESH_TOKEN_AUTH",
    "USER_PASSWORD_AUTH",
    "USER_SRP_AUTH",
]
```
## ChallengeNameType

```python
# ChallengeNameType usage example

from types_aiobotocore_cognito_idp.literals import ChallengeNameType

def get_value() -> ChallengeNameType:
    return "Mfa"
```

```python
# ChallengeNameType definition

ChallengeNameType = Literal[
    "Mfa",
    "Password",
]
```
## ChallengeNameTypeType

```python
# ChallengeNameTypeType usage example

from types_aiobotocore_cognito_idp.literals import ChallengeNameTypeType

def get_value() -> ChallengeNameTypeType:
    return "ADMIN_NO_SRP_AUTH"
```

```python
# ChallengeNameTypeType definition

ChallengeNameTypeType = Literal[
    "ADMIN_NO_SRP_AUTH",
    "CUSTOM_CHALLENGE",
    "DEVICE_PASSWORD_VERIFIER",
    "DEVICE_SRP_AUTH",
    "MFA_SETUP",
    "NEW_PASSWORD_REQUIRED",
    "PASSWORD_VERIFIER",
    "SELECT_MFA_TYPE",
    "SMS_MFA",
    "SOFTWARE_TOKEN_MFA",
]
```
## ChallengeResponseType

```python
# ChallengeResponseType usage example

from types_aiobotocore_cognito_idp.literals import ChallengeResponseType

def get_value() -> ChallengeResponseType:
    return "Failure"
```

```python
# ChallengeResponseType definition

ChallengeResponseType = Literal[
    "Failure",
    "Success",
]
```
## CompromisedCredentialsEventActionTypeType

```python
# CompromisedCredentialsEventActionTypeType usage example

from types_aiobotocore_cognito_idp.literals import CompromisedCredentialsEventActionTypeType

def get_value() -> CompromisedCredentialsEventActionTypeType:
    return "BLOCK"
```

```python
# CompromisedCredentialsEventActionTypeType definition

CompromisedCredentialsEventActionTypeType = Literal[
    "BLOCK",
    "NO_ACTION",
]
```
## CustomEmailSenderLambdaVersionTypeType

```python
# CustomEmailSenderLambdaVersionTypeType usage example

from types_aiobotocore_cognito_idp.literals import CustomEmailSenderLambdaVersionTypeType

def get_value() -> CustomEmailSenderLambdaVersionTypeType:
    return "V1_0"
```

```python
# CustomEmailSenderLambdaVersionTypeType definition

CustomEmailSenderLambdaVersionTypeType = Literal[
    "V1_0",
]
```
## CustomSMSSenderLambdaVersionTypeType

```python
# CustomSMSSenderLambdaVersionTypeType usage example

from types_aiobotocore_cognito_idp.literals import CustomSMSSenderLambdaVersionTypeType

def get_value() -> CustomSMSSenderLambdaVersionTypeType:
    return "V1_0"
```

```python
# CustomSMSSenderLambdaVersionTypeType definition

CustomSMSSenderLambdaVersionTypeType = Literal[
    "V1_0",
]
```
## DefaultEmailOptionTypeType

```python
# DefaultEmailOptionTypeType usage example

from types_aiobotocore_cognito_idp.literals import DefaultEmailOptionTypeType

def get_value() -> DefaultEmailOptionTypeType:
    return "CONFIRM_WITH_CODE"
```

```python
# DefaultEmailOptionTypeType definition

DefaultEmailOptionTypeType = Literal[
    "CONFIRM_WITH_CODE",
    "CONFIRM_WITH_LINK",
]
```
## DeletionProtectionTypeType

```python
# DeletionProtectionTypeType usage example

from types_aiobotocore_cognito_idp.literals import DeletionProtectionTypeType

def get_value() -> DeletionProtectionTypeType:
    return "ACTIVE"
```

```python
# DeletionProtectionTypeType definition

DeletionProtectionTypeType = Literal[
    "ACTIVE",
    "INACTIVE",
]
```
## DeliveryMediumTypeType

```python
# DeliveryMediumTypeType usage example

from types_aiobotocore_cognito_idp.literals import DeliveryMediumTypeType

def get_value() -> DeliveryMediumTypeType:
    return "EMAIL"
```

```python
# DeliveryMediumTypeType definition

DeliveryMediumTypeType = Literal[
    "EMAIL",
    "SMS",
]
```
## DeviceRememberedStatusTypeType

```python
# DeviceRememberedStatusTypeType usage example

from types_aiobotocore_cognito_idp.literals import DeviceRememberedStatusTypeType

def get_value() -> DeviceRememberedStatusTypeType:
    return "not_remembered"
```

```python
# DeviceRememberedStatusTypeType definition

DeviceRememberedStatusTypeType = Literal[
    "not_remembered",
    "remembered",
]
```
## DomainStatusTypeType

```python
# DomainStatusTypeType usage example

from types_aiobotocore_cognito_idp.literals import DomainStatusTypeType

def get_value() -> DomainStatusTypeType:
    return "ACTIVE"
```

```python
# DomainStatusTypeType definition

DomainStatusTypeType = Literal[
    "ACTIVE",
    "CREATING",
    "DELETING",
    "FAILED",
    "UPDATING",
]
```
## EmailSendingAccountTypeType

```python
# EmailSendingAccountTypeType usage example

from types_aiobotocore_cognito_idp.literals import EmailSendingAccountTypeType

def get_value() -> EmailSendingAccountTypeType:
    return "COGNITO_DEFAULT"
```

```python
# EmailSendingAccountTypeType definition

EmailSendingAccountTypeType = Literal[
    "COGNITO_DEFAULT",
    "DEVELOPER",
]
```
## EventFilterTypeType

```python
# EventFilterTypeType usage example

from types_aiobotocore_cognito_idp.literals import EventFilterTypeType

def get_value() -> EventFilterTypeType:
    return "PASSWORD_CHANGE"
```

```python
# EventFilterTypeType definition

EventFilterTypeType = Literal[
    "PASSWORD_CHANGE",
    "SIGN_IN",
    "SIGN_UP",
]
```
## EventResponseTypeType

```python
# EventResponseTypeType usage example

from types_aiobotocore_cognito_idp.literals import EventResponseTypeType

def get_value() -> EventResponseTypeType:
    return "Fail"
```

```python
# EventResponseTypeType definition

EventResponseTypeType = Literal[
    "Fail",
    "InProgress",
    "Pass",
]
```
## EventSourceNameType

```python
# EventSourceNameType usage example

from types_aiobotocore_cognito_idp.literals import EventSourceNameType

def get_value() -> EventSourceNameType:
    return "userNotification"
```

```python
# EventSourceNameType definition

EventSourceNameType = Literal[
    "userNotification",
]
```
## EventTypeType

```python
# EventTypeType usage example

from types_aiobotocore_cognito_idp.literals import EventTypeType

def get_value() -> EventTypeType:
    return "ForgotPassword"
```

```python
# EventTypeType definition

EventTypeType = Literal[
    "ForgotPassword",
    "PasswordChange",
    "ResendCode",
    "SignIn",
    "SignUp",
]
```
## ExplicitAuthFlowsTypeType

```python
# ExplicitAuthFlowsTypeType usage example

from types_aiobotocore_cognito_idp.literals import ExplicitAuthFlowsTypeType

def get_value() -> ExplicitAuthFlowsTypeType:
    return "ADMIN_NO_SRP_AUTH"
```

```python
# ExplicitAuthFlowsTypeType definition

ExplicitAuthFlowsTypeType = Literal[
    "ADMIN_NO_SRP_AUTH",
    "ALLOW_ADMIN_USER_PASSWORD_AUTH",
    "ALLOW_CUSTOM_AUTH",
    "ALLOW_REFRESH_TOKEN_AUTH",
    "ALLOW_USER_PASSWORD_AUTH",
    "ALLOW_USER_SRP_AUTH",
    "CUSTOM_AUTH_FLOW_ONLY",
    "USER_PASSWORD_AUTH",
]
```
## FeedbackValueTypeType

```python
# FeedbackValueTypeType usage example

from types_aiobotocore_cognito_idp.literals import FeedbackValueTypeType

def get_value() -> FeedbackValueTypeType:
    return "Invalid"
```

```python
# FeedbackValueTypeType definition

FeedbackValueTypeType = Literal[
    "Invalid",
    "Valid",
]
```
## IdentityProviderTypeTypeType

```python
# IdentityProviderTypeTypeType usage example

from types_aiobotocore_cognito_idp.literals import IdentityProviderTypeTypeType

def get_value() -> IdentityProviderTypeTypeType:
    return "Facebook"
```

```python
# IdentityProviderTypeTypeType definition

IdentityProviderTypeTypeType = Literal[
    "Facebook",
    "Google",
    "LoginWithAmazon",
    "OIDC",
    "SAML",
    "SignInWithApple",
]
```
## ListGroupsPaginatorName

```python
# ListGroupsPaginatorName usage example

from types_aiobotocore_cognito_idp.literals import ListGroupsPaginatorName

def get_value() -> ListGroupsPaginatorName:
    return "list_groups"
```

```python
# ListGroupsPaginatorName definition

ListGroupsPaginatorName = Literal[
    "list_groups",
]
```
## ListIdentityProvidersPaginatorName

```python
# ListIdentityProvidersPaginatorName usage example

from types_aiobotocore_cognito_idp.literals import ListIdentityProvidersPaginatorName

def get_value() -> ListIdentityProvidersPaginatorName:
    return "list_identity_providers"
```

```python
# ListIdentityProvidersPaginatorName definition

ListIdentityProvidersPaginatorName = Literal[
    "list_identity_providers",
]
```
## ListResourceServersPaginatorName

```python
# ListResourceServersPaginatorName usage example

from types_aiobotocore_cognito_idp.literals import ListResourceServersPaginatorName

def get_value() -> ListResourceServersPaginatorName:
    return "list_resource_servers"
```

```python
# ListResourceServersPaginatorName definition

ListResourceServersPaginatorName = Literal[
    "list_resource_servers",
]
```
## ListUserPoolClientsPaginatorName

```python
# ListUserPoolClientsPaginatorName usage example

from types_aiobotocore_cognito_idp.literals import ListUserPoolClientsPaginatorName

def get_value() -> ListUserPoolClientsPaginatorName:
    return "list_user_pool_clients"
```

```python
# ListUserPoolClientsPaginatorName definition

ListUserPoolClientsPaginatorName = Literal[
    "list_user_pool_clients",
]
```
## ListUserPoolsPaginatorName

```python
# ListUserPoolsPaginatorName usage example

from types_aiobotocore_cognito_idp.literals import ListUserPoolsPaginatorName

def get_value() -> ListUserPoolsPaginatorName:
    return "list_user_pools"
```

```python
# ListUserPoolsPaginatorName definition

ListUserPoolsPaginatorName = Literal[
    "list_user_pools",
]
```
## ListUsersInGroupPaginatorName

```python
# ListUsersInGroupPaginatorName usage example

from types_aiobotocore_cognito_idp.literals import ListUsersInGroupPaginatorName

def get_value() -> ListUsersInGroupPaginatorName:
    return "list_users_in_group"
```

```python
# ListUsersInGroupPaginatorName definition

ListUsersInGroupPaginatorName = Literal[
    "list_users_in_group",
]
```
## ListUsersPaginatorName

```python
# ListUsersPaginatorName usage example

from types_aiobotocore_cognito_idp.literals import ListUsersPaginatorName

def get_value() -> ListUsersPaginatorName:
    return "list_users"
```

```python
# ListUsersPaginatorName definition

ListUsersPaginatorName = Literal[
    "list_users",
]
```
## LogLevelType

```python
# LogLevelType usage example

from types_aiobotocore_cognito_idp.literals import LogLevelType

def get_value() -> LogLevelType:
    return "ERROR"
```

```python
# LogLevelType definition

LogLevelType = Literal[
    "ERROR",
]
```
## MessageActionTypeType

```python
# MessageActionTypeType usage example

from types_aiobotocore_cognito_idp.literals import MessageActionTypeType

def get_value() -> MessageActionTypeType:
    return "RESEND"
```

```python
# MessageActionTypeType definition

MessageActionTypeType = Literal[
    "RESEND",
    "SUPPRESS",
]
```
## OAuthFlowTypeType

```python
# OAuthFlowTypeType usage example

from types_aiobotocore_cognito_idp.literals import OAuthFlowTypeType

def get_value() -> OAuthFlowTypeType:
    return "client_credentials"
```

```python
# OAuthFlowTypeType definition

OAuthFlowTypeType = Literal[
    "client_credentials",
    "code",
    "implicit",
]
```
## PreventUserExistenceErrorTypesType

```python
# PreventUserExistenceErrorTypesType usage example

from types_aiobotocore_cognito_idp.literals import PreventUserExistenceErrorTypesType

def get_value() -> PreventUserExistenceErrorTypesType:
    return "ENABLED"
```

```python
# PreventUserExistenceErrorTypesType definition

PreventUserExistenceErrorTypesType = Literal[
    "ENABLED",
    "LEGACY",
]
```
## RecoveryOptionNameTypeType

```python
# RecoveryOptionNameTypeType usage example

from types_aiobotocore_cognito_idp.literals import RecoveryOptionNameTypeType

def get_value() -> RecoveryOptionNameTypeType:
    return "admin_only"
```

```python
# RecoveryOptionNameTypeType definition

RecoveryOptionNameTypeType = Literal[
    "admin_only",
    "verified_email",
    "verified_phone_number",
]
```
## RiskDecisionTypeType

```python
# RiskDecisionTypeType usage example

from types_aiobotocore_cognito_idp.literals import RiskDecisionTypeType

def get_value() -> RiskDecisionTypeType:
    return "AccountTakeover"
```

```python
# RiskDecisionTypeType definition

RiskDecisionTypeType = Literal[
    "AccountTakeover",
    "Block",
    "NoRisk",
]
```
## RiskLevelTypeType

```python
# RiskLevelTypeType usage example

from types_aiobotocore_cognito_idp.literals import RiskLevelTypeType

def get_value() -> RiskLevelTypeType:
    return "High"
```

```python
# RiskLevelTypeType definition

RiskLevelTypeType = Literal[
    "High",
    "Low",
    "Medium",
]
```
## StatusTypeType

```python
# StatusTypeType usage example

from types_aiobotocore_cognito_idp.literals import StatusTypeType

def get_value() -> StatusTypeType:
    return "Disabled"
```

```python
# StatusTypeType definition

StatusTypeType = Literal[
    "Disabled",
    "Enabled",
]
```
## TimeUnitsTypeType

```python
# TimeUnitsTypeType usage example

from types_aiobotocore_cognito_idp.literals import TimeUnitsTypeType

def get_value() -> TimeUnitsTypeType:
    return "days"
```

```python
# TimeUnitsTypeType definition

TimeUnitsTypeType = Literal[
    "days",
    "hours",
    "minutes",
    "seconds",
]
```
## UserImportJobStatusTypeType

```python
# UserImportJobStatusTypeType usage example

from types_aiobotocore_cognito_idp.literals import UserImportJobStatusTypeType

def get_value() -> UserImportJobStatusTypeType:
    return "Created"
```

```python
# UserImportJobStatusTypeType definition

UserImportJobStatusTypeType = Literal[
    "Created",
    "Expired",
    "Failed",
    "InProgress",
    "Pending",
    "Stopped",
    "Stopping",
    "Succeeded",
]
```
## UserPoolMfaTypeType

```python
# UserPoolMfaTypeType usage example

from types_aiobotocore_cognito_idp.literals import UserPoolMfaTypeType

def get_value() -> UserPoolMfaTypeType:
    return "OFF"
```

```python
# UserPoolMfaTypeType definition

UserPoolMfaTypeType = Literal[
    "OFF",
    "ON",
    "OPTIONAL",
]
```
## UserStatusTypeType

```python
# UserStatusTypeType usage example

from types_aiobotocore_cognito_idp.literals import UserStatusTypeType

def get_value() -> UserStatusTypeType:
    return "ARCHIVED"
```

```python
# UserStatusTypeType definition

UserStatusTypeType = Literal[
    "ARCHIVED",
    "COMPROMISED",
    "CONFIRMED",
    "FORCE_CHANGE_PASSWORD",
    "RESET_REQUIRED",
    "UNCONFIRMED",
    "UNKNOWN",
]
```
## UsernameAttributeTypeType

```python
# UsernameAttributeTypeType usage example

from types_aiobotocore_cognito_idp.literals import UsernameAttributeTypeType

def get_value() -> UsernameAttributeTypeType:
    return "email"
```

```python
# UsernameAttributeTypeType definition

UsernameAttributeTypeType = Literal[
    "email",
    "phone_number",
]
```
## VerifiedAttributeTypeType

```python
# VerifiedAttributeTypeType usage example

from types_aiobotocore_cognito_idp.literals import VerifiedAttributeTypeType

def get_value() -> VerifiedAttributeTypeType:
    return "email"
```

```python
# VerifiedAttributeTypeType definition

VerifiedAttributeTypeType = Literal[
    "email",
    "phone_number",
]
```
## VerifySoftwareTokenResponseTypeType

```python
# VerifySoftwareTokenResponseTypeType usage example

from types_aiobotocore_cognito_idp.literals import VerifySoftwareTokenResponseTypeType

def get_value() -> VerifySoftwareTokenResponseTypeType:
    return "ERROR"
```

```python
# VerifySoftwareTokenResponseTypeType definition

VerifySoftwareTokenResponseTypeType = Literal[
    "ERROR",
    "SUCCESS",
]
```
## CognitoIdentityProviderServiceName

```python
# CognitoIdentityProviderServiceName usage example

from types_aiobotocore_cognito_idp.literals import CognitoIdentityProviderServiceName

def get_value() -> CognitoIdentityProviderServiceName:
    return "cognito-idp"
```

```python
# CognitoIdentityProviderServiceName definition

CognitoIdentityProviderServiceName = Literal[
    "cognito-idp",
]
```
## ServiceName

```python
# ServiceName usage example

from types_aiobotocore_cognito_idp.literals import ServiceName

def get_value() -> ServiceName:
    return "accessanalyzer"
```

```python
# ServiceName definition

ServiceName = Literal[
    "accessanalyzer",
    "account",
    "acm",
    "acm-pca",
    "alexaforbusiness",
    "amp",
    "amplify",
    "amplifybackend",
    "amplifyuibuilder",
    "apigateway",
    "apigatewaymanagementapi",
    "apigatewayv2",
    "appconfig",
    "appconfigdata",
    "appfabric",
    "appflow",
    "appintegrations",
    "application-autoscaling",
    "application-insights",
    "applicationcostprofiler",
    "appmesh",
    "apprunner",
    "appstream",
    "appsync",
    "arc-zonal-shift",
    "athena",
    "auditmanager",
    "autoscaling",
    "autoscaling-plans",
    "backup",
    "backup-gateway",
    "backupstorage",
    "batch",
    "billingconductor",
    "braket",
    "budgets",
    "ce",
    "chime",
    "chime-sdk-identity",
    "chime-sdk-media-pipelines",
    "chime-sdk-meetings",
    "chime-sdk-messaging",
    "chime-sdk-voice",
    "cleanrooms",
    "cloud9",
    "cloudcontrol",
    "clouddirectory",
    "cloudformation",
    "cloudfront",
    "cloudhsm",
    "cloudhsmv2",
    "cloudsearch",
    "cloudsearchdomain",
    "cloudtrail",
    "cloudtrail-data",
    "cloudwatch",
    "codeartifact",
    "codebuild",
    "codecatalyst",
    "codecommit",
    "codedeploy",
    "codeguru-reviewer",
    "codeguru-security",
    "codeguruprofiler",
    "codepipeline",
    "codestar",
    "codestar-connections",
    "codestar-notifications",
    "cognito-identity",
    "cognito-idp",
    "cognito-sync",
    "comprehend",
    "comprehendmedical",
    "compute-optimizer",
    "config",
    "connect",
    "connect-contact-lens",
    "connectcampaigns",
    "connectcases",
    "connectparticipant",
    "controltower",
    "cur",
    "customer-profiles",
    "databrew",
    "dataexchange",
    "datapipeline",
    "datasync",
    "dax",
    "detective",
    "devicefarm",
    "devops-guru",
    "directconnect",
    "discovery",
    "dlm",
    "dms",
    "docdb",
    "docdb-elastic",
    "drs",
    "ds",
    "dynamodb",
    "dynamodbstreams",
    "ebs",
    "ec2",
    "ec2-instance-connect",
    "ecr",
    "ecr-public",
    "ecs",
    "efs",
    "eks",
    "elastic-inference",
    "elasticache",
    "elasticbeanstalk",
    "elastictranscoder",
    "elb",
    "elbv2",
    "emr",
    "emr-containers",
    "emr-serverless",
    "entityresolution",
    "es",
    "events",
    "evidently",
    "finspace",
    "finspace-data",
    "firehose",
    "fis",
    "fms",
    "forecast",
    "forecastquery",
    "frauddetector",
    "fsx",
    "gamelift",
    "gamesparks",
    "glacier",
    "globalaccelerator",
    "glue",
    "grafana",
    "greengrass",
    "greengrassv2",
    "groundstation",
    "guardduty",
    "health",
    "healthlake",
    "honeycode",
    "iam",
    "identitystore",
    "imagebuilder",
    "importexport",
    "inspector",
    "inspector2",
    "internetmonitor",
    "iot",
    "iot-data",
    "iot-jobs-data",
    "iot-roborunner",
    "iot1click-devices",
    "iot1click-projects",
    "iotanalytics",
    "iotdeviceadvisor",
    "iotevents",
    "iotevents-data",
    "iotfleethub",
    "iotfleetwise",
    "iotsecuretunneling",
    "iotsitewise",
    "iotthingsgraph",
    "iottwinmaker",
    "iotwireless",
    "ivs",
    "ivs-realtime",
    "ivschat",
    "kafka",
    "kafkaconnect",
    "kendra",
    "kendra-ranking",
    "keyspaces",
    "kinesis",
    "kinesis-video-archived-media",
    "kinesis-video-media",
    "kinesis-video-signaling",
    "kinesis-video-webrtc-storage",
    "kinesisanalytics",
    "kinesisanalyticsv2",
    "kinesisvideo",
    "kms",
    "lakeformation",
    "lambda",
    "lex-models",
    "lex-runtime",
    "lexv2-models",
    "lexv2-runtime",
    "license-manager",
    "license-manager-linux-subscriptions",
    "license-manager-user-subscriptions",
    "lightsail",
    "location",
    "logs",
    "lookoutequipment",
    "lookoutmetrics",
    "lookoutvision",
    "m2",
    "machinelearning",
    "macie",
    "macie2",
    "managedblockchain",
    "managedblockchain-query",
    "marketplace-catalog",
    "marketplace-entitlement",
    "marketplacecommerceanalytics",
    "mediaconnect",
    "mediaconvert",
    "medialive",
    "mediapackage",
    "mediapackage-vod",
    "mediapackagev2",
    "mediastore",
    "mediastore-data",
    "mediatailor",
    "medical-imaging",
    "memorydb",
    "meteringmarketplace",
    "mgh",
    "mgn",
    "migration-hub-refactor-spaces",
    "migrationhub-config",
    "migrationhuborchestrator",
    "migrationhubstrategy",
    "mobile",
    "mq",
    "mturk",
    "mwaa",
    "neptune",
    "network-firewall",
    "networkmanager",
    "nimble",
    "oam",
    "omics",
    "opensearch",
    "opensearchserverless",
    "opsworks",
    "opsworkscm",
    "organizations",
    "osis",
    "outposts",
    "panorama",
    "payment-cryptography",
    "payment-cryptography-data",
    "personalize",
    "personalize-events",
    "personalize-runtime",
    "pi",
    "pinpoint",
    "pinpoint-email",
    "pinpoint-sms-voice",
    "pinpoint-sms-voice-v2",
    "pipes",
    "polly",
    "pricing",
    "privatenetworks",
    "proton",
    "qldb",
    "qldb-session",
    "quicksight",
    "ram",
    "rbin",
    "rds",
    "rds-data",
    "redshift",
    "redshift-data",
    "redshift-serverless",
    "rekognition",
    "resiliencehub",
    "resource-explorer-2",
    "resource-groups",
    "resourcegroupstaggingapi",
    "robomaker",
    "rolesanywhere",
    "route53",
    "route53-recovery-cluster",
    "route53-recovery-control-config",
    "route53-recovery-readiness",
    "route53domains",
    "route53resolver",
    "rum",
    "s3",
    "s3control",
    "s3outposts",
    "sagemaker",
    "sagemaker-a2i-runtime",
    "sagemaker-edge",
    "sagemaker-featurestore-runtime",
    "sagemaker-geospatial",
    "sagemaker-metrics",
    "sagemaker-runtime",
    "savingsplans",
    "scheduler",
    "schemas",
    "sdb",
    "secretsmanager",
    "securityhub",
    "securitylake",
    "serverlessrepo",
    "service-quotas",
    "servicecatalog",
    "servicecatalog-appregistry",
    "servicediscovery",
    "ses",
    "sesv2",
    "shield",
    "signer",
    "simspaceweaver",
    "sms",
    "sms-voice",
    "snow-device-management",
    "snowball",
    "sns",
    "sqs",
    "ssm",
    "ssm-contacts",
    "ssm-incidents",
    "ssm-sap",
    "sso",
    "sso-admin",
    "sso-oidc",
    "stepfunctions",
    "storagegateway",
    "sts",
    "support",
    "support-app",
    "swf",
    "synthetics",
    "textract",
    "timestream-query",
    "timestream-write",
    "tnb",
    "transcribe",
    "transfer",
    "translate",
    "verifiedpermissions",
    "voice-id",
    "vpc-lattice",
    "waf",
    "waf-regional",
    "wafv2",
    "wellarchitected",
    "wisdom",
    "workdocs",
    "worklink",
    "workmail",
    "workmailmessageflow",
    "workspaces",
    "workspaces-web",
    "xray",
]
```
## ResourceServiceName

```python
# ResourceServiceName usage example

from types_aiobotocore_cognito_idp.literals import ResourceServiceName

def get_value() -> ResourceServiceName:
    return "cloudformation"
```

```python
# ResourceServiceName definition

ResourceServiceName = Literal[
    "cloudformation",
    "cloudwatch",
    "dynamodb",
    "ec2",
    "glacier",
    "iam",
    "opsworks",
    "s3",
    "sns",
    "sqs",
]
```
## PaginatorName

```python
# PaginatorName usage example

from types_aiobotocore_cognito_idp.literals import PaginatorName

def get_value() -> PaginatorName:
    return "admin_list_groups_for_user"
```

```python
# PaginatorName definition

PaginatorName = Literal[
    "admin_list_groups_for_user",
    "admin_list_user_auth_events",
    "list_groups",
    "list_identity_providers",
    "list_resource_servers",
    "list_user_pool_clients",
    "list_user_pools",
    "list_users",
    "list_users_in_group",
]
```
## RegionName

```python
# RegionName usage example

from types_aiobotocore_cognito_idp.literals import RegionName

def get_value() -> RegionName:
    return "ap-northeast-1"
```

```python
# RegionName definition

RegionName = Literal[
    "ap-northeast-1",
    "ap-northeast-2",
    "ap-south-1",
    "ap-southeast-1",
    "ap-southeast-2",
    "ca-central-1",
    "eu-central-1",
    "eu-north-1",
    "eu-south-1",
    "eu-west-1",
    "eu-west-2",
    "eu-west-3",
    "me-south-1",
    "sa-east-1",
    "us-east-1",
    "us-east-2",
    "us-west-1",
    "us-west-2",
]
```
