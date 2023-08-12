# Type definitions

> [Index](../README.md) > [SecurityLake](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [SecurityLake](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake)
    type annotations stubs module [types-aiobotocore-securitylake](https://pypi.org/project/types-aiobotocore-securitylake/).



## AwsIdentityTypeDef

```python
# AwsIdentityTypeDef definition

class AwsIdentityTypeDef(TypedDict):
    externalId: str,
    principal: str,
```

## AwsLogSourceConfigurationTypeDef

```python
# AwsLogSourceConfigurationTypeDef definition

class AwsLogSourceConfigurationTypeDef(TypedDict):
    regions: Sequence[str],
    sourceName: AwsLogSourceNameType,  # (1)
    accounts: NotRequired[Sequence[str]],
    sourceVersion: NotRequired[str],
```

1. See [:material-code-brackets: AwsLogSourceNameType](./literals.md#awslogsourcenametype) 
## AwsLogSourceResourceTypeDef

```python
# AwsLogSourceResourceTypeDef definition

class AwsLogSourceResourceTypeDef(TypedDict):
    sourceName: NotRequired[AwsLogSourceNameType],  # (1)
    sourceVersion: NotRequired[str],
```

1. See [:material-code-brackets: AwsLogSourceNameType](./literals.md#awslogsourcenametype) 
## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef definition

class ResponseMetadataTypeDef(TypedDict):
    RequestId: str,
    HostId: str,
    HTTPStatusCode: int,
    HTTPHeaders: Dict[str, str],
    RetryAttempts: int,
```

## CreateDataLakeExceptionSubscriptionRequestRequestTypeDef

```python
# CreateDataLakeExceptionSubscriptionRequestRequestTypeDef definition

class CreateDataLakeExceptionSubscriptionRequestRequestTypeDef(TypedDict):
    notificationEndpoint: str,
    subscriptionProtocol: str,
    exceptionTimeToLive: NotRequired[int],
```

## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    key: str,
    value: str,
```

## CustomLogSourceAttributesTypeDef

```python
# CustomLogSourceAttributesTypeDef definition

class CustomLogSourceAttributesTypeDef(TypedDict):
    crawlerArn: NotRequired[str],
    databaseArn: NotRequired[str],
    tableArn: NotRequired[str],
```

## CustomLogSourceCrawlerConfigurationTypeDef

```python
# CustomLogSourceCrawlerConfigurationTypeDef definition

class CustomLogSourceCrawlerConfigurationTypeDef(TypedDict):
    roleArn: str,
```

## CustomLogSourceProviderTypeDef

```python
# CustomLogSourceProviderTypeDef definition

class CustomLogSourceProviderTypeDef(TypedDict):
    location: NotRequired[str],
    roleArn: NotRequired[str],
```

## DataLakeEncryptionConfigurationTypeDef

```python
# DataLakeEncryptionConfigurationTypeDef definition

class DataLakeEncryptionConfigurationTypeDef(TypedDict):
    kmsKeyId: NotRequired[str],
```

## DataLakeReplicationConfigurationTypeDef

```python
# DataLakeReplicationConfigurationTypeDef definition

class DataLakeReplicationConfigurationTypeDef(TypedDict):
    regions: NotRequired[Sequence[str]],
    roleArn: NotRequired[str],
```

## DataLakeExceptionTypeDef

```python
# DataLakeExceptionTypeDef definition

class DataLakeExceptionTypeDef(TypedDict):
    exception: NotRequired[str],
    region: NotRequired[str],
    remediation: NotRequired[str],
    timestamp: NotRequired[datetime],
```

## DataLakeLifecycleExpirationTypeDef

```python
# DataLakeLifecycleExpirationTypeDef definition

class DataLakeLifecycleExpirationTypeDef(TypedDict):
    days: NotRequired[int],
```

## DataLakeLifecycleTransitionTypeDef

```python
# DataLakeLifecycleTransitionTypeDef definition

class DataLakeLifecycleTransitionTypeDef(TypedDict):
    days: NotRequired[int],
    storageClass: NotRequired[str],
```

## DataLakeSourceStatusTypeDef

```python
# DataLakeSourceStatusTypeDef definition

class DataLakeSourceStatusTypeDef(TypedDict):
    resource: NotRequired[str],
    status: NotRequired[SourceCollectionStatusType],  # (1)
```

1. See [:material-code-brackets: SourceCollectionStatusType](./literals.md#sourcecollectionstatustype) 
## DataLakeUpdateExceptionTypeDef

```python
# DataLakeUpdateExceptionTypeDef definition

class DataLakeUpdateExceptionTypeDef(TypedDict):
    code: NotRequired[str],
    reason: NotRequired[str],
```

## DeleteCustomLogSourceRequestRequestTypeDef

```python
# DeleteCustomLogSourceRequestRequestTypeDef definition

class DeleteCustomLogSourceRequestRequestTypeDef(TypedDict):
    sourceName: str,
    sourceVersion: NotRequired[str],
```

## DeleteDataLakeRequestRequestTypeDef

```python
# DeleteDataLakeRequestRequestTypeDef definition

class DeleteDataLakeRequestRequestTypeDef(TypedDict):
    regions: Sequence[str],
```

## DeleteSubscriberNotificationRequestRequestTypeDef

```python
# DeleteSubscriberNotificationRequestRequestTypeDef definition

class DeleteSubscriberNotificationRequestRequestTypeDef(TypedDict):
    subscriberId: str,
```

## DeleteSubscriberRequestRequestTypeDef

```python
# DeleteSubscriberRequestRequestTypeDef definition

class DeleteSubscriberRequestRequestTypeDef(TypedDict):
    subscriberId: str,
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## GetDataLakeSourcesRequestRequestTypeDef

```python
# GetDataLakeSourcesRequestRequestTypeDef definition

class GetDataLakeSourcesRequestRequestTypeDef(TypedDict):
    accounts: NotRequired[Sequence[str]],
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## GetSubscriberRequestRequestTypeDef

```python
# GetSubscriberRequestRequestTypeDef definition

class GetSubscriberRequestRequestTypeDef(TypedDict):
    subscriberId: str,
```

## HttpsNotificationConfigurationTypeDef

```python
# HttpsNotificationConfigurationTypeDef definition

class HttpsNotificationConfigurationTypeDef(TypedDict):
    endpoint: str,
    targetRoleArn: str,
    authorizationApiKeyName: NotRequired[str],
    authorizationApiKeyValue: NotRequired[str],
    httpMethod: NotRequired[HttpMethodType],  # (1)
```

1. See [:material-code-brackets: HttpMethodType](./literals.md#httpmethodtype) 
## ListDataLakeExceptionsRequestRequestTypeDef

```python
# ListDataLakeExceptionsRequestRequestTypeDef definition

class ListDataLakeExceptionsRequestRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    regions: NotRequired[Sequence[str]],
```

## ListDataLakesRequestRequestTypeDef

```python
# ListDataLakesRequestRequestTypeDef definition

class ListDataLakesRequestRequestTypeDef(TypedDict):
    regions: NotRequired[Sequence[str]],
```

## ListSubscribersRequestRequestTypeDef

```python
# ListSubscribersRequestRequestTypeDef definition

class ListSubscribersRequestRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
```

## RegisterDataLakeDelegatedAdministratorRequestRequestTypeDef

```python
# RegisterDataLakeDelegatedAdministratorRequestRequestTypeDef definition

class RegisterDataLakeDelegatedAdministratorRequestRequestTypeDef(TypedDict):
    accountId: str,
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    tagKeys: Sequence[str],
```

## UpdateDataLakeExceptionSubscriptionRequestRequestTypeDef

```python
# UpdateDataLakeExceptionSubscriptionRequestRequestTypeDef definition

class UpdateDataLakeExceptionSubscriptionRequestRequestTypeDef(TypedDict):
    notificationEndpoint: str,
    subscriptionProtocol: str,
    exceptionTimeToLive: NotRequired[int],
```

## CreateAwsLogSourceRequestRequestTypeDef

```python
# CreateAwsLogSourceRequestRequestTypeDef definition

class CreateAwsLogSourceRequestRequestTypeDef(TypedDict):
    sources: Sequence[AwsLogSourceConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: AwsLogSourceConfigurationTypeDef](./type_defs.md#awslogsourceconfigurationtypedef) 
## DeleteAwsLogSourceRequestRequestTypeDef

```python
# DeleteAwsLogSourceRequestRequestTypeDef definition

class DeleteAwsLogSourceRequestRequestTypeDef(TypedDict):
    sources: Sequence[AwsLogSourceConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: AwsLogSourceConfigurationTypeDef](./type_defs.md#awslogsourceconfigurationtypedef) 
## DataLakeAutoEnableNewAccountConfigurationTypeDef

```python
# DataLakeAutoEnableNewAccountConfigurationTypeDef definition

class DataLakeAutoEnableNewAccountConfigurationTypeDef(TypedDict):
    region: str,
    sources: Sequence[AwsLogSourceResourceTypeDef],  # (1)
```

1. See [:material-code-braces: AwsLogSourceResourceTypeDef](./type_defs.md#awslogsourceresourcetypedef) 
## CreateAwsLogSourceResponseTypeDef

```python
# CreateAwsLogSourceResponseTypeDef definition

class CreateAwsLogSourceResponseTypeDef(TypedDict):
    failed: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateSubscriberNotificationResponseTypeDef

```python
# CreateSubscriberNotificationResponseTypeDef definition

class CreateSubscriberNotificationResponseTypeDef(TypedDict):
    subscriberEndpoint: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteAwsLogSourceResponseTypeDef

```python
# DeleteAwsLogSourceResponseTypeDef definition

class DeleteAwsLogSourceResponseTypeDef(TypedDict):
    failed: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetDataLakeExceptionSubscriptionResponseTypeDef

```python
# GetDataLakeExceptionSubscriptionResponseTypeDef definition

class GetDataLakeExceptionSubscriptionResponseTypeDef(TypedDict):
    exceptionTimeToLive: int,
    notificationEndpoint: str,
    subscriptionProtocol: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateSubscriberNotificationResponseTypeDef

```python
# UpdateSubscriberNotificationResponseTypeDef definition

class UpdateSubscriberNotificationResponseTypeDef(TypedDict):
    subscriberEndpoint: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    tags: List[TagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CustomLogSourceConfigurationTypeDef

```python
# CustomLogSourceConfigurationTypeDef definition

class CustomLogSourceConfigurationTypeDef(TypedDict):
    crawlerConfiguration: CustomLogSourceCrawlerConfigurationTypeDef,  # (1)
    providerIdentity: AwsIdentityTypeDef,  # (2)
```

1. See [:material-code-braces: CustomLogSourceCrawlerConfigurationTypeDef](./type_defs.md#customlogsourcecrawlerconfigurationtypedef) 
2. See [:material-code-braces: AwsIdentityTypeDef](./type_defs.md#awsidentitytypedef) 
## CustomLogSourceResourceTypeDef

```python
# CustomLogSourceResourceTypeDef definition

class CustomLogSourceResourceTypeDef(TypedDict):
    attributes: NotRequired[CustomLogSourceAttributesTypeDef],  # (1)
    provider: NotRequired[CustomLogSourceProviderTypeDef],  # (2)
    sourceName: NotRequired[str],
    sourceVersion: NotRequired[str],
```

1. See [:material-code-braces: CustomLogSourceAttributesTypeDef](./type_defs.md#customlogsourceattributestypedef) 
2. See [:material-code-braces: CustomLogSourceProviderTypeDef](./type_defs.md#customlogsourceprovidertypedef) 
## ListDataLakeExceptionsResponseTypeDef

```python
# ListDataLakeExceptionsResponseTypeDef definition

class ListDataLakeExceptionsResponseTypeDef(TypedDict):
    exceptions: List[DataLakeExceptionTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DataLakeExceptionTypeDef](./type_defs.md#datalakeexceptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DataLakeLifecycleConfigurationTypeDef

```python
# DataLakeLifecycleConfigurationTypeDef definition

class DataLakeLifecycleConfigurationTypeDef(TypedDict):
    expiration: NotRequired[DataLakeLifecycleExpirationTypeDef],  # (1)
    transitions: NotRequired[Sequence[DataLakeLifecycleTransitionTypeDef]],  # (2)
```

1. See [:material-code-braces: DataLakeLifecycleExpirationTypeDef](./type_defs.md#datalakelifecycleexpirationtypedef) 
2. See [:material-code-braces: DataLakeLifecycleTransitionTypeDef](./type_defs.md#datalakelifecycletransitiontypedef) 
## DataLakeSourceTypeDef

```python
# DataLakeSourceTypeDef definition

class DataLakeSourceTypeDef(TypedDict):
    account: NotRequired[str],
    eventClasses: NotRequired[List[str]],
    sourceName: NotRequired[str],
    sourceStatuses: NotRequired[List[DataLakeSourceStatusTypeDef]],  # (1)
```

1. See [:material-code-braces: DataLakeSourceStatusTypeDef](./type_defs.md#datalakesourcestatustypedef) 
## DataLakeUpdateStatusTypeDef

```python
# DataLakeUpdateStatusTypeDef definition

class DataLakeUpdateStatusTypeDef(TypedDict):
    exception: NotRequired[DataLakeUpdateExceptionTypeDef],  # (1)
    requestId: NotRequired[str],
    status: NotRequired[DataLakeStatusType],  # (2)
```

1. See [:material-code-braces: DataLakeUpdateExceptionTypeDef](./type_defs.md#datalakeupdateexceptiontypedef) 
2. See [:material-code-brackets: DataLakeStatusType](./literals.md#datalakestatustype) 
## GetDataLakeSourcesRequestGetDataLakeSourcesPaginateTypeDef

```python
# GetDataLakeSourcesRequestGetDataLakeSourcesPaginateTypeDef definition

class GetDataLakeSourcesRequestGetDataLakeSourcesPaginateTypeDef(TypedDict):
    accounts: NotRequired[Sequence[str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDataLakeExceptionsRequestListDataLakeExceptionsPaginateTypeDef

```python
# ListDataLakeExceptionsRequestListDataLakeExceptionsPaginateTypeDef definition

class ListDataLakeExceptionsRequestListDataLakeExceptionsPaginateTypeDef(TypedDict):
    regions: NotRequired[Sequence[str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListSubscribersRequestListSubscribersPaginateTypeDef

```python
# ListSubscribersRequestListSubscribersPaginateTypeDef definition

class ListSubscribersRequestListSubscribersPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## NotificationConfigurationTypeDef

```python
# NotificationConfigurationTypeDef definition

class NotificationConfigurationTypeDef(TypedDict):
    httpsNotificationConfiguration: NotRequired[HttpsNotificationConfigurationTypeDef],  # (1)
    sqsNotificationConfiguration: NotRequired[Mapping[str, Any]],
```

1. See [:material-code-braces: HttpsNotificationConfigurationTypeDef](./type_defs.md#httpsnotificationconfigurationtypedef) 
## CreateDataLakeOrganizationConfigurationRequestRequestTypeDef

```python
# CreateDataLakeOrganizationConfigurationRequestRequestTypeDef definition

class CreateDataLakeOrganizationConfigurationRequestRequestTypeDef(TypedDict):
    autoEnableNewAccount: Sequence[DataLakeAutoEnableNewAccountConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: DataLakeAutoEnableNewAccountConfigurationTypeDef](./type_defs.md#datalakeautoenablenewaccountconfigurationtypedef) 
## DeleteDataLakeOrganizationConfigurationRequestRequestTypeDef

```python
# DeleteDataLakeOrganizationConfigurationRequestRequestTypeDef definition

class DeleteDataLakeOrganizationConfigurationRequestRequestTypeDef(TypedDict):
    autoEnableNewAccount: Sequence[DataLakeAutoEnableNewAccountConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: DataLakeAutoEnableNewAccountConfigurationTypeDef](./type_defs.md#datalakeautoenablenewaccountconfigurationtypedef) 
## GetDataLakeOrganizationConfigurationResponseTypeDef

```python
# GetDataLakeOrganizationConfigurationResponseTypeDef definition

class GetDataLakeOrganizationConfigurationResponseTypeDef(TypedDict):
    autoEnableNewAccount: List[DataLakeAutoEnableNewAccountConfigurationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DataLakeAutoEnableNewAccountConfigurationTypeDef](./type_defs.md#datalakeautoenablenewaccountconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateCustomLogSourceRequestRequestTypeDef

```python
# CreateCustomLogSourceRequestRequestTypeDef definition

class CreateCustomLogSourceRequestRequestTypeDef(TypedDict):
    sourceName: str,
    configuration: NotRequired[CustomLogSourceConfigurationTypeDef],  # (1)
    eventClasses: NotRequired[Sequence[str]],
    sourceVersion: NotRequired[str],
```

1. See [:material-code-braces: CustomLogSourceConfigurationTypeDef](./type_defs.md#customlogsourceconfigurationtypedef) 
## CreateCustomLogSourceResponseTypeDef

```python
# CreateCustomLogSourceResponseTypeDef definition

class CreateCustomLogSourceResponseTypeDef(TypedDict):
    source: CustomLogSourceResourceTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CustomLogSourceResourceTypeDef](./type_defs.md#customlogsourceresourcetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## LogSourceResourceTypeDef

```python
# LogSourceResourceTypeDef definition

class LogSourceResourceTypeDef(TypedDict):
    awsLogSource: NotRequired[AwsLogSourceResourceTypeDef],  # (1)
    customLogSource: NotRequired[CustomLogSourceResourceTypeDef],  # (2)
```

1. See [:material-code-braces: AwsLogSourceResourceTypeDef](./type_defs.md#awslogsourceresourcetypedef) 
2. See [:material-code-braces: CustomLogSourceResourceTypeDef](./type_defs.md#customlogsourceresourcetypedef) 
## DataLakeConfigurationTypeDef

```python
# DataLakeConfigurationTypeDef definition

class DataLakeConfigurationTypeDef(TypedDict):
    region: str,
    encryptionConfiguration: NotRequired[DataLakeEncryptionConfigurationTypeDef],  # (1)
    lifecycleConfiguration: NotRequired[DataLakeLifecycleConfigurationTypeDef],  # (2)
    replicationConfiguration: NotRequired[DataLakeReplicationConfigurationTypeDef],  # (3)
```

1. See [:material-code-braces: DataLakeEncryptionConfigurationTypeDef](./type_defs.md#datalakeencryptionconfigurationtypedef) 
2. See [:material-code-braces: DataLakeLifecycleConfigurationTypeDef](./type_defs.md#datalakelifecycleconfigurationtypedef) 
3. See [:material-code-braces: DataLakeReplicationConfigurationTypeDef](./type_defs.md#datalakereplicationconfigurationtypedef) 
## GetDataLakeSourcesResponseTypeDef

```python
# GetDataLakeSourcesResponseTypeDef definition

class GetDataLakeSourcesResponseTypeDef(TypedDict):
    dataLakeArn: str,
    dataLakeSources: List[DataLakeSourceTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DataLakeSourceTypeDef](./type_defs.md#datalakesourcetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DataLakeResourceTypeDef

```python
# DataLakeResourceTypeDef definition

class DataLakeResourceTypeDef(TypedDict):
    dataLakeArn: str,
    region: str,
    createStatus: NotRequired[DataLakeStatusType],  # (1)
    encryptionConfiguration: NotRequired[DataLakeEncryptionConfigurationTypeDef],  # (2)
    lifecycleConfiguration: NotRequired[DataLakeLifecycleConfigurationTypeDef],  # (3)
    replicationConfiguration: NotRequired[DataLakeReplicationConfigurationTypeDef],  # (4)
    s3BucketArn: NotRequired[str],
    updateStatus: NotRequired[DataLakeUpdateStatusTypeDef],  # (5)
```

1. See [:material-code-brackets: DataLakeStatusType](./literals.md#datalakestatustype) 
2. See [:material-code-braces: DataLakeEncryptionConfigurationTypeDef](./type_defs.md#datalakeencryptionconfigurationtypedef) 
3. See [:material-code-braces: DataLakeLifecycleConfigurationTypeDef](./type_defs.md#datalakelifecycleconfigurationtypedef) 
4. See [:material-code-braces: DataLakeReplicationConfigurationTypeDef](./type_defs.md#datalakereplicationconfigurationtypedef) 
5. See [:material-code-braces: DataLakeUpdateStatusTypeDef](./type_defs.md#datalakeupdatestatustypedef) 
## CreateSubscriberNotificationRequestRequestTypeDef

```python
# CreateSubscriberNotificationRequestRequestTypeDef definition

class CreateSubscriberNotificationRequestRequestTypeDef(TypedDict):
    configuration: NotificationConfigurationTypeDef,  # (1)
    subscriberId: str,
```

1. See [:material-code-braces: NotificationConfigurationTypeDef](./type_defs.md#notificationconfigurationtypedef) 
## UpdateSubscriberNotificationRequestRequestTypeDef

```python
# UpdateSubscriberNotificationRequestRequestTypeDef definition

class UpdateSubscriberNotificationRequestRequestTypeDef(TypedDict):
    configuration: NotificationConfigurationTypeDef,  # (1)
    subscriberId: str,
```

1. See [:material-code-braces: NotificationConfigurationTypeDef](./type_defs.md#notificationconfigurationtypedef) 
## CreateSubscriberRequestRequestTypeDef

```python
# CreateSubscriberRequestRequestTypeDef definition

class CreateSubscriberRequestRequestTypeDef(TypedDict):
    sources: Sequence[LogSourceResourceTypeDef],  # (1)
    subscriberIdentity: AwsIdentityTypeDef,  # (2)
    subscriberName: str,
    accessTypes: NotRequired[Sequence[AccessTypeType]],  # (3)
    subscriberDescription: NotRequired[str],
    tags: NotRequired[Sequence[TagTypeDef]],  # (4)
```

1. See [:material-code-braces: LogSourceResourceTypeDef](./type_defs.md#logsourceresourcetypedef) 
2. See [:material-code-braces: AwsIdentityTypeDef](./type_defs.md#awsidentitytypedef) 
3. See [:material-code-brackets: AccessTypeType](./literals.md#accesstypetype) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## ListLogSourcesRequestListLogSourcesPaginateTypeDef

```python
# ListLogSourcesRequestListLogSourcesPaginateTypeDef definition

class ListLogSourcesRequestListLogSourcesPaginateTypeDef(TypedDict):
    accounts: NotRequired[Sequence[str]],
    regions: NotRequired[Sequence[str]],
    sources: NotRequired[Sequence[LogSourceResourceTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: LogSourceResourceTypeDef](./type_defs.md#logsourceresourcetypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListLogSourcesRequestRequestTypeDef

```python
# ListLogSourcesRequestRequestTypeDef definition

class ListLogSourcesRequestRequestTypeDef(TypedDict):
    accounts: NotRequired[Sequence[str]],
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    regions: NotRequired[Sequence[str]],
    sources: NotRequired[Sequence[LogSourceResourceTypeDef]],  # (1)
```

1. See [:material-code-braces: LogSourceResourceTypeDef](./type_defs.md#logsourceresourcetypedef) 
## LogSourceTypeDef

```python
# LogSourceTypeDef definition

class LogSourceTypeDef(TypedDict):
    account: NotRequired[str],
    region: NotRequired[str],
    sources: NotRequired[List[LogSourceResourceTypeDef]],  # (1)
```

1. See [:material-code-braces: LogSourceResourceTypeDef](./type_defs.md#logsourceresourcetypedef) 
## SubscriberResourceTypeDef

```python
# SubscriberResourceTypeDef definition

class SubscriberResourceTypeDef(TypedDict):
    sources: List[LogSourceResourceTypeDef],  # (2)
    subscriberArn: str,
    subscriberId: str,
    subscriberIdentity: AwsIdentityTypeDef,  # (3)
    subscriberName: str,
    accessTypes: NotRequired[List[AccessTypeType]],  # (1)
    createdAt: NotRequired[datetime],
    resourceShareArn: NotRequired[str],
    resourceShareName: NotRequired[str],
    roleArn: NotRequired[str],
    s3BucketArn: NotRequired[str],
    subscriberDescription: NotRequired[str],
    subscriberEndpoint: NotRequired[str],
    subscriberStatus: NotRequired[SubscriberStatusType],  # (4)
    updatedAt: NotRequired[datetime],
```

1. See [:material-code-brackets: AccessTypeType](./literals.md#accesstypetype) 
2. See [:material-code-braces: LogSourceResourceTypeDef](./type_defs.md#logsourceresourcetypedef) 
3. See [:material-code-braces: AwsIdentityTypeDef](./type_defs.md#awsidentitytypedef) 
4. See [:material-code-brackets: SubscriberStatusType](./literals.md#subscriberstatustype) 
## UpdateSubscriberRequestRequestTypeDef

```python
# UpdateSubscriberRequestRequestTypeDef definition

class UpdateSubscriberRequestRequestTypeDef(TypedDict):
    subscriberId: str,
    sources: NotRequired[Sequence[LogSourceResourceTypeDef]],  # (1)
    subscriberDescription: NotRequired[str],
    subscriberIdentity: NotRequired[AwsIdentityTypeDef],  # (2)
    subscriberName: NotRequired[str],
```

1. See [:material-code-braces: LogSourceResourceTypeDef](./type_defs.md#logsourceresourcetypedef) 
2. See [:material-code-braces: AwsIdentityTypeDef](./type_defs.md#awsidentitytypedef) 
## CreateDataLakeRequestRequestTypeDef

```python
# CreateDataLakeRequestRequestTypeDef definition

class CreateDataLakeRequestRequestTypeDef(TypedDict):
    configurations: Sequence[DataLakeConfigurationTypeDef],  # (1)
    metaStoreManagerRoleArn: str,
    tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-braces: DataLakeConfigurationTypeDef](./type_defs.md#datalakeconfigurationtypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## UpdateDataLakeRequestRequestTypeDef

```python
# UpdateDataLakeRequestRequestTypeDef definition

class UpdateDataLakeRequestRequestTypeDef(TypedDict):
    configurations: Sequence[DataLakeConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: DataLakeConfigurationTypeDef](./type_defs.md#datalakeconfigurationtypedef) 
## CreateDataLakeResponseTypeDef

```python
# CreateDataLakeResponseTypeDef definition

class CreateDataLakeResponseTypeDef(TypedDict):
    dataLakes: List[DataLakeResourceTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DataLakeResourceTypeDef](./type_defs.md#datalakeresourcetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDataLakesResponseTypeDef

```python
# ListDataLakesResponseTypeDef definition

class ListDataLakesResponseTypeDef(TypedDict):
    dataLakes: List[DataLakeResourceTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DataLakeResourceTypeDef](./type_defs.md#datalakeresourcetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateDataLakeResponseTypeDef

```python
# UpdateDataLakeResponseTypeDef definition

class UpdateDataLakeResponseTypeDef(TypedDict):
    dataLakes: List[DataLakeResourceTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DataLakeResourceTypeDef](./type_defs.md#datalakeresourcetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListLogSourcesResponseTypeDef

```python
# ListLogSourcesResponseTypeDef definition

class ListLogSourcesResponseTypeDef(TypedDict):
    nextToken: str,
    sources: List[LogSourceTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LogSourceTypeDef](./type_defs.md#logsourcetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateSubscriberResponseTypeDef

```python
# CreateSubscriberResponseTypeDef definition

class CreateSubscriberResponseTypeDef(TypedDict):
    subscriber: SubscriberResourceTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SubscriberResourceTypeDef](./type_defs.md#subscriberresourcetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetSubscriberResponseTypeDef

```python
# GetSubscriberResponseTypeDef definition

class GetSubscriberResponseTypeDef(TypedDict):
    subscriber: SubscriberResourceTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SubscriberResourceTypeDef](./type_defs.md#subscriberresourcetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListSubscribersResponseTypeDef

```python
# ListSubscribersResponseTypeDef definition

class ListSubscribersResponseTypeDef(TypedDict):
    nextToken: str,
    subscribers: List[SubscriberResourceTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SubscriberResourceTypeDef](./type_defs.md#subscriberresourcetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateSubscriberResponseTypeDef

```python
# UpdateSubscriberResponseTypeDef definition

class UpdateSubscriberResponseTypeDef(TypedDict):
    subscriber: SubscriberResourceTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SubscriberResourceTypeDef](./type_defs.md#subscriberresourcetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
