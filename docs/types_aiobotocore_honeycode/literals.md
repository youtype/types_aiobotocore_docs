<a id="literals-for-aiobotocore-honeycode-module"></a>

# Literals for aiobotocore Honeycode module

> [Index](../README.md) > [Honeycode](./README.md) > Literals

Auto-generated documentation for
[Honeycode](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode)
type annotations stubs module
[types-aiobotocore-honeycode](https://pypi.org/project/types-aiobotocore-honeycode/).

- [Literals for aiobotocore Honeycode module](#literals-for-aiobotocore-honeycode-module)
  - [ErrorCodeType](#errorcodetype)
  - [FormatType](#formattype)
  - [ImportDataCharacterEncodingType](#importdatacharacterencodingtype)
  - [ImportSourceDataFormatType](#importsourcedataformattype)
  - [ListTableColumnsPaginatorName](#listtablecolumnspaginatorname)
  - [ListTableRowsPaginatorName](#listtablerowspaginatorname)
  - [ListTablesPaginatorName](#listtablespaginatorname)
  - [QueryTableRowsPaginatorName](#querytablerowspaginatorname)
  - [TableDataImportJobStatusType](#tabledataimportjobstatustype)
  - [UpsertActionType](#upsertactiontype)
  - [HoneycodeServiceName](#honeycodeservicename)
  - [ServiceName](#servicename)
  - [ResourceServiceName](#resourceservicename)
  - [PaginatorName](#paginatorname)

<a id="errorcodetype"></a>

## ErrorCodeType

```python
from types_aiobotocore_honeycode.literals import ErrorCodeType
```

Values:

- `ACCESS_DENIED`
- `FILE_EMPTY_ERROR`
- `FILE_NOT_FOUND_ERROR`
- `FILE_PARSING_ERROR`
- `FILE_SIZE_LIMIT_ERROR`
- `INVALID_FILE_TYPE_ERROR`
- `INVALID_IMPORT_OPTIONS_ERROR`
- `INVALID_TABLE_COLUMN_ID_ERROR`
- `INVALID_TABLE_ID_ERROR`
- `INVALID_URL_ERROR`
- `RESOURCE_NOT_FOUND_ERROR`
- `SYSTEM_LIMIT_ERROR`
- `TABLE_NOT_FOUND_ERROR`
- `UNKNOWN_ERROR`

<a id="formattype"></a>

## FormatType

```python
from types_aiobotocore_honeycode.literals import FormatType
```

Values:

- `ACCOUNTING`
- `AUTO`
- `CONTACT`
- `CURRENCY`
- `DATE`
- `DATE_TIME`
- `NUMBER`
- `PERCENTAGE`
- `ROWLINK`
- `ROWSET`
- `TEXT`
- `TIME`

<a id="importdatacharacterencodingtype"></a>

## ImportDataCharacterEncodingType

```python
from types_aiobotocore_honeycode.literals import ImportDataCharacterEncodingType
```

Values:

- `ISO-8859-1`
- `US-ASCII`
- `UTF-16`
- `UTF-16BE`
- `UTF-16LE`
- `UTF-8`

<a id="importsourcedataformattype"></a>

## ImportSourceDataFormatType

```python
from types_aiobotocore_honeycode.literals import ImportSourceDataFormatType
```

Values:

- `DELIMITED_TEXT`

<a id="listtablecolumnspaginatorname"></a>

## ListTableColumnsPaginatorName

```python
from types_aiobotocore_honeycode.literals import ListTableColumnsPaginatorName
```

Values:

- `list_table_columns`

<a id="listtablerowspaginatorname"></a>

## ListTableRowsPaginatorName

```python
from types_aiobotocore_honeycode.literals import ListTableRowsPaginatorName
```

Values:

- `list_table_rows`

<a id="listtablespaginatorname"></a>

## ListTablesPaginatorName

```python
from types_aiobotocore_honeycode.literals import ListTablesPaginatorName
```

Values:

- `list_tables`

<a id="querytablerowspaginatorname"></a>

## QueryTableRowsPaginatorName

```python
from types_aiobotocore_honeycode.literals import QueryTableRowsPaginatorName
```

Values:

- `query_table_rows`

<a id="tabledataimportjobstatustype"></a>

## TableDataImportJobStatusType

```python
from types_aiobotocore_honeycode.literals import TableDataImportJobStatusType
```

Values:

- `COMPLETED`
- `FAILED`
- `IN_PROGRESS`
- `SUBMITTED`

<a id="upsertactiontype"></a>

## UpsertActionType

```python
from types_aiobotocore_honeycode.literals import UpsertActionType
```

Values:

- `APPENDED`
- `UPDATED`

<a id="honeycodeservicename"></a>

## HoneycodeServiceName

```python
from types_aiobotocore_honeycode.literals import HoneycodeServiceName
```

Values:

- `honeycode`

<a id="servicename"></a>

## ServiceName

```python
from types_aiobotocore_honeycode.literals import ServiceName
```

Values:

- `accessanalyzer`
- `account`
- `acm`
- `acm-pca`
- `alexaforbusiness`
- `amp`
- `amplify`
- `amplifybackend`
- `amplifyuibuilder`
- `apigateway`
- `apigatewaymanagementapi`
- `apigatewayv2`
- `appconfig`
- `appconfigdata`
- `appflow`
- `appintegrations`
- `application-autoscaling`
- `application-insights`
- `applicationcostprofiler`
- `appmesh`
- `apprunner`
- `appstream`
- `appsync`
- `athena`
- `auditmanager`
- `autoscaling`
- `autoscaling-plans`
- `backup`
- `backup-gateway`
- `batch`
- `billingconductor`
- `braket`
- `budgets`
- `ce`
- `chime`
- `chime-sdk-identity`
- `chime-sdk-meetings`
- `chime-sdk-messaging`
- `cloud9`
- `cloudcontrol`
- `clouddirectory`
- `cloudformation`
- `cloudfront`
- `cloudhsm`
- `cloudhsmv2`
- `cloudsearch`
- `cloudsearchdomain`
- `cloudtrail`
- `cloudwatch`
- `codeartifact`
- `codebuild`
- `codecommit`
- `codedeploy`
- `codeguru-reviewer`
- `codeguruprofiler`
- `codepipeline`
- `codestar`
- `codestar-connections`
- `codestar-notifications`
- `cognito-identity`
- `cognito-idp`
- `cognito-sync`
- `comprehend`
- `comprehendmedical`
- `compute-optimizer`
- `config`
- `connect`
- `connect-contact-lens`
- `connectparticipant`
- `cur`
- `customer-profiles`
- `databrew`
- `dataexchange`
- `datapipeline`
- `datasync`
- `dax`
- `detective`
- `devicefarm`
- `devops-guru`
- `directconnect`
- `discovery`
- `dlm`
- `dms`
- `docdb`
- `drs`
- `ds`
- `dynamodb`
- `dynamodbstreams`
- `ebs`
- `ec2`
- `ec2-instance-connect`
- `ecr`
- `ecr-public`
- `ecs`
- `efs`
- `eks`
- `elastic-inference`
- `elasticache`
- `elasticbeanstalk`
- `elastictranscoder`
- `elb`
- `elbv2`
- `emr`
- `emr-containers`
- `es`
- `events`
- `evidently`
- `finspace`
- `finspace-data`
- `firehose`
- `fis`
- `fms`
- `forecast`
- `forecastquery`
- `frauddetector`
- `fsx`
- `gamelift`
- `glacier`
- `globalaccelerator`
- `glue`
- `grafana`
- `greengrass`
- `greengrassv2`
- `groundstation`
- `guardduty`
- `health`
- `healthlake`
- `honeycode`
- `iam`
- `identitystore`
- `imagebuilder`
- `importexport`
- `inspector`
- `inspector2`
- `iot`
- `iot-data`
- `iot-jobs-data`
- `iot1click-devices`
- `iot1click-projects`
- `iotanalytics`
- `iotdeviceadvisor`
- `iotevents`
- `iotevents-data`
- `iotfleethub`
- `iotsecuretunneling`
- `iotsitewise`
- `iotthingsgraph`
- `iottwinmaker`
- `iotwireless`
- `ivs`
- `kafka`
- `kafkaconnect`
- `kendra`
- `keyspaces`
- `kinesis`
- `kinesis-video-archived-media`
- `kinesis-video-media`
- `kinesis-video-signaling`
- `kinesisanalytics`
- `kinesisanalyticsv2`
- `kinesisvideo`
- `kms`
- `lakeformation`
- `lambda`
- `lex-models`
- `lex-runtime`
- `lexv2-models`
- `lexv2-runtime`
- `license-manager`
- `lightsail`
- `location`
- `logs`
- `lookoutequipment`
- `lookoutmetrics`
- `lookoutvision`
- `machinelearning`
- `macie`
- `macie2`
- `managedblockchain`
- `marketplace-catalog`
- `marketplace-entitlement`
- `marketplacecommerceanalytics`
- `mediaconnect`
- `mediaconvert`
- `medialive`
- `mediapackage`
- `mediapackage-vod`
- `mediastore`
- `mediastore-data`
- `mediatailor`
- `memorydb`
- `meteringmarketplace`
- `mgh`
- `mgn`
- `migration-hub-refactor-spaces`
- `migrationhub-config`
- `migrationhubstrategy`
- `mobile`
- `mq`
- `mturk`
- `mwaa`
- `neptune`
- `network-firewall`
- `networkmanager`
- `nimble`
- `opensearch`
- `opsworks`
- `opsworkscm`
- `organizations`
- `outposts`
- `panorama`
- `personalize`
- `personalize-events`
- `personalize-runtime`
- `pi`
- `pinpoint`
- `pinpoint-email`
- `pinpoint-sms-voice`
- `polly`
- `pricing`
- `proton`
- `qldb`
- `qldb-session`
- `quicksight`
- `ram`
- `rbin`
- `rds`
- `rds-data`
- `redshift`
- `redshift-data`
- `rekognition`
- `resiliencehub`
- `resource-groups`
- `resourcegroupstaggingapi`
- `robomaker`
- `route53`
- `route53-recovery-cluster`
- `route53-recovery-control-config`
- `route53-recovery-readiness`
- `route53domains`
- `route53resolver`
- `rum`
- `s3`
- `s3control`
- `s3outposts`
- `sagemaker`
- `sagemaker-a2i-runtime`
- `sagemaker-edge`
- `sagemaker-featurestore-runtime`
- `sagemaker-runtime`
- `savingsplans`
- `schemas`
- `sdb`
- `secretsmanager`
- `securityhub`
- `serverlessrepo`
- `service-quotas`
- `servicecatalog`
- `servicecatalog-appregistry`
- `servicediscovery`
- `ses`
- `sesv2`
- `shield`
- `signer`
- `sms`
- `sms-voice`
- `snow-device-management`
- `snowball`
- `sns`
- `sqs`
- `ssm`
- `ssm-contacts`
- `ssm-incidents`
- `sso`
- `sso-admin`
- `sso-oidc`
- `stepfunctions`
- `storagegateway`
- `sts`
- `support`
- `swf`
- `synthetics`
- `textract`
- `timestream-query`
- `timestream-write`
- `transcribe`
- `transfer`
- `translate`
- `voice-id`
- `waf`
- `waf-regional`
- `wafv2`
- `wellarchitected`
- `wisdom`
- `workdocs`
- `worklink`
- `workmail`
- `workmailmessageflow`
- `workspaces`
- `workspaces-web`
- `xray`

<a id="resourceservicename"></a>

## ResourceServiceName

```python
from types_aiobotocore_honeycode.literals import ResourceServiceName
```

Values:

- `cloudformation`
- `cloudwatch`
- `dynamodb`
- `ec2`
- `glacier`
- `iam`
- `opsworks`
- `s3`
- `sns`
- `sqs`

<a id="paginatorname"></a>

## PaginatorName

```python
from types_aiobotocore_honeycode.literals import PaginatorName
```

Values:

- `list_table_columns`
- `list_table_rows`
- `list_tables`
- `query_table_rows`