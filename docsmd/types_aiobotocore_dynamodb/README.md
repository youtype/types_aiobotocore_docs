# DynamoDB module

> [Index](../README.md) > DynamoDB


!!! note ""

    Auto-generated documentation for [DynamoDB](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#dynamodb)
    type annotations stubs module [types-aiobotocore-dynamodb](https://pypi.org/project/types-aiobotocore-dynamodb/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.19.0' mypy_boto3_builder`
1. Select `aiobotocore` AWS SDK.
1. Add `DynamoDB` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `DynamoDB` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[dynamodb]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[dynamodb]'

# standalone installation
python -m pip install types-aiobotocore-dynamodb
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-dynamodb
```

## Usage

Code samples can be found in [Examples](./usage.md).

## DynamoDBClient

Type annotations and code completion for  `#!python session.create_client("dynamodb")` as [DynamoDBClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client)

```python
# DynamoDBClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_dynamodb.client import DynamoDBClient


session = get_session()
async with session.create_client("dynamodb") as client:
    client: DynamoDBClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("dynamodb").get_paginator("...")`.

```python
# ListBackupsPaginator usage example

from types_aiobotocore_dynamodb.paginator import ListBackupsPaginator

def get_list_backups_paginator() -> ListBackupsPaginator:
    return client.get_paginator("list_backups"))
```

- [ListBackupsPaginator](./paginators.md#listbackupspaginator)
- [ListTablesPaginator](./paginators.md#listtablespaginator)
- [ListTagsOfResourcePaginator](./paginators.md#listtagsofresourcepaginator)
- [QueryPaginator](./paginators.md#querypaginator)
- [ScanPaginator](./paginators.md#scanpaginator)




## Waiters

Type annotations and code completion for
[waiters](./waiters.md)
from `#!python session.create_client("dynamodb").get_waiter("...")`.

```python
# TableExistsWaiter usage example

from types_aiobotocore_dynamodb.waiter import TableExistsWaiter

def get_table_exists_waiter() -> TableExistsWaiter:
    return Session().client("dynamodb").get_waiter("table_exists")
```

- [TableExistsWaiter](./waiters.md#tableexistswaiter)
- [TableNotExistsWaiter](./waiters.md#tablenotexistswaiter)




## DynamoDBServiceResource

Type annotations and code completion for `#!python session.resource("dynamodb")` as
[DynamoDBServiceResource](./service_resource.md#dynamodbserviceresource)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb/service-resource/index.html)

```python
# DynamoDBServiceResource usage example

from types_aiobotocore_dynamodb.service_resource import DynamoDBServiceResource
```


### Collections

Type annotations and code completion for collections
from `#!python session.resource("dynamodb").*`.

```python
# ServiceResourceTablesCollection usage example

from types_aiobotocore_dynamodb.service_resource import ServiceResourceTablesCollection

def get_collection() -> ServiceResourceTablesCollection:
    return resource.tables
```

- [ServiceResourceTablesCollection](./service_resource.md#serviceresourcetablescollection)





### Resources

Type annotations and code completion for additional resources
from `#!python session.resource("dynamodb").*`.

```python
# Table usage example

from types_aiobotocore_dynamodb.service_resource import Table

def get_resource() -> Table:
    return resource.Table(...)
```

- [Table](./service_resource.md#table)





## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# ApproximateCreationDateTimePrecisionType usage example

from types_aiobotocore_dynamodb.literals import ApproximateCreationDateTimePrecisionType

def get_value() -> ApproximateCreationDateTimePrecisionType:
    return "MICROSECOND"
```

- [ApproximateCreationDateTimePrecisionType](./literals.md#approximatecreationdatetimeprecisiontype)
- [AttributeActionType](./literals.md#attributeactiontype)
- [BackupStatusType](./literals.md#backupstatustype)
- [BackupTypeFilterType](./literals.md#backuptypefiltertype)
- [BackupTypeType](./literals.md#backuptypetype)
- [BatchStatementErrorCodeEnumType](./literals.md#batchstatementerrorcodeenumtype)
- [BillingModeType](./literals.md#billingmodetype)
- [ComparisonOperatorType](./literals.md#comparisonoperatortype)
- [ConditionalOperatorType](./literals.md#conditionaloperatortype)
- [ContinuousBackupsStatusType](./literals.md#continuousbackupsstatustype)
- [ContributorInsightsActionType](./literals.md#contributorinsightsactiontype)
- [ContributorInsightsStatusType](./literals.md#contributorinsightsstatustype)
- [DestinationStatusType](./literals.md#destinationstatustype)
- [ExportFormatType](./literals.md#exportformattype)
- [ExportStatusType](./literals.md#exportstatustype)
- [ExportTypeType](./literals.md#exporttypetype)
- [ExportViewTypeType](./literals.md#exportviewtypetype)
- [GlobalTableStatusType](./literals.md#globaltablestatustype)
- [ImportStatusType](./literals.md#importstatustype)
- [IndexStatusType](./literals.md#indexstatustype)
- [InputCompressionTypeType](./literals.md#inputcompressiontypetype)
- [InputFormatType](./literals.md#inputformattype)
- [KeyTypeType](./literals.md#keytypetype)
- [ListBackupsPaginatorName](./literals.md#listbackupspaginatorname)
- [ListTablesPaginatorName](./literals.md#listtablespaginatorname)
- [ListTagsOfResourcePaginatorName](./literals.md#listtagsofresourcepaginatorname)
- [MultiRegionConsistencyType](./literals.md#multiregionconsistencytype)
- [PointInTimeRecoveryStatusType](./literals.md#pointintimerecoverystatustype)
- [ProjectionTypeType](./literals.md#projectiontypetype)
- [QueryPaginatorName](./literals.md#querypaginatorname)
- [ReplicaStatusType](./literals.md#replicastatustype)
- [ReturnConsumedCapacityType](./literals.md#returnconsumedcapacitytype)
- [ReturnItemCollectionMetricsType](./literals.md#returnitemcollectionmetricstype)
- [ReturnValueType](./literals.md#returnvaluetype)
- [ReturnValuesOnConditionCheckFailureType](./literals.md#returnvaluesonconditioncheckfailuretype)
- [S3SseAlgorithmType](./literals.md#s3ssealgorithmtype)
- [SSEStatusType](./literals.md#ssestatustype)
- [SSETypeType](./literals.md#ssetypetype)
- [ScalarAttributeTypeType](./literals.md#scalarattributetypetype)
- [ScanPaginatorName](./literals.md#scanpaginatorname)
- [SelectType](./literals.md#selecttype)
- [StreamViewTypeType](./literals.md#streamviewtypetype)
- [TableClassType](./literals.md#tableclasstype)
- [TableExistsWaiterName](./literals.md#tableexistswaitername)
- [TableNotExistsWaiterName](./literals.md#tablenotexistswaitername)
- [TableStatusType](./literals.md#tablestatustype)
- [TimeToLiveStatusType](./literals.md#timetolivestatustype)
- [DynamoDBServiceName](./literals.md#dynamodbservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [WaiterName](./literals.md#waitername)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [ArchivalSummaryTypeDef](./type_defs.md#archivalsummarytypedef)
- [AttributeDefinitionTypeDef](./type_defs.md#attributedefinitiontypedef)
- [AttributeValueTypeDef](./type_defs.md#attributevaluetypedef)
- [TableAttributeValueTypeDef](./type_defs.md#tableattributevaluetypedef)
- [AutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef](./type_defs.md#autoscalingtargettrackingscalingpolicyconfigurationdescriptiontypedef)
- [AutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef](./type_defs.md#autoscalingtargettrackingscalingpolicyconfigurationupdatetypedef)
- [BackupDetailsTypeDef](./type_defs.md#backupdetailstypedef)
- [BackupSummaryTypeDef](./type_defs.md#backupsummarytypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [BillingModeSummaryTypeDef](./type_defs.md#billingmodesummarytypedef)
- [CapacityTypeDef](./type_defs.md#capacitytypedef)
- [ConditionBaseImportTypeDef](./type_defs.md#conditionbaseimporttypedef)
- [PointInTimeRecoveryDescriptionTypeDef](./type_defs.md#pointintimerecoverydescriptiontypedef)
- [ContributorInsightsSummaryTypeDef](./type_defs.md#contributorinsightssummarytypedef)
- [CreateBackupInputRequestTypeDef](./type_defs.md#createbackupinputrequesttypedef)
- [KeySchemaElementTypeDef](./type_defs.md#keyschemaelementtypedef)
- [OnDemandThroughputTypeDef](./type_defs.md#ondemandthroughputtypedef)
- [ProvisionedThroughputTypeDef](./type_defs.md#provisionedthroughputtypedef)
- [WarmThroughputTypeDef](./type_defs.md#warmthroughputtypedef)
- [ReplicaTypeDef](./type_defs.md#replicatypedef)
- [CreateReplicaActionTypeDef](./type_defs.md#createreplicaactiontypedef)
- [OnDemandThroughputOverrideTypeDef](./type_defs.md#ondemandthroughputoverridetypedef)
- [ProvisionedThroughputOverrideTypeDef](./type_defs.md#provisionedthroughputoverridetypedef)
- [SSESpecificationTypeDef](./type_defs.md#ssespecificationtypedef)
- [StreamSpecificationTypeDef](./type_defs.md#streamspecificationtypedef)
- [TagTypeDef](./type_defs.md#tagtypedef)
- [CsvOptionsOutputTypeDef](./type_defs.md#csvoptionsoutputtypedef)
- [CsvOptionsTypeDef](./type_defs.md#csvoptionstypedef)
- [DeleteBackupInputRequestTypeDef](./type_defs.md#deletebackupinputrequesttypedef)
- [DeleteGlobalSecondaryIndexActionTypeDef](./type_defs.md#deleteglobalsecondaryindexactiontypedef)
- [DeleteReplicaActionTypeDef](./type_defs.md#deletereplicaactiontypedef)
- [DeleteReplicationGroupMemberActionTypeDef](./type_defs.md#deletereplicationgroupmemberactiontypedef)
- [DeleteResourcePolicyInputRequestTypeDef](./type_defs.md#deleteresourcepolicyinputrequesttypedef)
- [DeleteTableInputRequestTypeDef](./type_defs.md#deletetableinputrequesttypedef)
- [DescribeBackupInputRequestTypeDef](./type_defs.md#describebackupinputrequesttypedef)
- [DescribeContinuousBackupsInputRequestTypeDef](./type_defs.md#describecontinuousbackupsinputrequesttypedef)
- [DescribeContributorInsightsInputRequestTypeDef](./type_defs.md#describecontributorinsightsinputrequesttypedef)
- [FailureExceptionTypeDef](./type_defs.md#failureexceptiontypedef)
- [EndpointTypeDef](./type_defs.md#endpointtypedef)
- [DescribeExportInputRequestTypeDef](./type_defs.md#describeexportinputrequesttypedef)
- [DescribeGlobalTableInputRequestTypeDef](./type_defs.md#describeglobaltableinputrequesttypedef)
- [DescribeGlobalTableSettingsInputRequestTypeDef](./type_defs.md#describeglobaltablesettingsinputrequesttypedef)
- [DescribeImportInputRequestTypeDef](./type_defs.md#describeimportinputrequesttypedef)
- [DescribeKinesisStreamingDestinationInputRequestTypeDef](./type_defs.md#describekinesisstreamingdestinationinputrequesttypedef)
- [KinesisDataStreamDestinationTypeDef](./type_defs.md#kinesisdatastreamdestinationtypedef)
- [DescribeTableInputRequestTypeDef](./type_defs.md#describetableinputrequesttypedef)
- [WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)
- [DescribeTableReplicaAutoScalingInputRequestTypeDef](./type_defs.md#describetablereplicaautoscalinginputrequesttypedef)
- [DescribeTimeToLiveInputRequestTypeDef](./type_defs.md#describetimetoliveinputrequesttypedef)
- [TimeToLiveDescriptionTypeDef](./type_defs.md#timetolivedescriptiontypedef)
- [EnableKinesisStreamingConfigurationTypeDef](./type_defs.md#enablekinesisstreamingconfigurationtypedef)
- [IncrementalExportSpecificationOutputTypeDef](./type_defs.md#incrementalexportspecificationoutputtypedef)
- [ExportSummaryTypeDef](./type_defs.md#exportsummarytypedef)
- [TimestampTypeDef](./type_defs.md#timestamptypedef)
- [GetResourcePolicyInputRequestTypeDef](./type_defs.md#getresourcepolicyinputrequesttypedef)
- [GlobalSecondaryIndexWarmThroughputDescriptionTypeDef](./type_defs.md#globalsecondaryindexwarmthroughputdescriptiontypedef)
- [ProjectionOutputTypeDef](./type_defs.md#projectionoutputtypedef)
- [ProvisionedThroughputDescriptionTypeDef](./type_defs.md#provisionedthroughputdescriptiontypedef)
- [S3BucketSourceTypeDef](./type_defs.md#s3bucketsourcetypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListContributorInsightsInputRequestTypeDef](./type_defs.md#listcontributorinsightsinputrequesttypedef)
- [ListExportsInputRequestTypeDef](./type_defs.md#listexportsinputrequesttypedef)
- [ListGlobalTablesInputRequestTypeDef](./type_defs.md#listglobaltablesinputrequesttypedef)
- [ListImportsInputRequestTypeDef](./type_defs.md#listimportsinputrequesttypedef)
- [ListTablesInputRequestTypeDef](./type_defs.md#listtablesinputrequesttypedef)
- [ListTagsOfResourceInputRequestTypeDef](./type_defs.md#listtagsofresourceinputrequesttypedef)
- [PointInTimeRecoverySpecificationTypeDef](./type_defs.md#pointintimerecoveryspecificationtypedef)
- [ProjectionTypeDef](./type_defs.md#projectiontypedef)
- [PutResourcePolicyInputRequestTypeDef](./type_defs.md#putresourcepolicyinputrequesttypedef)
- [TableClassSummaryTypeDef](./type_defs.md#tableclasssummarytypedef)
- [TableWarmThroughputDescriptionTypeDef](./type_defs.md#tablewarmthroughputdescriptiontypedef)
- [RestoreSummaryTypeDef](./type_defs.md#restoresummarytypedef)
- [SSEDescriptionTypeDef](./type_defs.md#ssedescriptiontypedef)
- [TableBatchWriterRequestTypeDef](./type_defs.md#tablebatchwriterrequesttypedef)
- [TimeToLiveSpecificationTypeDef](./type_defs.md#timetolivespecificationtypedef)
- [UntagResourceInputRequestTypeDef](./type_defs.md#untagresourceinputrequesttypedef)
- [UpdateContributorInsightsInputRequestTypeDef](./type_defs.md#updatecontributorinsightsinputrequesttypedef)
- [UpdateKinesisStreamingConfigurationTypeDef](./type_defs.md#updatekinesisstreamingconfigurationtypedef)
- [BatchStatementErrorTypeDef](./type_defs.md#batchstatementerrortypedef)
- [DeleteRequestOutputTypeDef](./type_defs.md#deleterequestoutputtypedef)
- [ItemCollectionMetricsTypeDef](./type_defs.md#itemcollectionmetricstypedef)
- [ItemResponseTypeDef](./type_defs.md#itemresponsetypedef)
- [KeysAndAttributesOutputTypeDef](./type_defs.md#keysandattributesoutputtypedef)
- [PutRequestOutputTypeDef](./type_defs.md#putrequestoutputtypedef)
- [UniversalAttributeValueTypeDef](./type_defs.md#universalattributevaluetypedef)
- [AttributeValueUpdateTableTypeDef](./type_defs.md#attributevalueupdatetabletypedef)
- [ConditionTableTypeDef](./type_defs.md#conditiontabletypedef)
- [DeleteRequestServiceResourceOutputTypeDef](./type_defs.md#deleterequestserviceresourceoutputtypedef)
- [DeleteRequestServiceResourceTypeDef](./type_defs.md#deleterequestserviceresourcetypedef)
- [ExpectedAttributeValueTableTypeDef](./type_defs.md#expectedattributevaluetabletypedef)
- [GetItemInputTableGetItemTypeDef](./type_defs.md#getiteminputtablegetitemtypedef)
- [ItemCollectionMetricsServiceResourceTypeDef](./type_defs.md#itemcollectionmetricsserviceresourcetypedef)
- [ItemCollectionMetricsTableTypeDef](./type_defs.md#itemcollectionmetricstabletypedef)
- [KeysAndAttributesServiceResourceOutputTypeDef](./type_defs.md#keysandattributesserviceresourceoutputtypedef)
- [KeysAndAttributesServiceResourceTypeDef](./type_defs.md#keysandattributesserviceresourcetypedef)
- [PutRequestServiceResourceOutputTypeDef](./type_defs.md#putrequestserviceresourceoutputtypedef)
- [PutRequestServiceResourceTypeDef](./type_defs.md#putrequestserviceresourcetypedef)
- [AutoScalingPolicyDescriptionTypeDef](./type_defs.md#autoscalingpolicydescriptiontypedef)
- [AutoScalingPolicyUpdateTypeDef](./type_defs.md#autoscalingpolicyupdatetypedef)
- [CreateBackupOutputTypeDef](./type_defs.md#createbackupoutputtypedef)
- [DeleteResourcePolicyOutputTypeDef](./type_defs.md#deleteresourcepolicyoutputtypedef)
- [DescribeLimitsOutputTypeDef](./type_defs.md#describelimitsoutputtypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [GetResourcePolicyOutputTypeDef](./type_defs.md#getresourcepolicyoutputtypedef)
- [ListBackupsOutputTypeDef](./type_defs.md#listbackupsoutputtypedef)
- [ListTablesOutputTypeDef](./type_defs.md#listtablesoutputtypedef)
- [PutResourcePolicyOutputTypeDef](./type_defs.md#putresourcepolicyoutputtypedef)
- [UpdateContributorInsightsOutputTypeDef](./type_defs.md#updatecontributorinsightsoutputtypedef)
- [ConsumedCapacityTypeDef](./type_defs.md#consumedcapacitytypedef)
- [ContinuousBackupsDescriptionTypeDef](./type_defs.md#continuousbackupsdescriptiontypedef)
- [ListContributorInsightsOutputTypeDef](./type_defs.md#listcontributorinsightsoutputtypedef)
- [SourceTableDetailsTypeDef](./type_defs.md#sourcetabledetailstypedef)
- [UpdateGlobalSecondaryIndexActionTypeDef](./type_defs.md#updateglobalsecondaryindexactiontypedef)
- [CreateGlobalTableInputRequestTypeDef](./type_defs.md#createglobaltableinputrequesttypedef)
- [GlobalTableTypeDef](./type_defs.md#globaltabletypedef)
- [ReplicaGlobalSecondaryIndexTypeDef](./type_defs.md#replicaglobalsecondaryindextypedef)
- [ListTagsOfResourceOutputTypeDef](./type_defs.md#listtagsofresourceoutputtypedef)
- [TagResourceInputRequestTypeDef](./type_defs.md#tagresourceinputrequesttypedef)
- [InputFormatOptionsOutputTypeDef](./type_defs.md#inputformatoptionsoutputtypedef)
- [CsvOptionsUnionTypeDef](./type_defs.md#csvoptionsuniontypedef)
- [ReplicaUpdateTypeDef](./type_defs.md#replicaupdatetypedef)
- [DescribeContributorInsightsOutputTypeDef](./type_defs.md#describecontributorinsightsoutputtypedef)
- [DescribeEndpointsResponseTypeDef](./type_defs.md#describeendpointsresponsetypedef)
- [DescribeKinesisStreamingDestinationOutputTypeDef](./type_defs.md#describekinesisstreamingdestinationoutputtypedef)
- [DescribeTableInputWaitTypeDef](./type_defs.md#describetableinputwaittypedef)
- [DescribeTimeToLiveOutputTypeDef](./type_defs.md#describetimetoliveoutputtypedef)
- [KinesisStreamingDestinationInputRequestTypeDef](./type_defs.md#kinesisstreamingdestinationinputrequesttypedef)
- [KinesisStreamingDestinationOutputTypeDef](./type_defs.md#kinesisstreamingdestinationoutputtypedef)
- [ExportDescriptionTypeDef](./type_defs.md#exportdescriptiontypedef)
- [ListExportsOutputTypeDef](./type_defs.md#listexportsoutputtypedef)
- [IncrementalExportSpecificationTypeDef](./type_defs.md#incrementalexportspecificationtypedef)
- [ListBackupsInputRequestTypeDef](./type_defs.md#listbackupsinputrequesttypedef)
- [ReplicaGlobalSecondaryIndexDescriptionTypeDef](./type_defs.md#replicaglobalsecondaryindexdescriptiontypedef)
- [GlobalSecondaryIndexInfoTypeDef](./type_defs.md#globalsecondaryindexinfotypedef)
- [GlobalSecondaryIndexOutputTypeDef](./type_defs.md#globalsecondaryindexoutputtypedef)
- [LocalSecondaryIndexDescriptionTypeDef](./type_defs.md#localsecondaryindexdescriptiontypedef)
- [LocalSecondaryIndexInfoTypeDef](./type_defs.md#localsecondaryindexinfotypedef)
- [GlobalSecondaryIndexDescriptionTypeDef](./type_defs.md#globalsecondaryindexdescriptiontypedef)
- [ImportSummaryTypeDef](./type_defs.md#importsummarytypedef)
- [ListBackupsInputPaginateTypeDef](./type_defs.md#listbackupsinputpaginatetypedef)
- [ListTablesInputPaginateTypeDef](./type_defs.md#listtablesinputpaginatetypedef)
- [ListTagsOfResourceInputPaginateTypeDef](./type_defs.md#listtagsofresourceinputpaginatetypedef)
- [UpdateContinuousBackupsInputRequestTypeDef](./type_defs.md#updatecontinuousbackupsinputrequesttypedef)
- [ProjectionUnionTypeDef](./type_defs.md#projectionuniontypedef)
- [UpdateTimeToLiveInputRequestTypeDef](./type_defs.md#updatetimetoliveinputrequesttypedef)
- [UpdateTimeToLiveOutputTypeDef](./type_defs.md#updatetimetoliveoutputtypedef)
- [UpdateKinesisStreamingDestinationInputRequestTypeDef](./type_defs.md#updatekinesisstreamingdestinationinputrequesttypedef)
- [UpdateKinesisStreamingDestinationOutputTypeDef](./type_defs.md#updatekinesisstreamingdestinationoutputtypedef)
- [BatchStatementResponseTypeDef](./type_defs.md#batchstatementresponsetypedef)
- [WriteRequestOutputTypeDef](./type_defs.md#writerequestoutputtypedef)
- [AttributeValueUpdateTypeDef](./type_defs.md#attributevalueupdatetypedef)
- [BatchStatementRequestTypeDef](./type_defs.md#batchstatementrequesttypedef)
- [ConditionCheckTypeDef](./type_defs.md#conditionchecktypedef)
- [ConditionTypeDef](./type_defs.md#conditiontypedef)
- [DeleteRequestTypeDef](./type_defs.md#deleterequesttypedef)
- [DeleteTypeDef](./type_defs.md#deletetypedef)
- [ExecuteStatementInputRequestTypeDef](./type_defs.md#executestatementinputrequesttypedef)
- [ExpectedAttributeValueTypeDef](./type_defs.md#expectedattributevaluetypedef)
- [GetItemInputRequestTypeDef](./type_defs.md#getiteminputrequesttypedef)
- [GetTypeDef](./type_defs.md#gettypedef)
- [KeysAndAttributesTypeDef](./type_defs.md#keysandattributestypedef)
- [ParameterizedStatementTypeDef](./type_defs.md#parameterizedstatementtypedef)
- [PutRequestTypeDef](./type_defs.md#putrequesttypedef)
- [PutTypeDef](./type_defs.md#puttypedef)
- [UpdateTypeDef](./type_defs.md#updatetypedef)
- [QueryInputTableQueryTypeDef](./type_defs.md#queryinputtablequerytypedef)
- [ScanInputTableScanTypeDef](./type_defs.md#scaninputtablescantypedef)
- [DeleteRequestServiceResourceUnionTypeDef](./type_defs.md#deleterequestserviceresourceuniontypedef)
- [DeleteItemInputTableDeleteItemTypeDef](./type_defs.md#deleteiteminputtabledeleteitemtypedef)
- [PutItemInputTablePutItemTypeDef](./type_defs.md#putiteminputtableputitemtypedef)
- [UpdateItemInputTableUpdateItemTypeDef](./type_defs.md#updateiteminputtableupdateitemtypedef)
- [KeysAndAttributesServiceResourceUnionTypeDef](./type_defs.md#keysandattributesserviceresourceuniontypedef)
- [WriteRequestServiceResourceOutputTypeDef](./type_defs.md#writerequestserviceresourceoutputtypedef)
- [PutRequestServiceResourceUnionTypeDef](./type_defs.md#putrequestserviceresourceuniontypedef)
- [AutoScalingSettingsDescriptionTypeDef](./type_defs.md#autoscalingsettingsdescriptiontypedef)
- [AutoScalingSettingsUpdateTypeDef](./type_defs.md#autoscalingsettingsupdatetypedef)
- [BatchGetItemOutputServiceResourceTypeDef](./type_defs.md#batchgetitemoutputserviceresourcetypedef)
- [BatchGetItemOutputTypeDef](./type_defs.md#batchgetitemoutputtypedef)
- [DeleteItemOutputTableTypeDef](./type_defs.md#deleteitemoutputtabletypedef)
- [DeleteItemOutputTypeDef](./type_defs.md#deleteitemoutputtypedef)
- [ExecuteStatementOutputTypeDef](./type_defs.md#executestatementoutputtypedef)
- [ExecuteTransactionOutputTypeDef](./type_defs.md#executetransactionoutputtypedef)
- [GetItemOutputTableTypeDef](./type_defs.md#getitemoutputtabletypedef)
- [GetItemOutputTypeDef](./type_defs.md#getitemoutputtypedef)
- [PutItemOutputTableTypeDef](./type_defs.md#putitemoutputtabletypedef)
- [PutItemOutputTypeDef](./type_defs.md#putitemoutputtypedef)
- [QueryOutputTableTypeDef](./type_defs.md#queryoutputtabletypedef)
- [QueryOutputTypeDef](./type_defs.md#queryoutputtypedef)
- [ScanOutputTableTypeDef](./type_defs.md#scanoutputtabletypedef)
- [ScanOutputTypeDef](./type_defs.md#scanoutputtypedef)
- [TransactGetItemsOutputTypeDef](./type_defs.md#transactgetitemsoutputtypedef)
- [TransactWriteItemsOutputTypeDef](./type_defs.md#transactwriteitemsoutputtypedef)
- [UpdateItemOutputTableTypeDef](./type_defs.md#updateitemoutputtabletypedef)
- [UpdateItemOutputTypeDef](./type_defs.md#updateitemoutputtypedef)
- [DescribeContinuousBackupsOutputTypeDef](./type_defs.md#describecontinuousbackupsoutputtypedef)
- [UpdateContinuousBackupsOutputTypeDef](./type_defs.md#updatecontinuousbackupsoutputtypedef)
- [ListGlobalTablesOutputTypeDef](./type_defs.md#listglobaltablesoutputtypedef)
- [CreateReplicationGroupMemberActionTypeDef](./type_defs.md#createreplicationgroupmemberactiontypedef)
- [UpdateReplicationGroupMemberActionTypeDef](./type_defs.md#updatereplicationgroupmemberactiontypedef)
- [InputFormatOptionsTypeDef](./type_defs.md#inputformatoptionstypedef)
- [UpdateGlobalTableInputRequestTypeDef](./type_defs.md#updateglobaltableinputrequesttypedef)
- [DescribeExportOutputTypeDef](./type_defs.md#describeexportoutputtypedef)
- [ExportTableToPointInTimeOutputTypeDef](./type_defs.md#exporttabletopointintimeoutputtypedef)
- [ExportTableToPointInTimeInputRequestTypeDef](./type_defs.md#exporttabletopointintimeinputrequesttypedef)
- [ReplicaDescriptionTypeDef](./type_defs.md#replicadescriptiontypedef)
- [TableCreationParametersOutputTypeDef](./type_defs.md#tablecreationparametersoutputtypedef)
- [SourceTableFeatureDetailsTypeDef](./type_defs.md#sourcetablefeaturedetailstypedef)
- [ListImportsOutputTypeDef](./type_defs.md#listimportsoutputtypedef)
- [CreateGlobalSecondaryIndexActionTypeDef](./type_defs.md#createglobalsecondaryindexactiontypedef)
- [GlobalSecondaryIndexTypeDef](./type_defs.md#globalsecondaryindextypedef)
- [LocalSecondaryIndexTypeDef](./type_defs.md#localsecondaryindextypedef)
- [BatchExecuteStatementOutputTypeDef](./type_defs.md#batchexecutestatementoutputtypedef)
- [BatchWriteItemOutputTypeDef](./type_defs.md#batchwriteitemoutputtypedef)
- [BatchExecuteStatementInputRequestTypeDef](./type_defs.md#batchexecutestatementinputrequesttypedef)
- [QueryInputPaginateTypeDef](./type_defs.md#queryinputpaginatetypedef)
- [QueryInputRequestTypeDef](./type_defs.md#queryinputrequesttypedef)
- [ScanInputPaginateTypeDef](./type_defs.md#scaninputpaginatetypedef)
- [ScanInputRequestTypeDef](./type_defs.md#scaninputrequesttypedef)
- [DeleteRequestUnionTypeDef](./type_defs.md#deleterequestuniontypedef)
- [DeleteItemInputRequestTypeDef](./type_defs.md#deleteiteminputrequesttypedef)
- [PutItemInputRequestTypeDef](./type_defs.md#putiteminputrequesttypedef)
- [UpdateItemInputRequestTypeDef](./type_defs.md#updateiteminputrequesttypedef)
- [TransactGetItemTypeDef](./type_defs.md#transactgetitemtypedef)
- [KeysAndAttributesUnionTypeDef](./type_defs.md#keysandattributesuniontypedef)
- [ExecuteTransactionInputRequestTypeDef](./type_defs.md#executetransactioninputrequesttypedef)
- [PutRequestUnionTypeDef](./type_defs.md#putrequestuniontypedef)
- [TransactWriteItemTypeDef](./type_defs.md#transactwriteitemtypedef)
- [BatchGetItemInputServiceResourceBatchGetItemTypeDef](./type_defs.md#batchgetiteminputserviceresourcebatchgetitemtypedef)
- [BatchWriteItemOutputServiceResourceTypeDef](./type_defs.md#batchwriteitemoutputserviceresourcetypedef)
- [WriteRequestServiceResourceTypeDef](./type_defs.md#writerequestserviceresourcetypedef)
- [ReplicaGlobalSecondaryIndexAutoScalingDescriptionTypeDef](./type_defs.md#replicaglobalsecondaryindexautoscalingdescriptiontypedef)
- [ReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef](./type_defs.md#replicaglobalsecondaryindexsettingsdescriptiontypedef)
- [GlobalSecondaryIndexAutoScalingUpdateTypeDef](./type_defs.md#globalsecondaryindexautoscalingupdatetypedef)
- [GlobalTableGlobalSecondaryIndexSettingsUpdateTypeDef](./type_defs.md#globaltableglobalsecondaryindexsettingsupdatetypedef)
- [ReplicaGlobalSecondaryIndexAutoScalingUpdateTypeDef](./type_defs.md#replicaglobalsecondaryindexautoscalingupdatetypedef)
- [ReplicaGlobalSecondaryIndexSettingsUpdateTypeDef](./type_defs.md#replicaglobalsecondaryindexsettingsupdatetypedef)
- [ReplicationGroupUpdateTypeDef](./type_defs.md#replicationgroupupdatetypedef)
- [GlobalTableDescriptionTypeDef](./type_defs.md#globaltabledescriptiontypedef)
- [TableDescriptionTypeDef](./type_defs.md#tabledescriptiontypedef)
- [ImportTableDescriptionTypeDef](./type_defs.md#importtabledescriptiontypedef)
- [BackupDescriptionTypeDef](./type_defs.md#backupdescriptiontypedef)
- [GlobalSecondaryIndexUpdateTypeDef](./type_defs.md#globalsecondaryindexupdatetypedef)
- [TableCreationParametersTypeDef](./type_defs.md#tablecreationparameterstypedef)
- [CreateTableInputRequestTypeDef](./type_defs.md#createtableinputrequesttypedef)
- [CreateTableInputServiceResourceCreateTableTypeDef](./type_defs.md#createtableinputserviceresourcecreatetabletypedef)
- [RestoreTableFromBackupInputRequestTypeDef](./type_defs.md#restoretablefrombackupinputrequesttypedef)
- [RestoreTableToPointInTimeInputRequestTypeDef](./type_defs.md#restoretabletopointintimeinputrequesttypedef)
- [TransactGetItemsInputRequestTypeDef](./type_defs.md#transactgetitemsinputrequesttypedef)
- [BatchGetItemInputRequestTypeDef](./type_defs.md#batchgetiteminputrequesttypedef)
- [WriteRequestTypeDef](./type_defs.md#writerequesttypedef)
- [TransactWriteItemsInputRequestTypeDef](./type_defs.md#transactwriteitemsinputrequesttypedef)
- [WriteRequestServiceResourceUnionTypeDef](./type_defs.md#writerequestserviceresourceuniontypedef)
- [ReplicaAutoScalingDescriptionTypeDef](./type_defs.md#replicaautoscalingdescriptiontypedef)
- [ReplicaSettingsDescriptionTypeDef](./type_defs.md#replicasettingsdescriptiontypedef)
- [ReplicaAutoScalingUpdateTypeDef](./type_defs.md#replicaautoscalingupdatetypedef)
- [ReplicaSettingsUpdateTypeDef](./type_defs.md#replicasettingsupdatetypedef)
- [CreateGlobalTableOutputTypeDef](./type_defs.md#createglobaltableoutputtypedef)
- [DescribeGlobalTableOutputTypeDef](./type_defs.md#describeglobaltableoutputtypedef)
- [UpdateGlobalTableOutputTypeDef](./type_defs.md#updateglobaltableoutputtypedef)
- [CreateTableOutputTypeDef](./type_defs.md#createtableoutputtypedef)
- [DeleteTableOutputTypeDef](./type_defs.md#deletetableoutputtypedef)
- [DescribeTableOutputTypeDef](./type_defs.md#describetableoutputtypedef)
- [RestoreTableFromBackupOutputTypeDef](./type_defs.md#restoretablefrombackupoutputtypedef)
- [RestoreTableToPointInTimeOutputTypeDef](./type_defs.md#restoretabletopointintimeoutputtypedef)
- [UpdateTableOutputTypeDef](./type_defs.md#updatetableoutputtypedef)
- [DescribeImportOutputTypeDef](./type_defs.md#describeimportoutputtypedef)
- [ImportTableOutputTypeDef](./type_defs.md#importtableoutputtypedef)
- [DeleteBackupOutputTypeDef](./type_defs.md#deletebackupoutputtypedef)
- [DescribeBackupOutputTypeDef](./type_defs.md#describebackupoutputtypedef)
- [UpdateTableInputRequestTypeDef](./type_defs.md#updatetableinputrequesttypedef)
- [UpdateTableInputTableUpdateTypeDef](./type_defs.md#updatetableinputtableupdatetypedef)
- [ImportTableInputRequestTypeDef](./type_defs.md#importtableinputrequesttypedef)
- [WriteRequestUnionTypeDef](./type_defs.md#writerequestuniontypedef)
- [BatchWriteItemInputServiceResourceBatchWriteItemTypeDef](./type_defs.md#batchwriteiteminputserviceresourcebatchwriteitemtypedef)
- [TableAutoScalingDescriptionTypeDef](./type_defs.md#tableautoscalingdescriptiontypedef)
- [DescribeGlobalTableSettingsOutputTypeDef](./type_defs.md#describeglobaltablesettingsoutputtypedef)
- [UpdateGlobalTableSettingsOutputTypeDef](./type_defs.md#updateglobaltablesettingsoutputtypedef)
- [UpdateTableReplicaAutoScalingInputRequestTypeDef](./type_defs.md#updatetablereplicaautoscalinginputrequesttypedef)
- [UpdateGlobalTableSettingsInputRequestTypeDef](./type_defs.md#updateglobaltablesettingsinputrequesttypedef)
- [BatchWriteItemInputRequestTypeDef](./type_defs.md#batchwriteiteminputrequesttypedef)
- [DescribeTableReplicaAutoScalingOutputTypeDef](./type_defs.md#describetablereplicaautoscalingoutputtypedef)
- [UpdateTableReplicaAutoScalingOutputTypeDef](./type_defs.md#updatetablereplicaautoscalingoutputtypedef)

