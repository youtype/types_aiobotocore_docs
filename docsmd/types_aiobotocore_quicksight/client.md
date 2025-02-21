# QuickSightClient

> [Index](../README.md) > [QuickSight](./README.md) > QuickSightClient

!!! note ""

    Auto-generated documentation for [QuickSight](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#quicksight)
    type annotations stubs module [types-aiobotocore-quicksight](https://pypi.org/project/types-aiobotocore-quicksight/).

## QuickSightClient

Type annotations and code completion for `#!python session.create_client("quicksight")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client)

```python
# QuickSightClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_quicksight.client import QuickSightClient

session = get_session()
async with session.create_client("quicksight") as client:
    client: QuickSightClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("quicksight").exceptions` structure.

```python
# QuickSightClient.exceptions usage example

async with session.create_client("quicksight") as client:
    try:
        do_something(client)
    except (
            client.AccessDeniedException,
        client.ClientError,
        client.ConcurrentUpdatingException,
        client.ConflictException,
        client.CustomerManagedKeyUnavailableException,
        client.DomainNotWhitelistedException,
        client.IdentityTypeNotSupportedException,
        client.InternalFailureException,
        client.InternalServerException,
        client.InvalidNextTokenException,
        client.InvalidParameterValueException,
        client.InvalidRequestException,
        client.LimitExceededException,
        client.PreconditionNotMetException,
        client.QuickSightUserNotFoundException,
        client.ResourceExistsException,
        client.ResourceNotFoundException,
        client.ResourceUnavailableException,
        client.SessionLifetimeInMinutesInvalidException,
        client.ThrottlingException,
        client.UnsupportedPricingPlanException,
        client.UnsupportedUserEditionException,
    ) as e:
        print(e)
```

```python
# QuickSightClient usage type checking example

from types_aiobotocore_quicksight.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("quicksight").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("quicksight").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/generate_presigned_url.html)

```python
# generate_presigned_url method definition

await def generate_presigned_url(
    self,
    ClientMethod: str,
    Params: Mapping[str, Any] = ...,
    ExpiresIn: int = 3600,
    HttpMethod: str = ...,
) -> str:
    ...
```


### batch\_create\_topic\_reviewed\_answer

Creates new reviewed answers for a Q Topic.

Type annotations and code completion for `#!python session.create_client("quicksight").batch_create_topic_reviewed_answer` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/batch_create_topic_reviewed_answer.html)

```python
# batch_create_topic_reviewed_answer method definition

await def batch_create_topic_reviewed_answer(
    self,
    *,
    AwsAccountId: str,
    TopicId: str,
    Answers: Sequence[CreateTopicReviewedAnswerTypeDef],  # (1)
) -> BatchCreateTopicReviewedAnswerResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: CreateTopicReviewedAnswerTypeDef](./type_defs.md#createtopicreviewedanswertypedef) 
2. See [:material-code-braces: BatchCreateTopicReviewedAnswerResponseTypeDef](./type_defs.md#batchcreatetopicreviewedanswerresponsetypedef) 


```python
# batch_create_topic_reviewed_answer method usage example with argument unpacking

kwargs: BatchCreateTopicReviewedAnswerRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "TopicId": ...,
    "Answers": ...,
}

parent.batch_create_topic_reviewed_answer(**kwargs)
```

1. See [:material-code-braces: BatchCreateTopicReviewedAnswerRequestTypeDef](./type_defs.md#batchcreatetopicreviewedanswerrequesttypedef) 

### batch\_delete\_topic\_reviewed\_answer

Deletes reviewed answers for Q Topic.

Type annotations and code completion for `#!python session.create_client("quicksight").batch_delete_topic_reviewed_answer` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/batch_delete_topic_reviewed_answer.html)

```python
# batch_delete_topic_reviewed_answer method definition

await def batch_delete_topic_reviewed_answer(
    self,
    *,
    AwsAccountId: str,
    TopicId: str,
    AnswerIds: Sequence[str] = ...,
) -> BatchDeleteTopicReviewedAnswerResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: BatchDeleteTopicReviewedAnswerResponseTypeDef](./type_defs.md#batchdeletetopicreviewedanswerresponsetypedef) 


```python
# batch_delete_topic_reviewed_answer method usage example with argument unpacking

kwargs: BatchDeleteTopicReviewedAnswerRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "TopicId": ...,
}

parent.batch_delete_topic_reviewed_answer(**kwargs)
```

1. See [:material-code-braces: BatchDeleteTopicReviewedAnswerRequestTypeDef](./type_defs.md#batchdeletetopicreviewedanswerrequesttypedef) 

### cancel\_ingestion

Cancels an ongoing ingestion of data into SPICE.

Type annotations and code completion for `#!python session.create_client("quicksight").cancel_ingestion` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/cancel_ingestion.html)

```python
# cancel_ingestion method definition

await def cancel_ingestion(
    self,
    *,
    AwsAccountId: str,
    DataSetId: str,
    IngestionId: str,
) -> CancelIngestionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CancelIngestionResponseTypeDef](./type_defs.md#cancelingestionresponsetypedef) 


```python
# cancel_ingestion method usage example with argument unpacking

kwargs: CancelIngestionRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "DataSetId": ...,
    "IngestionId": ...,
}

parent.cancel_ingestion(**kwargs)
```

1. See [:material-code-braces: CancelIngestionRequestTypeDef](./type_defs.md#cancelingestionrequesttypedef) 

### create\_account\_customization

Creates Amazon QuickSight customizations for the current Amazon Web Services
Region.

Type annotations and code completion for `#!python session.create_client("quicksight").create_account_customization` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/create_account_customization.html)

```python
# create_account_customization method definition

await def create_account_customization(
    self,
    *,
    AwsAccountId: str,
    AccountCustomization: AccountCustomizationTypeDef,  # (1)
    Namespace: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (2)
) -> CreateAccountCustomizationResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: AccountCustomizationTypeDef](./type_defs.md#accountcustomizationtypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: CreateAccountCustomizationResponseTypeDef](./type_defs.md#createaccountcustomizationresponsetypedef) 


```python
# create_account_customization method usage example with argument unpacking

kwargs: CreateAccountCustomizationRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "AccountCustomization": ...,
}

parent.create_account_customization(**kwargs)
```

1. See [:material-code-braces: CreateAccountCustomizationRequestTypeDef](./type_defs.md#createaccountcustomizationrequesttypedef) 

### create\_account\_subscription

Creates an Amazon QuickSight account, or subscribes to Amazon QuickSight Q.

Type annotations and code completion for `#!python session.create_client("quicksight").create_account_subscription` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/create_account_subscription.html)

```python
# create_account_subscription method definition

await def create_account_subscription(
    self,
    *,
    AuthenticationMethod: AuthenticationMethodOptionType,  # (1)
    AwsAccountId: str,
    AccountName: str,
    NotificationEmail: str,
    Edition: EditionType = ...,  # (2)
    ActiveDirectoryName: str = ...,
    Realm: str = ...,
    DirectoryId: str = ...,
    AdminGroup: Sequence[str] = ...,
    AuthorGroup: Sequence[str] = ...,
    ReaderGroup: Sequence[str] = ...,
    AdminProGroup: Sequence[str] = ...,
    AuthorProGroup: Sequence[str] = ...,
    ReaderProGroup: Sequence[str] = ...,
    FirstName: str = ...,
    LastName: str = ...,
    EmailAddress: str = ...,
    ContactNumber: str = ...,
    IAMIdentityCenterInstanceArn: str = ...,
) -> CreateAccountSubscriptionResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: AuthenticationMethodOptionType](./literals.md#authenticationmethodoptiontype) 
2. See [:material-code-brackets: EditionType](./literals.md#editiontype) 
3. See [:material-code-braces: CreateAccountSubscriptionResponseTypeDef](./type_defs.md#createaccountsubscriptionresponsetypedef) 


```python
# create_account_subscription method usage example with argument unpacking

kwargs: CreateAccountSubscriptionRequestTypeDef = {  # (1)
    "AuthenticationMethod": ...,
    "AwsAccountId": ...,
    "AccountName": ...,
    "NotificationEmail": ...,
}

parent.create_account_subscription(**kwargs)
```

1. See [:material-code-braces: CreateAccountSubscriptionRequestTypeDef](./type_defs.md#createaccountsubscriptionrequesttypedef) 

### create\_analysis

Creates an analysis in Amazon QuickSight.

Type annotations and code completion for `#!python session.create_client("quicksight").create_analysis` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/create_analysis.html)

```python
# create_analysis method definition

await def create_analysis(
    self,
    *,
    AwsAccountId: str,
    AnalysisId: str,
    Name: str,
    Parameters: ParametersUnionTypeDef = ...,  # (1)
    Permissions: Sequence[ResourcePermissionUnionTypeDef] = ...,  # (2)
    SourceEntity: AnalysisSourceEntityTypeDef = ...,  # (3)
    ThemeArn: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (4)
    Definition: AnalysisDefinitionUnionTypeDef = ...,  # (5)
    ValidationStrategy: ValidationStrategyTypeDef = ...,  # (6)
    FolderArns: Sequence[str] = ...,
) -> CreateAnalysisResponseTypeDef:  # (7)
    ...
```

1. See [:material-code-braces: ParametersTypeDef](./type_defs.md#parameterstypedef) [:material-code-braces: ParametersOutputTypeDef](./type_defs.md#parametersoutputtypedef) 
2. See [:material-code-braces: ResourcePermissionTypeDef](./type_defs.md#resourcepermissiontypedef) [:material-code-braces: ResourcePermissionOutputTypeDef](./type_defs.md#resourcepermissionoutputtypedef) 
3. See [:material-code-braces: AnalysisSourceEntityTypeDef](./type_defs.md#analysissourceentitytypedef) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
5. See [:material-code-braces: AnalysisDefinitionTypeDef](./type_defs.md#analysisdefinitiontypedef) [:material-code-braces: AnalysisDefinitionOutputTypeDef](./type_defs.md#analysisdefinitionoutputtypedef) 
6. See [:material-code-braces: ValidationStrategyTypeDef](./type_defs.md#validationstrategytypedef) 
7. See [:material-code-braces: CreateAnalysisResponseTypeDef](./type_defs.md#createanalysisresponsetypedef) 


```python
# create_analysis method usage example with argument unpacking

kwargs: CreateAnalysisRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "AnalysisId": ...,
    "Name": ...,
}

parent.create_analysis(**kwargs)
```

1. See [:material-code-braces: CreateAnalysisRequestTypeDef](./type_defs.md#createanalysisrequesttypedef) 

### create\_brand

Creates an Amazon QuickSight brand.

Type annotations and code completion for `#!python session.create_client("quicksight").create_brand` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/create_brand.html)

```python
# create_brand method definition

await def create_brand(
    self,
    *,
    AwsAccountId: str,
    BrandId: str,
    BrandDefinition: BrandDefinitionTypeDef = ...,  # (1)
    Tags: Sequence[TagTypeDef] = ...,  # (2)
) -> CreateBrandResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: BrandDefinitionTypeDef](./type_defs.md#branddefinitiontypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: CreateBrandResponseTypeDef](./type_defs.md#createbrandresponsetypedef) 


```python
# create_brand method usage example with argument unpacking

kwargs: CreateBrandRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "BrandId": ...,
}

parent.create_brand(**kwargs)
```

1. See [:material-code-braces: CreateBrandRequestTypeDef](./type_defs.md#createbrandrequesttypedef) 

### create\_custom\_permissions

Creates a custom permissions profile.

Type annotations and code completion for `#!python session.create_client("quicksight").create_custom_permissions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/create_custom_permissions.html)

```python
# create_custom_permissions method definition

await def create_custom_permissions(
    self,
    *,
    AwsAccountId: str,
    CustomPermissionsName: str,
    Capabilities: CapabilitiesTypeDef = ...,  # (1)
    Tags: Sequence[TagTypeDef] = ...,  # (2)
) -> CreateCustomPermissionsResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: CapabilitiesTypeDef](./type_defs.md#capabilitiestypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: CreateCustomPermissionsResponseTypeDef](./type_defs.md#createcustompermissionsresponsetypedef) 


```python
# create_custom_permissions method usage example with argument unpacking

kwargs: CreateCustomPermissionsRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "CustomPermissionsName": ...,
}

parent.create_custom_permissions(**kwargs)
```

1. See [:material-code-braces: CreateCustomPermissionsRequestTypeDef](./type_defs.md#createcustompermissionsrequesttypedef) 

### create\_dashboard

Creates a dashboard from either a template or directly with a
<code>DashboardDefinition</code>.

Type annotations and code completion for `#!python session.create_client("quicksight").create_dashboard` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/create_dashboard.html)

```python
# create_dashboard method definition

await def create_dashboard(
    self,
    *,
    AwsAccountId: str,
    DashboardId: str,
    Name: str,
    Parameters: ParametersUnionTypeDef = ...,  # (1)
    Permissions: Sequence[ResourcePermissionUnionTypeDef] = ...,  # (2)
    SourceEntity: DashboardSourceEntityTypeDef = ...,  # (3)
    Tags: Sequence[TagTypeDef] = ...,  # (4)
    VersionDescription: str = ...,
    DashboardPublishOptions: DashboardPublishOptionsTypeDef = ...,  # (5)
    ThemeArn: str = ...,
    Definition: DashboardVersionDefinitionUnionTypeDef = ...,  # (6)
    ValidationStrategy: ValidationStrategyTypeDef = ...,  # (7)
    FolderArns: Sequence[str] = ...,
    LinkSharingConfiguration: LinkSharingConfigurationUnionTypeDef = ...,  # (8)
    LinkEntities: Sequence[str] = ...,
) -> CreateDashboardResponseTypeDef:  # (9)
    ...
```

1. See [:material-code-braces: ParametersTypeDef](./type_defs.md#parameterstypedef) [:material-code-braces: ParametersOutputTypeDef](./type_defs.md#parametersoutputtypedef) 
2. See [:material-code-braces: ResourcePermissionTypeDef](./type_defs.md#resourcepermissiontypedef) [:material-code-braces: ResourcePermissionOutputTypeDef](./type_defs.md#resourcepermissionoutputtypedef) 
3. See [:material-code-braces: DashboardSourceEntityTypeDef](./type_defs.md#dashboardsourceentitytypedef) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
5. See [:material-code-braces: DashboardPublishOptionsTypeDef](./type_defs.md#dashboardpublishoptionstypedef) 
6. See [:material-code-braces: DashboardVersionDefinitionTypeDef](./type_defs.md#dashboardversiondefinitiontypedef) [:material-code-braces: DashboardVersionDefinitionOutputTypeDef](./type_defs.md#dashboardversiondefinitionoutputtypedef) 
7. See [:material-code-braces: ValidationStrategyTypeDef](./type_defs.md#validationstrategytypedef) 
8. See [:material-code-braces: LinkSharingConfigurationTypeDef](./type_defs.md#linksharingconfigurationtypedef) [:material-code-braces: LinkSharingConfigurationOutputTypeDef](./type_defs.md#linksharingconfigurationoutputtypedef) 
9. See [:material-code-braces: CreateDashboardResponseTypeDef](./type_defs.md#createdashboardresponsetypedef) 


```python
# create_dashboard method usage example with argument unpacking

kwargs: CreateDashboardRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "DashboardId": ...,
    "Name": ...,
}

parent.create_dashboard(**kwargs)
```

1. See [:material-code-braces: CreateDashboardRequestTypeDef](./type_defs.md#createdashboardrequesttypedef) 

### create\_data\_set

Creates a dataset.

Type annotations and code completion for `#!python session.create_client("quicksight").create_data_set` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/create_data_set.html)

```python
# create_data_set method definition

await def create_data_set(
    self,
    *,
    AwsAccountId: str,
    DataSetId: str,
    Name: str,
    PhysicalTableMap: Mapping[str, PhysicalTableUnionTypeDef],  # (1)
    ImportMode: DataSetImportModeType,  # (2)
    LogicalTableMap: Mapping[str, LogicalTableUnionTypeDef] = ...,  # (3)
    ColumnGroups: Sequence[ColumnGroupUnionTypeDef] = ...,  # (4)
    FieldFolders: Mapping[str, FieldFolderUnionTypeDef] = ...,  # (5)
    Permissions: Sequence[ResourcePermissionUnionTypeDef] = ...,  # (6)
    RowLevelPermissionDataSet: RowLevelPermissionDataSetTypeDef = ...,  # (7)
    RowLevelPermissionTagConfiguration: RowLevelPermissionTagConfigurationUnionTypeDef = ...,  # (8)
    ColumnLevelPermissionRules: Sequence[ColumnLevelPermissionRuleUnionTypeDef] = ...,  # (9)
    Tags: Sequence[TagTypeDef] = ...,  # (10)
    DataSetUsageConfiguration: DataSetUsageConfigurationTypeDef = ...,  # (11)
    DatasetParameters: Sequence[DatasetParameterUnionTypeDef] = ...,  # (12)
    FolderArns: Sequence[str] = ...,
    PerformanceConfiguration: PerformanceConfigurationUnionTypeDef = ...,  # (13)
) -> CreateDataSetResponseTypeDef:  # (14)
    ...
```

1. See [:material-code-braces: PhysicalTableTypeDef](./type_defs.md#physicaltabletypedef) [:material-code-braces: PhysicalTableOutputTypeDef](./type_defs.md#physicaltableoutputtypedef) 
2. See [:material-code-brackets: DataSetImportModeType](./literals.md#datasetimportmodetype) 
3. See [:material-code-braces: LogicalTableTypeDef](./type_defs.md#logicaltabletypedef) [:material-code-braces: LogicalTableOutputTypeDef](./type_defs.md#logicaltableoutputtypedef) 
4. See [:material-code-braces: ColumnGroupTypeDef](./type_defs.md#columngrouptypedef) [:material-code-braces: ColumnGroupOutputTypeDef](./type_defs.md#columngroupoutputtypedef) 
5. See [:material-code-braces: FieldFolderTypeDef](./type_defs.md#fieldfoldertypedef) [:material-code-braces: FieldFolderOutputTypeDef](./type_defs.md#fieldfolderoutputtypedef) 
6. See [:material-code-braces: ResourcePermissionTypeDef](./type_defs.md#resourcepermissiontypedef) [:material-code-braces: ResourcePermissionOutputTypeDef](./type_defs.md#resourcepermissionoutputtypedef) 
7. See [:material-code-braces: RowLevelPermissionDataSetTypeDef](./type_defs.md#rowlevelpermissiondatasettypedef) 
8. See [:material-code-braces: RowLevelPermissionTagConfigurationTypeDef](./type_defs.md#rowlevelpermissiontagconfigurationtypedef) [:material-code-braces: RowLevelPermissionTagConfigurationOutputTypeDef](./type_defs.md#rowlevelpermissiontagconfigurationoutputtypedef) 
9. See [:material-code-braces: ColumnLevelPermissionRuleTypeDef](./type_defs.md#columnlevelpermissionruletypedef) [:material-code-braces: ColumnLevelPermissionRuleOutputTypeDef](./type_defs.md#columnlevelpermissionruleoutputtypedef) 
10. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
11. See [:material-code-braces: DataSetUsageConfigurationTypeDef](./type_defs.md#datasetusageconfigurationtypedef) 
12. See [:material-code-braces: DatasetParameterTypeDef](./type_defs.md#datasetparametertypedef) [:material-code-braces: DatasetParameterOutputTypeDef](./type_defs.md#datasetparameteroutputtypedef) 
13. See [:material-code-braces: PerformanceConfigurationTypeDef](./type_defs.md#performanceconfigurationtypedef) [:material-code-braces: PerformanceConfigurationOutputTypeDef](./type_defs.md#performanceconfigurationoutputtypedef) 
14. See [:material-code-braces: CreateDataSetResponseTypeDef](./type_defs.md#createdatasetresponsetypedef) 


```python
# create_data_set method usage example with argument unpacking

kwargs: CreateDataSetRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "DataSetId": ...,
    "Name": ...,
    "PhysicalTableMap": ...,
    "ImportMode": ...,
}

parent.create_data_set(**kwargs)
```

1. See [:material-code-braces: CreateDataSetRequestTypeDef](./type_defs.md#createdatasetrequesttypedef) 

### create\_data\_source

Creates a data source.

Type annotations and code completion for `#!python session.create_client("quicksight").create_data_source` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/create_data_source.html)

```python
# create_data_source method definition

await def create_data_source(
    self,
    *,
    AwsAccountId: str,
    DataSourceId: str,
    Name: str,
    Type: DataSourceTypeType,  # (1)
    DataSourceParameters: DataSourceParametersUnionTypeDef = ...,  # (2)
    Credentials: DataSourceCredentialsTypeDef = ...,  # (3)
    Permissions: Sequence[ResourcePermissionUnionTypeDef] = ...,  # (4)
    VpcConnectionProperties: VpcConnectionPropertiesTypeDef = ...,  # (5)
    SslProperties: SslPropertiesTypeDef = ...,  # (6)
    Tags: Sequence[TagTypeDef] = ...,  # (7)
    FolderArns: Sequence[str] = ...,
) -> CreateDataSourceResponseTypeDef:  # (8)
    ...
```

1. See [:material-code-brackets: DataSourceTypeType](./literals.md#datasourcetypetype) 
2. See [:material-code-braces: DataSourceParametersTypeDef](./type_defs.md#datasourceparameterstypedef) [:material-code-braces: DataSourceParametersOutputTypeDef](./type_defs.md#datasourceparametersoutputtypedef) 
3. See [:material-code-braces: DataSourceCredentialsTypeDef](./type_defs.md#datasourcecredentialstypedef) 
4. See [:material-code-braces: ResourcePermissionTypeDef](./type_defs.md#resourcepermissiontypedef) [:material-code-braces: ResourcePermissionOutputTypeDef](./type_defs.md#resourcepermissionoutputtypedef) 
5. See [:material-code-braces: VpcConnectionPropertiesTypeDef](./type_defs.md#vpcconnectionpropertiestypedef) 
6. See [:material-code-braces: SslPropertiesTypeDef](./type_defs.md#sslpropertiestypedef) 
7. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
8. See [:material-code-braces: CreateDataSourceResponseTypeDef](./type_defs.md#createdatasourceresponsetypedef) 


```python
# create_data_source method usage example with argument unpacking

kwargs: CreateDataSourceRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "DataSourceId": ...,
    "Name": ...,
    "Type": ...,
}

parent.create_data_source(**kwargs)
```

1. See [:material-code-braces: CreateDataSourceRequestTypeDef](./type_defs.md#createdatasourcerequesttypedef) 

### create\_folder

Creates an empty shared folder.

Type annotations and code completion for `#!python session.create_client("quicksight").create_folder` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/create_folder.html)

```python
# create_folder method definition

await def create_folder(
    self,
    *,
    AwsAccountId: str,
    FolderId: str,
    Name: str = ...,
    FolderType: FolderTypeType = ...,  # (1)
    ParentFolderArn: str = ...,
    Permissions: Sequence[ResourcePermissionUnionTypeDef] = ...,  # (2)
    Tags: Sequence[TagTypeDef] = ...,  # (3)
    SharingModel: SharingModelType = ...,  # (4)
) -> CreateFolderResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-brackets: FolderTypeType](./literals.md#foldertypetype) 
2. See [:material-code-braces: ResourcePermissionTypeDef](./type_defs.md#resourcepermissiontypedef) [:material-code-braces: ResourcePermissionOutputTypeDef](./type_defs.md#resourcepermissionoutputtypedef) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
4. See [:material-code-brackets: SharingModelType](./literals.md#sharingmodeltype) 
5. See [:material-code-braces: CreateFolderResponseTypeDef](./type_defs.md#createfolderresponsetypedef) 


```python
# create_folder method usage example with argument unpacking

kwargs: CreateFolderRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "FolderId": ...,
}

parent.create_folder(**kwargs)
```

1. See [:material-code-braces: CreateFolderRequestTypeDef](./type_defs.md#createfolderrequesttypedef) 

### create\_folder\_membership

Adds an asset, such as a dashboard, analysis, or dataset into a folder.

Type annotations and code completion for `#!python session.create_client("quicksight").create_folder_membership` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/create_folder_membership.html)

```python
# create_folder_membership method definition

await def create_folder_membership(
    self,
    *,
    AwsAccountId: str,
    FolderId: str,
    MemberId: str,
    MemberType: MemberTypeType,  # (1)
) -> CreateFolderMembershipResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: MemberTypeType](./literals.md#membertypetype) 
2. See [:material-code-braces: CreateFolderMembershipResponseTypeDef](./type_defs.md#createfoldermembershipresponsetypedef) 


```python
# create_folder_membership method usage example with argument unpacking

kwargs: CreateFolderMembershipRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "FolderId": ...,
    "MemberId": ...,
    "MemberType": ...,
}

parent.create_folder_membership(**kwargs)
```

1. See [:material-code-braces: CreateFolderMembershipRequestTypeDef](./type_defs.md#createfoldermembershiprequesttypedef) 

### create\_group

Use the <code>CreateGroup</code> operation to create a group in Amazon
QuickSight.

Type annotations and code completion for `#!python session.create_client("quicksight").create_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/create_group.html)

```python
# create_group method definition

await def create_group(
    self,
    *,
    GroupName: str,
    AwsAccountId: str,
    Namespace: str,
    Description: str = ...,
) -> CreateGroupResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateGroupResponseTypeDef](./type_defs.md#creategroupresponsetypedef) 


```python
# create_group method usage example with argument unpacking

kwargs: CreateGroupRequestTypeDef = {  # (1)
    "GroupName": ...,
    "AwsAccountId": ...,
    "Namespace": ...,
}

parent.create_group(**kwargs)
```

1. See [:material-code-braces: CreateGroupRequestTypeDef](./type_defs.md#creategrouprequesttypedef) 

### create\_group\_membership

Adds an Amazon QuickSight user to an Amazon QuickSight group.

Type annotations and code completion for `#!python session.create_client("quicksight").create_group_membership` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/create_group_membership.html)

```python
# create_group_membership method definition

await def create_group_membership(
    self,
    *,
    MemberName: str,
    GroupName: str,
    AwsAccountId: str,
    Namespace: str,
) -> CreateGroupMembershipResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateGroupMembershipResponseTypeDef](./type_defs.md#creategroupmembershipresponsetypedef) 


```python
# create_group_membership method usage example with argument unpacking

kwargs: CreateGroupMembershipRequestTypeDef = {  # (1)
    "MemberName": ...,
    "GroupName": ...,
    "AwsAccountId": ...,
    "Namespace": ...,
}

parent.create_group_membership(**kwargs)
```

1. See [:material-code-braces: CreateGroupMembershipRequestTypeDef](./type_defs.md#creategroupmembershiprequesttypedef) 

### create\_iam\_policy\_assignment

Creates an assignment with one specified IAM policy, identified by its Amazon
Resource Name (ARN).

Type annotations and code completion for `#!python session.create_client("quicksight").create_iam_policy_assignment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/create_iam_policy_assignment.html)

```python
# create_iam_policy_assignment method definition

await def create_iam_policy_assignment(
    self,
    *,
    AwsAccountId: str,
    AssignmentName: str,
    AssignmentStatus: AssignmentStatusType,  # (1)
    Namespace: str,
    PolicyArn: str = ...,
    Identities: Mapping[str, Sequence[str]] = ...,
) -> CreateIAMPolicyAssignmentResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: AssignmentStatusType](./literals.md#assignmentstatustype) 
2. See [:material-code-braces: CreateIAMPolicyAssignmentResponseTypeDef](./type_defs.md#createiampolicyassignmentresponsetypedef) 


```python
# create_iam_policy_assignment method usage example with argument unpacking

kwargs: CreateIAMPolicyAssignmentRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "AssignmentName": ...,
    "AssignmentStatus": ...,
    "Namespace": ...,
}

parent.create_iam_policy_assignment(**kwargs)
```

1. See [:material-code-braces: CreateIAMPolicyAssignmentRequestTypeDef](./type_defs.md#createiampolicyassignmentrequesttypedef) 

### create\_ingestion

Creates and starts a new SPICE ingestion for a dataset.

Type annotations and code completion for `#!python session.create_client("quicksight").create_ingestion` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/create_ingestion.html)

```python
# create_ingestion method definition

await def create_ingestion(
    self,
    *,
    DataSetId: str,
    IngestionId: str,
    AwsAccountId: str,
    IngestionType: IngestionTypeType = ...,  # (1)
) -> CreateIngestionResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: IngestionTypeType](./literals.md#ingestiontypetype) 
2. See [:material-code-braces: CreateIngestionResponseTypeDef](./type_defs.md#createingestionresponsetypedef) 


```python
# create_ingestion method usage example with argument unpacking

kwargs: CreateIngestionRequestTypeDef = {  # (1)
    "DataSetId": ...,
    "IngestionId": ...,
    "AwsAccountId": ...,
}

parent.create_ingestion(**kwargs)
```

1. See [:material-code-braces: CreateIngestionRequestTypeDef](./type_defs.md#createingestionrequesttypedef) 

### create\_namespace

(Enterprise edition only) Creates a new namespace for you to use with Amazon
QuickSight.

Type annotations and code completion for `#!python session.create_client("quicksight").create_namespace` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/create_namespace.html)

```python
# create_namespace method definition

await def create_namespace(
    self,
    *,
    AwsAccountId: str,
    Namespace: str,
    IdentityStore: IdentityStoreType,  # (1)
    Tags: Sequence[TagTypeDef] = ...,  # (2)
) -> CreateNamespaceResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: IdentityStoreType](./literals.md#identitystoretype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: CreateNamespaceResponseTypeDef](./type_defs.md#createnamespaceresponsetypedef) 


```python
# create_namespace method usage example with argument unpacking

kwargs: CreateNamespaceRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "Namespace": ...,
    "IdentityStore": ...,
}

parent.create_namespace(**kwargs)
```

1. See [:material-code-braces: CreateNamespaceRequestTypeDef](./type_defs.md#createnamespacerequesttypedef) 

### create\_refresh\_schedule

Creates a refresh schedule for a dataset.

Type annotations and code completion for `#!python session.create_client("quicksight").create_refresh_schedule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/create_refresh_schedule.html)

```python
# create_refresh_schedule method definition

await def create_refresh_schedule(
    self,
    *,
    DataSetId: str,
    AwsAccountId: str,
    Schedule: RefreshScheduleUnionTypeDef,  # (1)
) -> CreateRefreshScheduleResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: RefreshScheduleTypeDef](./type_defs.md#refreshscheduletypedef) [:material-code-braces: RefreshScheduleOutputTypeDef](./type_defs.md#refreshscheduleoutputtypedef) 
2. See [:material-code-braces: CreateRefreshScheduleResponseTypeDef](./type_defs.md#createrefreshscheduleresponsetypedef) 


```python
# create_refresh_schedule method usage example with argument unpacking

kwargs: CreateRefreshScheduleRequestTypeDef = {  # (1)
    "DataSetId": ...,
    "AwsAccountId": ...,
    "Schedule": ...,
}

parent.create_refresh_schedule(**kwargs)
```

1. See [:material-code-braces: CreateRefreshScheduleRequestTypeDef](./type_defs.md#createrefreshschedulerequesttypedef) 

### create\_role\_membership

Use <code>CreateRoleMembership</code> to add an existing Amazon QuickSight
group to an existing role.

Type annotations and code completion for `#!python session.create_client("quicksight").create_role_membership` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/create_role_membership.html)

```python
# create_role_membership method definition

await def create_role_membership(
    self,
    *,
    MemberName: str,
    AwsAccountId: str,
    Namespace: str,
    Role: RoleType,  # (1)
) -> CreateRoleMembershipResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: RoleType](./literals.md#roletype) 
2. See [:material-code-braces: CreateRoleMembershipResponseTypeDef](./type_defs.md#createrolemembershipresponsetypedef) 


```python
# create_role_membership method usage example with argument unpacking

kwargs: CreateRoleMembershipRequestTypeDef = {  # (1)
    "MemberName": ...,
    "AwsAccountId": ...,
    "Namespace": ...,
    "Role": ...,
}

parent.create_role_membership(**kwargs)
```

1. See [:material-code-braces: CreateRoleMembershipRequestTypeDef](./type_defs.md#createrolemembershiprequesttypedef) 

### create\_template

Creates a template either from a <code>TemplateDefinition</code> or from an
existing Amazon QuickSight analysis or template.

Type annotations and code completion for `#!python session.create_client("quicksight").create_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/create_template.html)

```python
# create_template method definition

await def create_template(
    self,
    *,
    AwsAccountId: str,
    TemplateId: str,
    Name: str = ...,
    Permissions: Sequence[ResourcePermissionUnionTypeDef] = ...,  # (1)
    SourceEntity: TemplateSourceEntityTypeDef = ...,  # (2)
    Tags: Sequence[TagTypeDef] = ...,  # (3)
    VersionDescription: str = ...,
    Definition: TemplateVersionDefinitionUnionTypeDef = ...,  # (4)
    ValidationStrategy: ValidationStrategyTypeDef = ...,  # (5)
) -> CreateTemplateResponseTypeDef:  # (6)
    ...
```

1. See [:material-code-braces: ResourcePermissionTypeDef](./type_defs.md#resourcepermissiontypedef) [:material-code-braces: ResourcePermissionOutputTypeDef](./type_defs.md#resourcepermissionoutputtypedef) 
2. See [:material-code-braces: TemplateSourceEntityTypeDef](./type_defs.md#templatesourceentitytypedef) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
4. See [:material-code-braces: TemplateVersionDefinitionTypeDef](./type_defs.md#templateversiondefinitiontypedef) [:material-code-braces: TemplateVersionDefinitionOutputTypeDef](./type_defs.md#templateversiondefinitionoutputtypedef) 
5. See [:material-code-braces: ValidationStrategyTypeDef](./type_defs.md#validationstrategytypedef) 
6. See [:material-code-braces: CreateTemplateResponseTypeDef](./type_defs.md#createtemplateresponsetypedef) 


```python
# create_template method usage example with argument unpacking

kwargs: CreateTemplateRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "TemplateId": ...,
}

parent.create_template(**kwargs)
```

1. See [:material-code-braces: CreateTemplateRequestTypeDef](./type_defs.md#createtemplaterequesttypedef) 

### create\_template\_alias

Creates a template alias for a template.

Type annotations and code completion for `#!python session.create_client("quicksight").create_template_alias` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/create_template_alias.html)

```python
# create_template_alias method definition

await def create_template_alias(
    self,
    *,
    AwsAccountId: str,
    TemplateId: str,
    AliasName: str,
    TemplateVersionNumber: int,
) -> CreateTemplateAliasResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateTemplateAliasResponseTypeDef](./type_defs.md#createtemplatealiasresponsetypedef) 


```python
# create_template_alias method usage example with argument unpacking

kwargs: CreateTemplateAliasRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "TemplateId": ...,
    "AliasName": ...,
    "TemplateVersionNumber": ...,
}

parent.create_template_alias(**kwargs)
```

1. See [:material-code-braces: CreateTemplateAliasRequestTypeDef](./type_defs.md#createtemplatealiasrequesttypedef) 

### create\_theme

Creates a theme.

Type annotations and code completion for `#!python session.create_client("quicksight").create_theme` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/create_theme.html)

```python
# create_theme method definition

await def create_theme(
    self,
    *,
    AwsAccountId: str,
    ThemeId: str,
    Name: str,
    BaseThemeId: str,
    Configuration: ThemeConfigurationUnionTypeDef,  # (1)
    VersionDescription: str = ...,
    Permissions: Sequence[ResourcePermissionUnionTypeDef] = ...,  # (2)
    Tags: Sequence[TagTypeDef] = ...,  # (3)
) -> CreateThemeResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: ThemeConfigurationTypeDef](./type_defs.md#themeconfigurationtypedef) [:material-code-braces: ThemeConfigurationOutputTypeDef](./type_defs.md#themeconfigurationoutputtypedef) 
2. See [:material-code-braces: ResourcePermissionTypeDef](./type_defs.md#resourcepermissiontypedef) [:material-code-braces: ResourcePermissionOutputTypeDef](./type_defs.md#resourcepermissionoutputtypedef) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
4. See [:material-code-braces: CreateThemeResponseTypeDef](./type_defs.md#createthemeresponsetypedef) 


```python
# create_theme method usage example with argument unpacking

kwargs: CreateThemeRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "ThemeId": ...,
    "Name": ...,
    "BaseThemeId": ...,
    "Configuration": ...,
}

parent.create_theme(**kwargs)
```

1. See [:material-code-braces: CreateThemeRequestTypeDef](./type_defs.md#createthemerequesttypedef) 

### create\_theme\_alias

Creates a theme alias for a theme.

Type annotations and code completion for `#!python session.create_client("quicksight").create_theme_alias` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/create_theme_alias.html)

```python
# create_theme_alias method definition

await def create_theme_alias(
    self,
    *,
    AwsAccountId: str,
    ThemeId: str,
    AliasName: str,
    ThemeVersionNumber: int,
) -> CreateThemeAliasResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateThemeAliasResponseTypeDef](./type_defs.md#createthemealiasresponsetypedef) 


```python
# create_theme_alias method usage example with argument unpacking

kwargs: CreateThemeAliasRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "ThemeId": ...,
    "AliasName": ...,
    "ThemeVersionNumber": ...,
}

parent.create_theme_alias(**kwargs)
```

1. See [:material-code-braces: CreateThemeAliasRequestTypeDef](./type_defs.md#createthemealiasrequesttypedef) 

### create\_topic

Creates a new Q topic.

Type annotations and code completion for `#!python session.create_client("quicksight").create_topic` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/create_topic.html)

```python
# create_topic method definition

await def create_topic(
    self,
    *,
    AwsAccountId: str,
    TopicId: str,
    Topic: TopicDetailsUnionTypeDef,  # (1)
    Tags: Sequence[TagTypeDef] = ...,  # (2)
    FolderArns: Sequence[str] = ...,
) -> CreateTopicResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: TopicDetailsTypeDef](./type_defs.md#topicdetailstypedef) [:material-code-braces: TopicDetailsOutputTypeDef](./type_defs.md#topicdetailsoutputtypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: CreateTopicResponseTypeDef](./type_defs.md#createtopicresponsetypedef) 


```python
# create_topic method usage example with argument unpacking

kwargs: CreateTopicRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "TopicId": ...,
    "Topic": ...,
}

parent.create_topic(**kwargs)
```

1. See [:material-code-braces: CreateTopicRequestTypeDef](./type_defs.md#createtopicrequesttypedef) 

### create\_topic\_refresh\_schedule

Creates a topic refresh schedule.

Type annotations and code completion for `#!python session.create_client("quicksight").create_topic_refresh_schedule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/create_topic_refresh_schedule.html)

```python
# create_topic_refresh_schedule method definition

await def create_topic_refresh_schedule(
    self,
    *,
    AwsAccountId: str,
    TopicId: str,
    DatasetArn: str,
    RefreshSchedule: TopicRefreshScheduleUnionTypeDef,  # (1)
    DatasetName: str = ...,
) -> CreateTopicRefreshScheduleResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TopicRefreshScheduleTypeDef](./type_defs.md#topicrefreshscheduletypedef) [:material-code-braces: TopicRefreshScheduleOutputTypeDef](./type_defs.md#topicrefreshscheduleoutputtypedef) 
2. See [:material-code-braces: CreateTopicRefreshScheduleResponseTypeDef](./type_defs.md#createtopicrefreshscheduleresponsetypedef) 


```python
# create_topic_refresh_schedule method usage example with argument unpacking

kwargs: CreateTopicRefreshScheduleRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "TopicId": ...,
    "DatasetArn": ...,
    "RefreshSchedule": ...,
}

parent.create_topic_refresh_schedule(**kwargs)
```

1. See [:material-code-braces: CreateTopicRefreshScheduleRequestTypeDef](./type_defs.md#createtopicrefreshschedulerequesttypedef) 

### create\_vpc\_connection

Creates a new VPC connection.

Type annotations and code completion for `#!python session.create_client("quicksight").create_vpc_connection` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/create_vpc_connection.html)

```python
# create_vpc_connection method definition

await def create_vpc_connection(
    self,
    *,
    AwsAccountId: str,
    VPCConnectionId: str,
    Name: str,
    SubnetIds: Sequence[str],
    SecurityGroupIds: Sequence[str],
    RoleArn: str,
    DnsResolvers: Sequence[str] = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (1)
) -> CreateVPCConnectionResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: CreateVPCConnectionResponseTypeDef](./type_defs.md#createvpcconnectionresponsetypedef) 


```python
# create_vpc_connection method usage example with argument unpacking

kwargs: CreateVPCConnectionRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "VPCConnectionId": ...,
    "Name": ...,
    "SubnetIds": ...,
    "SecurityGroupIds": ...,
    "RoleArn": ...,
}

parent.create_vpc_connection(**kwargs)
```

1. See [:material-code-braces: CreateVPCConnectionRequestTypeDef](./type_defs.md#createvpcconnectionrequesttypedef) 

### delete\_account\_customization

Deletes all Amazon QuickSight customizations in this Amazon Web Services Region
for the specified Amazon Web Services account and Amazon QuickSight namespace.

Type annotations and code completion for `#!python session.create_client("quicksight").delete_account_customization` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/delete_account_customization.html)

```python
# delete_account_customization method definition

await def delete_account_customization(
    self,
    *,
    AwsAccountId: str,
    Namespace: str = ...,
) -> DeleteAccountCustomizationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteAccountCustomizationResponseTypeDef](./type_defs.md#deleteaccountcustomizationresponsetypedef) 


```python
# delete_account_customization method usage example with argument unpacking

kwargs: DeleteAccountCustomizationRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
}

parent.delete_account_customization(**kwargs)
```

1. See [:material-code-braces: DeleteAccountCustomizationRequestTypeDef](./type_defs.md#deleteaccountcustomizationrequesttypedef) 

### delete\_account\_subscription

Use the <code>DeleteAccountSubscription</code> operation to delete an Amazon
QuickSight account.

Type annotations and code completion for `#!python session.create_client("quicksight").delete_account_subscription` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/delete_account_subscription.html)

```python
# delete_account_subscription method definition

await def delete_account_subscription(
    self,
    *,
    AwsAccountId: str,
) -> DeleteAccountSubscriptionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteAccountSubscriptionResponseTypeDef](./type_defs.md#deleteaccountsubscriptionresponsetypedef) 


```python
# delete_account_subscription method usage example with argument unpacking

kwargs: DeleteAccountSubscriptionRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
}

parent.delete_account_subscription(**kwargs)
```

1. See [:material-code-braces: DeleteAccountSubscriptionRequestTypeDef](./type_defs.md#deleteaccountsubscriptionrequesttypedef) 

### delete\_analysis

Deletes an analysis from Amazon QuickSight.

Type annotations and code completion for `#!python session.create_client("quicksight").delete_analysis` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/delete_analysis.html)

```python
# delete_analysis method definition

await def delete_analysis(
    self,
    *,
    AwsAccountId: str,
    AnalysisId: str,
    RecoveryWindowInDays: int = ...,
    ForceDeleteWithoutRecovery: bool = ...,
) -> DeleteAnalysisResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteAnalysisResponseTypeDef](./type_defs.md#deleteanalysisresponsetypedef) 


```python
# delete_analysis method usage example with argument unpacking

kwargs: DeleteAnalysisRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "AnalysisId": ...,
}

parent.delete_analysis(**kwargs)
```

1. See [:material-code-braces: DeleteAnalysisRequestTypeDef](./type_defs.md#deleteanalysisrequesttypedef) 

### delete\_brand

Deletes an Amazon QuickSight brand.

Type annotations and code completion for `#!python session.create_client("quicksight").delete_brand` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/delete_brand.html)

```python
# delete_brand method definition

await def delete_brand(
    self,
    *,
    AwsAccountId: str,
    BrandId: str,
) -> DeleteBrandResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteBrandResponseTypeDef](./type_defs.md#deletebrandresponsetypedef) 


```python
# delete_brand method usage example with argument unpacking

kwargs: DeleteBrandRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "BrandId": ...,
}

parent.delete_brand(**kwargs)
```

1. See [:material-code-braces: DeleteBrandRequestTypeDef](./type_defs.md#deletebrandrequesttypedef) 

### delete\_brand\_assignment

Deletes a brand assignment.

Type annotations and code completion for `#!python session.create_client("quicksight").delete_brand_assignment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/delete_brand_assignment.html)

```python
# delete_brand_assignment method definition

await def delete_brand_assignment(
    self,
    *,
    AwsAccountId: str,
) -> DeleteBrandAssignmentResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteBrandAssignmentResponseTypeDef](./type_defs.md#deletebrandassignmentresponsetypedef) 


```python
# delete_brand_assignment method usage example with argument unpacking

kwargs: DeleteBrandAssignmentRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
}

parent.delete_brand_assignment(**kwargs)
```

1. See [:material-code-braces: DeleteBrandAssignmentRequestTypeDef](./type_defs.md#deletebrandassignmentrequesttypedef) 

### delete\_custom\_permissions

Deletes a custom permissions profile.

Type annotations and code completion for `#!python session.create_client("quicksight").delete_custom_permissions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/delete_custom_permissions.html)

```python
# delete_custom_permissions method definition

await def delete_custom_permissions(
    self,
    *,
    AwsAccountId: str,
    CustomPermissionsName: str,
) -> DeleteCustomPermissionsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteCustomPermissionsResponseTypeDef](./type_defs.md#deletecustompermissionsresponsetypedef) 


```python
# delete_custom_permissions method usage example with argument unpacking

kwargs: DeleteCustomPermissionsRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "CustomPermissionsName": ...,
}

parent.delete_custom_permissions(**kwargs)
```

1. See [:material-code-braces: DeleteCustomPermissionsRequestTypeDef](./type_defs.md#deletecustompermissionsrequesttypedef) 

### delete\_dashboard

Deletes a dashboard.

Type annotations and code completion for `#!python session.create_client("quicksight").delete_dashboard` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/delete_dashboard.html)

```python
# delete_dashboard method definition

await def delete_dashboard(
    self,
    *,
    AwsAccountId: str,
    DashboardId: str,
    VersionNumber: int = ...,
) -> DeleteDashboardResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteDashboardResponseTypeDef](./type_defs.md#deletedashboardresponsetypedef) 


```python
# delete_dashboard method usage example with argument unpacking

kwargs: DeleteDashboardRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "DashboardId": ...,
}

parent.delete_dashboard(**kwargs)
```

1. See [:material-code-braces: DeleteDashboardRequestTypeDef](./type_defs.md#deletedashboardrequesttypedef) 

### delete\_data\_set

Deletes a dataset.

Type annotations and code completion for `#!python session.create_client("quicksight").delete_data_set` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/delete_data_set.html)

```python
# delete_data_set method definition

await def delete_data_set(
    self,
    *,
    AwsAccountId: str,
    DataSetId: str,
) -> DeleteDataSetResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteDataSetResponseTypeDef](./type_defs.md#deletedatasetresponsetypedef) 


```python
# delete_data_set method usage example with argument unpacking

kwargs: DeleteDataSetRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "DataSetId": ...,
}

parent.delete_data_set(**kwargs)
```

1. See [:material-code-braces: DeleteDataSetRequestTypeDef](./type_defs.md#deletedatasetrequesttypedef) 

### delete\_data\_set\_refresh\_properties

Deletes the dataset refresh properties of the dataset.

Type annotations and code completion for `#!python session.create_client("quicksight").delete_data_set_refresh_properties` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/delete_data_set_refresh_properties.html)

```python
# delete_data_set_refresh_properties method definition

await def delete_data_set_refresh_properties(
    self,
    *,
    AwsAccountId: str,
    DataSetId: str,
) -> DeleteDataSetRefreshPropertiesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteDataSetRefreshPropertiesResponseTypeDef](./type_defs.md#deletedatasetrefreshpropertiesresponsetypedef) 


```python
# delete_data_set_refresh_properties method usage example with argument unpacking

kwargs: DeleteDataSetRefreshPropertiesRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "DataSetId": ...,
}

parent.delete_data_set_refresh_properties(**kwargs)
```

1. See [:material-code-braces: DeleteDataSetRefreshPropertiesRequestTypeDef](./type_defs.md#deletedatasetrefreshpropertiesrequesttypedef) 

### delete\_data\_source

Deletes the data source permanently.

Type annotations and code completion for `#!python session.create_client("quicksight").delete_data_source` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/delete_data_source.html)

```python
# delete_data_source method definition

await def delete_data_source(
    self,
    *,
    AwsAccountId: str,
    DataSourceId: str,
) -> DeleteDataSourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteDataSourceResponseTypeDef](./type_defs.md#deletedatasourceresponsetypedef) 


```python
# delete_data_source method usage example with argument unpacking

kwargs: DeleteDataSourceRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "DataSourceId": ...,
}

parent.delete_data_source(**kwargs)
```

1. See [:material-code-braces: DeleteDataSourceRequestTypeDef](./type_defs.md#deletedatasourcerequesttypedef) 

### delete\_default\_q\_business\_application

Deletes a linked Amazon Q Business application from an Amazon QuickSight
account.

Type annotations and code completion for `#!python session.create_client("quicksight").delete_default_q_business_application` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/delete_default_q_business_application.html)

```python
# delete_default_q_business_application method definition

await def delete_default_q_business_application(
    self,
    *,
    AwsAccountId: str,
    Namespace: str = ...,
) -> DeleteDefaultQBusinessApplicationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteDefaultQBusinessApplicationResponseTypeDef](./type_defs.md#deletedefaultqbusinessapplicationresponsetypedef) 


```python
# delete_default_q_business_application method usage example with argument unpacking

kwargs: DeleteDefaultQBusinessApplicationRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
}

parent.delete_default_q_business_application(**kwargs)
```

1. See [:material-code-braces: DeleteDefaultQBusinessApplicationRequestTypeDef](./type_defs.md#deletedefaultqbusinessapplicationrequesttypedef) 

### delete\_folder

Deletes an empty folder.

Type annotations and code completion for `#!python session.create_client("quicksight").delete_folder` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/delete_folder.html)

```python
# delete_folder method definition

await def delete_folder(
    self,
    *,
    AwsAccountId: str,
    FolderId: str,
) -> DeleteFolderResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteFolderResponseTypeDef](./type_defs.md#deletefolderresponsetypedef) 


```python
# delete_folder method usage example with argument unpacking

kwargs: DeleteFolderRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "FolderId": ...,
}

parent.delete_folder(**kwargs)
```

1. See [:material-code-braces: DeleteFolderRequestTypeDef](./type_defs.md#deletefolderrequesttypedef) 

### delete\_folder\_membership

Removes an asset, such as a dashboard, analysis, or dataset, from a folder.

Type annotations and code completion for `#!python session.create_client("quicksight").delete_folder_membership` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/delete_folder_membership.html)

```python
# delete_folder_membership method definition

await def delete_folder_membership(
    self,
    *,
    AwsAccountId: str,
    FolderId: str,
    MemberId: str,
    MemberType: MemberTypeType,  # (1)
) -> DeleteFolderMembershipResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: MemberTypeType](./literals.md#membertypetype) 
2. See [:material-code-braces: DeleteFolderMembershipResponseTypeDef](./type_defs.md#deletefoldermembershipresponsetypedef) 


```python
# delete_folder_membership method usage example with argument unpacking

kwargs: DeleteFolderMembershipRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "FolderId": ...,
    "MemberId": ...,
    "MemberType": ...,
}

parent.delete_folder_membership(**kwargs)
```

1. See [:material-code-braces: DeleteFolderMembershipRequestTypeDef](./type_defs.md#deletefoldermembershiprequesttypedef) 

### delete\_group

Removes a user group from Amazon QuickSight.

Type annotations and code completion for `#!python session.create_client("quicksight").delete_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/delete_group.html)

```python
# delete_group method definition

await def delete_group(
    self,
    *,
    GroupName: str,
    AwsAccountId: str,
    Namespace: str,
) -> DeleteGroupResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteGroupResponseTypeDef](./type_defs.md#deletegroupresponsetypedef) 


```python
# delete_group method usage example with argument unpacking

kwargs: DeleteGroupRequestTypeDef = {  # (1)
    "GroupName": ...,
    "AwsAccountId": ...,
    "Namespace": ...,
}

parent.delete_group(**kwargs)
```

1. See [:material-code-braces: DeleteGroupRequestTypeDef](./type_defs.md#deletegrouprequesttypedef) 

### delete\_group\_membership

Removes a user from a group so that the user is no longer a member of the group.

Type annotations and code completion for `#!python session.create_client("quicksight").delete_group_membership` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/delete_group_membership.html)

```python
# delete_group_membership method definition

await def delete_group_membership(
    self,
    *,
    MemberName: str,
    GroupName: str,
    AwsAccountId: str,
    Namespace: str,
) -> DeleteGroupMembershipResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteGroupMembershipResponseTypeDef](./type_defs.md#deletegroupmembershipresponsetypedef) 


```python
# delete_group_membership method usage example with argument unpacking

kwargs: DeleteGroupMembershipRequestTypeDef = {  # (1)
    "MemberName": ...,
    "GroupName": ...,
    "AwsAccountId": ...,
    "Namespace": ...,
}

parent.delete_group_membership(**kwargs)
```

1. See [:material-code-braces: DeleteGroupMembershipRequestTypeDef](./type_defs.md#deletegroupmembershiprequesttypedef) 

### delete\_iam\_policy\_assignment

Deletes an existing IAM policy assignment.

Type annotations and code completion for `#!python session.create_client("quicksight").delete_iam_policy_assignment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/delete_iam_policy_assignment.html)

```python
# delete_iam_policy_assignment method definition

await def delete_iam_policy_assignment(
    self,
    *,
    AwsAccountId: str,
    AssignmentName: str,
    Namespace: str,
) -> DeleteIAMPolicyAssignmentResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteIAMPolicyAssignmentResponseTypeDef](./type_defs.md#deleteiampolicyassignmentresponsetypedef) 


```python
# delete_iam_policy_assignment method usage example with argument unpacking

kwargs: DeleteIAMPolicyAssignmentRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "AssignmentName": ...,
    "Namespace": ...,
}

parent.delete_iam_policy_assignment(**kwargs)
```

1. See [:material-code-braces: DeleteIAMPolicyAssignmentRequestTypeDef](./type_defs.md#deleteiampolicyassignmentrequesttypedef) 

### delete\_identity\_propagation\_config

Deletes all access scopes and authorized targets that are associated with a
service from the Amazon QuickSight IAM Identity Center application.

Type annotations and code completion for `#!python session.create_client("quicksight").delete_identity_propagation_config` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/delete_identity_propagation_config.html)

```python
# delete_identity_propagation_config method definition

await def delete_identity_propagation_config(
    self,
    *,
    AwsAccountId: str,
    Service: ServiceTypeType,  # (1)
) -> DeleteIdentityPropagationConfigResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ServiceTypeType](./literals.md#servicetypetype) 
2. See [:material-code-braces: DeleteIdentityPropagationConfigResponseTypeDef](./type_defs.md#deleteidentitypropagationconfigresponsetypedef) 


```python
# delete_identity_propagation_config method usage example with argument unpacking

kwargs: DeleteIdentityPropagationConfigRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "Service": ...,
}

parent.delete_identity_propagation_config(**kwargs)
```

1. See [:material-code-braces: DeleteIdentityPropagationConfigRequestTypeDef](./type_defs.md#deleteidentitypropagationconfigrequesttypedef) 

### delete\_namespace

Deletes a namespace and the users and groups that are associated with the
namespace.

Type annotations and code completion for `#!python session.create_client("quicksight").delete_namespace` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/delete_namespace.html)

```python
# delete_namespace method definition

await def delete_namespace(
    self,
    *,
    AwsAccountId: str,
    Namespace: str,
) -> DeleteNamespaceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteNamespaceResponseTypeDef](./type_defs.md#deletenamespaceresponsetypedef) 


```python
# delete_namespace method usage example with argument unpacking

kwargs: DeleteNamespaceRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "Namespace": ...,
}

parent.delete_namespace(**kwargs)
```

1. See [:material-code-braces: DeleteNamespaceRequestTypeDef](./type_defs.md#deletenamespacerequesttypedef) 

### delete\_refresh\_schedule

Deletes a refresh schedule from a dataset.

Type annotations and code completion for `#!python session.create_client("quicksight").delete_refresh_schedule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/delete_refresh_schedule.html)

```python
# delete_refresh_schedule method definition

await def delete_refresh_schedule(
    self,
    *,
    DataSetId: str,
    AwsAccountId: str,
    ScheduleId: str,
) -> DeleteRefreshScheduleResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteRefreshScheduleResponseTypeDef](./type_defs.md#deleterefreshscheduleresponsetypedef) 


```python
# delete_refresh_schedule method usage example with argument unpacking

kwargs: DeleteRefreshScheduleRequestTypeDef = {  # (1)
    "DataSetId": ...,
    "AwsAccountId": ...,
    "ScheduleId": ...,
}

parent.delete_refresh_schedule(**kwargs)
```

1. See [:material-code-braces: DeleteRefreshScheduleRequestTypeDef](./type_defs.md#deleterefreshschedulerequesttypedef) 

### delete\_role\_custom\_permission

Removes custom permissions from the role.

Type annotations and code completion for `#!python session.create_client("quicksight").delete_role_custom_permission` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/delete_role_custom_permission.html)

```python
# delete_role_custom_permission method definition

await def delete_role_custom_permission(
    self,
    *,
    Role: RoleType,  # (1)
    AwsAccountId: str,
    Namespace: str,
) -> DeleteRoleCustomPermissionResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: RoleType](./literals.md#roletype) 
2. See [:material-code-braces: DeleteRoleCustomPermissionResponseTypeDef](./type_defs.md#deleterolecustompermissionresponsetypedef) 


```python
# delete_role_custom_permission method usage example with argument unpacking

kwargs: DeleteRoleCustomPermissionRequestTypeDef = {  # (1)
    "Role": ...,
    "AwsAccountId": ...,
    "Namespace": ...,
}

parent.delete_role_custom_permission(**kwargs)
```

1. See [:material-code-braces: DeleteRoleCustomPermissionRequestTypeDef](./type_defs.md#deleterolecustompermissionrequesttypedef) 

### delete\_role\_membership

Removes a group from a role.

Type annotations and code completion for `#!python session.create_client("quicksight").delete_role_membership` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/delete_role_membership.html)

```python
# delete_role_membership method definition

await def delete_role_membership(
    self,
    *,
    MemberName: str,
    Role: RoleType,  # (1)
    AwsAccountId: str,
    Namespace: str,
) -> DeleteRoleMembershipResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: RoleType](./literals.md#roletype) 
2. See [:material-code-braces: DeleteRoleMembershipResponseTypeDef](./type_defs.md#deleterolemembershipresponsetypedef) 


```python
# delete_role_membership method usage example with argument unpacking

kwargs: DeleteRoleMembershipRequestTypeDef = {  # (1)
    "MemberName": ...,
    "Role": ...,
    "AwsAccountId": ...,
    "Namespace": ...,
}

parent.delete_role_membership(**kwargs)
```

1. See [:material-code-braces: DeleteRoleMembershipRequestTypeDef](./type_defs.md#deleterolemembershiprequesttypedef) 

### delete\_template

Deletes a template.

Type annotations and code completion for `#!python session.create_client("quicksight").delete_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/delete_template.html)

```python
# delete_template method definition

await def delete_template(
    self,
    *,
    AwsAccountId: str,
    TemplateId: str,
    VersionNumber: int = ...,
) -> DeleteTemplateResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteTemplateResponseTypeDef](./type_defs.md#deletetemplateresponsetypedef) 


```python
# delete_template method usage example with argument unpacking

kwargs: DeleteTemplateRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "TemplateId": ...,
}

parent.delete_template(**kwargs)
```

1. See [:material-code-braces: DeleteTemplateRequestTypeDef](./type_defs.md#deletetemplaterequesttypedef) 

### delete\_template\_alias

Deletes the item that the specified template alias points to.

Type annotations and code completion for `#!python session.create_client("quicksight").delete_template_alias` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/delete_template_alias.html)

```python
# delete_template_alias method definition

await def delete_template_alias(
    self,
    *,
    AwsAccountId: str,
    TemplateId: str,
    AliasName: str,
) -> DeleteTemplateAliasResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteTemplateAliasResponseTypeDef](./type_defs.md#deletetemplatealiasresponsetypedef) 


```python
# delete_template_alias method usage example with argument unpacking

kwargs: DeleteTemplateAliasRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "TemplateId": ...,
    "AliasName": ...,
}

parent.delete_template_alias(**kwargs)
```

1. See [:material-code-braces: DeleteTemplateAliasRequestTypeDef](./type_defs.md#deletetemplatealiasrequesttypedef) 

### delete\_theme

Deletes a theme.

Type annotations and code completion for `#!python session.create_client("quicksight").delete_theme` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/delete_theme.html)

```python
# delete_theme method definition

await def delete_theme(
    self,
    *,
    AwsAccountId: str,
    ThemeId: str,
    VersionNumber: int = ...,
) -> DeleteThemeResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteThemeResponseTypeDef](./type_defs.md#deletethemeresponsetypedef) 


```python
# delete_theme method usage example with argument unpacking

kwargs: DeleteThemeRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "ThemeId": ...,
}

parent.delete_theme(**kwargs)
```

1. See [:material-code-braces: DeleteThemeRequestTypeDef](./type_defs.md#deletethemerequesttypedef) 

### delete\_theme\_alias

Deletes the version of the theme that the specified theme alias points to.

Type annotations and code completion for `#!python session.create_client("quicksight").delete_theme_alias` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/delete_theme_alias.html)

```python
# delete_theme_alias method definition

await def delete_theme_alias(
    self,
    *,
    AwsAccountId: str,
    ThemeId: str,
    AliasName: str,
) -> DeleteThemeAliasResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteThemeAliasResponseTypeDef](./type_defs.md#deletethemealiasresponsetypedef) 


```python
# delete_theme_alias method usage example with argument unpacking

kwargs: DeleteThemeAliasRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "ThemeId": ...,
    "AliasName": ...,
}

parent.delete_theme_alias(**kwargs)
```

1. See [:material-code-braces: DeleteThemeAliasRequestTypeDef](./type_defs.md#deletethemealiasrequesttypedef) 

### delete\_topic

Deletes a topic.

Type annotations and code completion for `#!python session.create_client("quicksight").delete_topic` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/delete_topic.html)

```python
# delete_topic method definition

await def delete_topic(
    self,
    *,
    AwsAccountId: str,
    TopicId: str,
) -> DeleteTopicResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteTopicResponseTypeDef](./type_defs.md#deletetopicresponsetypedef) 


```python
# delete_topic method usage example with argument unpacking

kwargs: DeleteTopicRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "TopicId": ...,
}

parent.delete_topic(**kwargs)
```

1. See [:material-code-braces: DeleteTopicRequestTypeDef](./type_defs.md#deletetopicrequesttypedef) 

### delete\_topic\_refresh\_schedule

Deletes a topic refresh schedule.

Type annotations and code completion for `#!python session.create_client("quicksight").delete_topic_refresh_schedule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/delete_topic_refresh_schedule.html)

```python
# delete_topic_refresh_schedule method definition

await def delete_topic_refresh_schedule(
    self,
    *,
    AwsAccountId: str,
    TopicId: str,
    DatasetId: str,
) -> DeleteTopicRefreshScheduleResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteTopicRefreshScheduleResponseTypeDef](./type_defs.md#deletetopicrefreshscheduleresponsetypedef) 


```python
# delete_topic_refresh_schedule method usage example with argument unpacking

kwargs: DeleteTopicRefreshScheduleRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "TopicId": ...,
    "DatasetId": ...,
}

parent.delete_topic_refresh_schedule(**kwargs)
```

1. See [:material-code-braces: DeleteTopicRefreshScheduleRequestTypeDef](./type_defs.md#deletetopicrefreshschedulerequesttypedef) 

### delete\_user

Deletes the Amazon QuickSight user that is associated with the identity of the
IAM user or role that's making the call.

Type annotations and code completion for `#!python session.create_client("quicksight").delete_user` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/delete_user.html)

```python
# delete_user method definition

await def delete_user(
    self,
    *,
    UserName: str,
    AwsAccountId: str,
    Namespace: str,
) -> DeleteUserResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteUserResponseTypeDef](./type_defs.md#deleteuserresponsetypedef) 


```python
# delete_user method usage example with argument unpacking

kwargs: DeleteUserRequestTypeDef = {  # (1)
    "UserName": ...,
    "AwsAccountId": ...,
    "Namespace": ...,
}

parent.delete_user(**kwargs)
```

1. See [:material-code-braces: DeleteUserRequestTypeDef](./type_defs.md#deleteuserrequesttypedef) 

### delete\_user\_by\_principal\_id

Deletes a user identified by its principal ID.

Type annotations and code completion for `#!python session.create_client("quicksight").delete_user_by_principal_id` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/delete_user_by_principal_id.html)

```python
# delete_user_by_principal_id method definition

await def delete_user_by_principal_id(
    self,
    *,
    PrincipalId: str,
    AwsAccountId: str,
    Namespace: str,
) -> DeleteUserByPrincipalIdResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteUserByPrincipalIdResponseTypeDef](./type_defs.md#deleteuserbyprincipalidresponsetypedef) 


```python
# delete_user_by_principal_id method usage example with argument unpacking

kwargs: DeleteUserByPrincipalIdRequestTypeDef = {  # (1)
    "PrincipalId": ...,
    "AwsAccountId": ...,
    "Namespace": ...,
}

parent.delete_user_by_principal_id(**kwargs)
```

1. See [:material-code-braces: DeleteUserByPrincipalIdRequestTypeDef](./type_defs.md#deleteuserbyprincipalidrequesttypedef) 

### delete\_user\_custom\_permission

Deletes a custom permissions profile from a user.

Type annotations and code completion for `#!python session.create_client("quicksight").delete_user_custom_permission` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/delete_user_custom_permission.html)

```python
# delete_user_custom_permission method definition

await def delete_user_custom_permission(
    self,
    *,
    UserName: str,
    AwsAccountId: str,
    Namespace: str,
) -> DeleteUserCustomPermissionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteUserCustomPermissionResponseTypeDef](./type_defs.md#deleteusercustompermissionresponsetypedef) 


```python
# delete_user_custom_permission method usage example with argument unpacking

kwargs: DeleteUserCustomPermissionRequestTypeDef = {  # (1)
    "UserName": ...,
    "AwsAccountId": ...,
    "Namespace": ...,
}

parent.delete_user_custom_permission(**kwargs)
```

1. See [:material-code-braces: DeleteUserCustomPermissionRequestTypeDef](./type_defs.md#deleteusercustompermissionrequesttypedef) 

### delete\_vpc\_connection

Deletes a VPC connection.

Type annotations and code completion for `#!python session.create_client("quicksight").delete_vpc_connection` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/delete_vpc_connection.html)

```python
# delete_vpc_connection method definition

await def delete_vpc_connection(
    self,
    *,
    AwsAccountId: str,
    VPCConnectionId: str,
) -> DeleteVPCConnectionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteVPCConnectionResponseTypeDef](./type_defs.md#deletevpcconnectionresponsetypedef) 


```python
# delete_vpc_connection method usage example with argument unpacking

kwargs: DeleteVPCConnectionRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "VPCConnectionId": ...,
}

parent.delete_vpc_connection(**kwargs)
```

1. See [:material-code-braces: DeleteVPCConnectionRequestTypeDef](./type_defs.md#deletevpcconnectionrequesttypedef) 

### describe\_account\_customization

Describes the customizations associated with the provided Amazon Web Services
account and Amazon Amazon QuickSight namespace in an Amazon Web Services
Region.

Type annotations and code completion for `#!python session.create_client("quicksight").describe_account_customization` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/describe_account_customization.html)

```python
# describe_account_customization method definition

await def describe_account_customization(
    self,
    *,
    AwsAccountId: str,
    Namespace: str = ...,
    Resolved: bool = ...,
) -> DescribeAccountCustomizationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeAccountCustomizationResponseTypeDef](./type_defs.md#describeaccountcustomizationresponsetypedef) 


```python
# describe_account_customization method usage example with argument unpacking

kwargs: DescribeAccountCustomizationRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
}

parent.describe_account_customization(**kwargs)
```

1. See [:material-code-braces: DescribeAccountCustomizationRequestTypeDef](./type_defs.md#describeaccountcustomizationrequesttypedef) 

### describe\_account\_settings

Describes the settings that were used when your Amazon QuickSight subscription
was first created in this Amazon Web Services account.

Type annotations and code completion for `#!python session.create_client("quicksight").describe_account_settings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/describe_account_settings.html)

```python
# describe_account_settings method definition

await def describe_account_settings(
    self,
    *,
    AwsAccountId: str,
) -> DescribeAccountSettingsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeAccountSettingsResponseTypeDef](./type_defs.md#describeaccountsettingsresponsetypedef) 


```python
# describe_account_settings method usage example with argument unpacking

kwargs: DescribeAccountSettingsRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
}

parent.describe_account_settings(**kwargs)
```

1. See [:material-code-braces: DescribeAccountSettingsRequestTypeDef](./type_defs.md#describeaccountsettingsrequesttypedef) 

### describe\_account\_subscription

Use the DescribeAccountSubscription operation to receive a description of an
Amazon QuickSight account's subscription.

Type annotations and code completion for `#!python session.create_client("quicksight").describe_account_subscription` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/describe_account_subscription.html)

```python
# describe_account_subscription method definition

await def describe_account_subscription(
    self,
    *,
    AwsAccountId: str,
) -> DescribeAccountSubscriptionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeAccountSubscriptionResponseTypeDef](./type_defs.md#describeaccountsubscriptionresponsetypedef) 


```python
# describe_account_subscription method usage example with argument unpacking

kwargs: DescribeAccountSubscriptionRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
}

parent.describe_account_subscription(**kwargs)
```

1. See [:material-code-braces: DescribeAccountSubscriptionRequestTypeDef](./type_defs.md#describeaccountsubscriptionrequesttypedef) 

### describe\_analysis

Provides a summary of the metadata for an analysis.

Type annotations and code completion for `#!python session.create_client("quicksight").describe_analysis` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/describe_analysis.html)

```python
# describe_analysis method definition

await def describe_analysis(
    self,
    *,
    AwsAccountId: str,
    AnalysisId: str,
) -> DescribeAnalysisResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeAnalysisResponseTypeDef](./type_defs.md#describeanalysisresponsetypedef) 


```python
# describe_analysis method usage example with argument unpacking

kwargs: DescribeAnalysisRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "AnalysisId": ...,
}

parent.describe_analysis(**kwargs)
```

1. See [:material-code-braces: DescribeAnalysisRequestTypeDef](./type_defs.md#describeanalysisrequesttypedef) 

### describe\_analysis\_definition

Provides a detailed description of the definition of an analysis.

Type annotations and code completion for `#!python session.create_client("quicksight").describe_analysis_definition` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/describe_analysis_definition.html)

```python
# describe_analysis_definition method definition

await def describe_analysis_definition(
    self,
    *,
    AwsAccountId: str,
    AnalysisId: str,
) -> DescribeAnalysisDefinitionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeAnalysisDefinitionResponseTypeDef](./type_defs.md#describeanalysisdefinitionresponsetypedef) 


```python
# describe_analysis_definition method usage example with argument unpacking

kwargs: DescribeAnalysisDefinitionRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "AnalysisId": ...,
}

parent.describe_analysis_definition(**kwargs)
```

1. See [:material-code-braces: DescribeAnalysisDefinitionRequestTypeDef](./type_defs.md#describeanalysisdefinitionrequesttypedef) 

### describe\_analysis\_permissions

Provides the read and write permissions for an analysis.

Type annotations and code completion for `#!python session.create_client("quicksight").describe_analysis_permissions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/describe_analysis_permissions.html)

```python
# describe_analysis_permissions method definition

await def describe_analysis_permissions(
    self,
    *,
    AwsAccountId: str,
    AnalysisId: str,
) -> DescribeAnalysisPermissionsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeAnalysisPermissionsResponseTypeDef](./type_defs.md#describeanalysispermissionsresponsetypedef) 


```python
# describe_analysis_permissions method usage example with argument unpacking

kwargs: DescribeAnalysisPermissionsRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "AnalysisId": ...,
}

parent.describe_analysis_permissions(**kwargs)
```

1. See [:material-code-braces: DescribeAnalysisPermissionsRequestTypeDef](./type_defs.md#describeanalysispermissionsrequesttypedef) 

### describe\_asset\_bundle\_export\_job

Describes an existing export job.

Type annotations and code completion for `#!python session.create_client("quicksight").describe_asset_bundle_export_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/describe_asset_bundle_export_job.html)

```python
# describe_asset_bundle_export_job method definition

await def describe_asset_bundle_export_job(
    self,
    *,
    AwsAccountId: str,
    AssetBundleExportJobId: str,
) -> DescribeAssetBundleExportJobResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeAssetBundleExportJobResponseTypeDef](./type_defs.md#describeassetbundleexportjobresponsetypedef) 


```python
# describe_asset_bundle_export_job method usage example with argument unpacking

kwargs: DescribeAssetBundleExportJobRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "AssetBundleExportJobId": ...,
}

parent.describe_asset_bundle_export_job(**kwargs)
```

1. See [:material-code-braces: DescribeAssetBundleExportJobRequestTypeDef](./type_defs.md#describeassetbundleexportjobrequesttypedef) 

### describe\_asset\_bundle\_import\_job

Describes an existing import job.

Type annotations and code completion for `#!python session.create_client("quicksight").describe_asset_bundle_import_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/describe_asset_bundle_import_job.html)

```python
# describe_asset_bundle_import_job method definition

await def describe_asset_bundle_import_job(
    self,
    *,
    AwsAccountId: str,
    AssetBundleImportJobId: str,
) -> DescribeAssetBundleImportJobResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeAssetBundleImportJobResponseTypeDef](./type_defs.md#describeassetbundleimportjobresponsetypedef) 


```python
# describe_asset_bundle_import_job method usage example with argument unpacking

kwargs: DescribeAssetBundleImportJobRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "AssetBundleImportJobId": ...,
}

parent.describe_asset_bundle_import_job(**kwargs)
```

1. See [:material-code-braces: DescribeAssetBundleImportJobRequestTypeDef](./type_defs.md#describeassetbundleimportjobrequesttypedef) 

### describe\_brand

Describes a brand.

Type annotations and code completion for `#!python session.create_client("quicksight").describe_brand` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/describe_brand.html)

```python
# describe_brand method definition

await def describe_brand(
    self,
    *,
    AwsAccountId: str,
    BrandId: str,
    VersionId: str = ...,
) -> DescribeBrandResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeBrandResponseTypeDef](./type_defs.md#describebrandresponsetypedef) 


```python
# describe_brand method usage example with argument unpacking

kwargs: DescribeBrandRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "BrandId": ...,
}

parent.describe_brand(**kwargs)
```

1. See [:material-code-braces: DescribeBrandRequestTypeDef](./type_defs.md#describebrandrequesttypedef) 

### describe\_brand\_assignment

Describes a brand assignment.

Type annotations and code completion for `#!python session.create_client("quicksight").describe_brand_assignment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/describe_brand_assignment.html)

```python
# describe_brand_assignment method definition

await def describe_brand_assignment(
    self,
    *,
    AwsAccountId: str,
) -> DescribeBrandAssignmentResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeBrandAssignmentResponseTypeDef](./type_defs.md#describebrandassignmentresponsetypedef) 


```python
# describe_brand_assignment method usage example with argument unpacking

kwargs: DescribeBrandAssignmentRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
}

parent.describe_brand_assignment(**kwargs)
```

1. See [:material-code-braces: DescribeBrandAssignmentRequestTypeDef](./type_defs.md#describebrandassignmentrequesttypedef) 

### describe\_brand\_published\_version

Describes the published version of the brand.

Type annotations and code completion for `#!python session.create_client("quicksight").describe_brand_published_version` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/describe_brand_published_version.html)

```python
# describe_brand_published_version method definition

await def describe_brand_published_version(
    self,
    *,
    AwsAccountId: str,
    BrandId: str,
) -> DescribeBrandPublishedVersionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeBrandPublishedVersionResponseTypeDef](./type_defs.md#describebrandpublishedversionresponsetypedef) 


```python
# describe_brand_published_version method usage example with argument unpacking

kwargs: DescribeBrandPublishedVersionRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "BrandId": ...,
}

parent.describe_brand_published_version(**kwargs)
```

1. See [:material-code-braces: DescribeBrandPublishedVersionRequestTypeDef](./type_defs.md#describebrandpublishedversionrequesttypedef) 

### describe\_custom\_permissions

Describes a custom permissions profile.

Type annotations and code completion for `#!python session.create_client("quicksight").describe_custom_permissions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/describe_custom_permissions.html)

```python
# describe_custom_permissions method definition

await def describe_custom_permissions(
    self,
    *,
    AwsAccountId: str,
    CustomPermissionsName: str,
) -> DescribeCustomPermissionsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeCustomPermissionsResponseTypeDef](./type_defs.md#describecustompermissionsresponsetypedef) 


```python
# describe_custom_permissions method usage example with argument unpacking

kwargs: DescribeCustomPermissionsRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "CustomPermissionsName": ...,
}

parent.describe_custom_permissions(**kwargs)
```

1. See [:material-code-braces: DescribeCustomPermissionsRequestTypeDef](./type_defs.md#describecustompermissionsrequesttypedef) 

### describe\_dashboard

Provides a summary for a dashboard.

Type annotations and code completion for `#!python session.create_client("quicksight").describe_dashboard` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/describe_dashboard.html)

```python
# describe_dashboard method definition

await def describe_dashboard(
    self,
    *,
    AwsAccountId: str,
    DashboardId: str,
    VersionNumber: int = ...,
    AliasName: str = ...,
) -> DescribeDashboardResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeDashboardResponseTypeDef](./type_defs.md#describedashboardresponsetypedef) 


```python
# describe_dashboard method usage example with argument unpacking

kwargs: DescribeDashboardRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "DashboardId": ...,
}

parent.describe_dashboard(**kwargs)
```

1. See [:material-code-braces: DescribeDashboardRequestTypeDef](./type_defs.md#describedashboardrequesttypedef) 

### describe\_dashboard\_definition

Provides a detailed description of the definition of a dashboard.

Type annotations and code completion for `#!python session.create_client("quicksight").describe_dashboard_definition` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/describe_dashboard_definition.html)

```python
# describe_dashboard_definition method definition

await def describe_dashboard_definition(
    self,
    *,
    AwsAccountId: str,
    DashboardId: str,
    VersionNumber: int = ...,
    AliasName: str = ...,
) -> DescribeDashboardDefinitionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeDashboardDefinitionResponseTypeDef](./type_defs.md#describedashboarddefinitionresponsetypedef) 


```python
# describe_dashboard_definition method usage example with argument unpacking

kwargs: DescribeDashboardDefinitionRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "DashboardId": ...,
}

parent.describe_dashboard_definition(**kwargs)
```

1. See [:material-code-braces: DescribeDashboardDefinitionRequestTypeDef](./type_defs.md#describedashboarddefinitionrequesttypedef) 

### describe\_dashboard\_permissions

Describes read and write permissions for a dashboard.

Type annotations and code completion for `#!python session.create_client("quicksight").describe_dashboard_permissions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/describe_dashboard_permissions.html)

```python
# describe_dashboard_permissions method definition

await def describe_dashboard_permissions(
    self,
    *,
    AwsAccountId: str,
    DashboardId: str,
) -> DescribeDashboardPermissionsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeDashboardPermissionsResponseTypeDef](./type_defs.md#describedashboardpermissionsresponsetypedef) 


```python
# describe_dashboard_permissions method usage example with argument unpacking

kwargs: DescribeDashboardPermissionsRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "DashboardId": ...,
}

parent.describe_dashboard_permissions(**kwargs)
```

1. See [:material-code-braces: DescribeDashboardPermissionsRequestTypeDef](./type_defs.md#describedashboardpermissionsrequesttypedef) 

### describe\_dashboard\_snapshot\_job

Describes an existing snapshot job.

Type annotations and code completion for `#!python session.create_client("quicksight").describe_dashboard_snapshot_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/describe_dashboard_snapshot_job.html)

```python
# describe_dashboard_snapshot_job method definition

await def describe_dashboard_snapshot_job(
    self,
    *,
    AwsAccountId: str,
    DashboardId: str,
    SnapshotJobId: str,
) -> DescribeDashboardSnapshotJobResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeDashboardSnapshotJobResponseTypeDef](./type_defs.md#describedashboardsnapshotjobresponsetypedef) 


```python
# describe_dashboard_snapshot_job method usage example with argument unpacking

kwargs: DescribeDashboardSnapshotJobRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "DashboardId": ...,
    "SnapshotJobId": ...,
}

parent.describe_dashboard_snapshot_job(**kwargs)
```

1. See [:material-code-braces: DescribeDashboardSnapshotJobRequestTypeDef](./type_defs.md#describedashboardsnapshotjobrequesttypedef) 

### describe\_dashboard\_snapshot\_job\_result

Describes the result of an existing snapshot job that has finished running.

Type annotations and code completion for `#!python session.create_client("quicksight").describe_dashboard_snapshot_job_result` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/describe_dashboard_snapshot_job_result.html)

```python
# describe_dashboard_snapshot_job_result method definition

await def describe_dashboard_snapshot_job_result(
    self,
    *,
    AwsAccountId: str,
    DashboardId: str,
    SnapshotJobId: str,
) -> DescribeDashboardSnapshotJobResultResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeDashboardSnapshotJobResultResponseTypeDef](./type_defs.md#describedashboardsnapshotjobresultresponsetypedef) 


```python
# describe_dashboard_snapshot_job_result method usage example with argument unpacking

kwargs: DescribeDashboardSnapshotJobResultRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "DashboardId": ...,
    "SnapshotJobId": ...,
}

parent.describe_dashboard_snapshot_job_result(**kwargs)
```

1. See [:material-code-braces: DescribeDashboardSnapshotJobResultRequestTypeDef](./type_defs.md#describedashboardsnapshotjobresultrequesttypedef) 

### describe\_dashboards\_qa\_configuration

Describes an existing dashboard QA configuration.

Type annotations and code completion for `#!python session.create_client("quicksight").describe_dashboards_qa_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/describe_dashboards_qa_configuration.html)

```python
# describe_dashboards_qa_configuration method definition

await def describe_dashboards_qa_configuration(
    self,
    *,
    AwsAccountId: str,
) -> DescribeDashboardsQAConfigurationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeDashboardsQAConfigurationResponseTypeDef](./type_defs.md#describedashboardsqaconfigurationresponsetypedef) 


```python
# describe_dashboards_qa_configuration method usage example with argument unpacking

kwargs: DescribeDashboardsQAConfigurationRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
}

parent.describe_dashboards_qa_configuration(**kwargs)
```

1. See [:material-code-braces: DescribeDashboardsQAConfigurationRequestTypeDef](./type_defs.md#describedashboardsqaconfigurationrequesttypedef) 

### describe\_data\_set

Describes a dataset.

Type annotations and code completion for `#!python session.create_client("quicksight").describe_data_set` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/describe_data_set.html)

```python
# describe_data_set method definition

await def describe_data_set(
    self,
    *,
    AwsAccountId: str,
    DataSetId: str,
) -> DescribeDataSetResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeDataSetResponseTypeDef](./type_defs.md#describedatasetresponsetypedef) 


```python
# describe_data_set method usage example with argument unpacking

kwargs: DescribeDataSetRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "DataSetId": ...,
}

parent.describe_data_set(**kwargs)
```

1. See [:material-code-braces: DescribeDataSetRequestTypeDef](./type_defs.md#describedatasetrequesttypedef) 

### describe\_data\_set\_permissions

Describes the permissions on a dataset.

Type annotations and code completion for `#!python session.create_client("quicksight").describe_data_set_permissions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/describe_data_set_permissions.html)

```python
# describe_data_set_permissions method definition

await def describe_data_set_permissions(
    self,
    *,
    AwsAccountId: str,
    DataSetId: str,
) -> DescribeDataSetPermissionsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeDataSetPermissionsResponseTypeDef](./type_defs.md#describedatasetpermissionsresponsetypedef) 


```python
# describe_data_set_permissions method usage example with argument unpacking

kwargs: DescribeDataSetPermissionsRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "DataSetId": ...,
}

parent.describe_data_set_permissions(**kwargs)
```

1. See [:material-code-braces: DescribeDataSetPermissionsRequestTypeDef](./type_defs.md#describedatasetpermissionsrequesttypedef) 

### describe\_data\_set\_refresh\_properties

Describes the refresh properties of a dataset.

Type annotations and code completion for `#!python session.create_client("quicksight").describe_data_set_refresh_properties` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/describe_data_set_refresh_properties.html)

```python
# describe_data_set_refresh_properties method definition

await def describe_data_set_refresh_properties(
    self,
    *,
    AwsAccountId: str,
    DataSetId: str,
) -> DescribeDataSetRefreshPropertiesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeDataSetRefreshPropertiesResponseTypeDef](./type_defs.md#describedatasetrefreshpropertiesresponsetypedef) 


```python
# describe_data_set_refresh_properties method usage example with argument unpacking

kwargs: DescribeDataSetRefreshPropertiesRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "DataSetId": ...,
}

parent.describe_data_set_refresh_properties(**kwargs)
```

1. See [:material-code-braces: DescribeDataSetRefreshPropertiesRequestTypeDef](./type_defs.md#describedatasetrefreshpropertiesrequesttypedef) 

### describe\_data\_source

Describes a data source.

Type annotations and code completion for `#!python session.create_client("quicksight").describe_data_source` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/describe_data_source.html)

```python
# describe_data_source method definition

await def describe_data_source(
    self,
    *,
    AwsAccountId: str,
    DataSourceId: str,
) -> DescribeDataSourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeDataSourceResponseTypeDef](./type_defs.md#describedatasourceresponsetypedef) 


```python
# describe_data_source method usage example with argument unpacking

kwargs: DescribeDataSourceRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "DataSourceId": ...,
}

parent.describe_data_source(**kwargs)
```

1. See [:material-code-braces: DescribeDataSourceRequestTypeDef](./type_defs.md#describedatasourcerequesttypedef) 

### describe\_data\_source\_permissions

Describes the resource permissions for a data source.

Type annotations and code completion for `#!python session.create_client("quicksight").describe_data_source_permissions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/describe_data_source_permissions.html)

```python
# describe_data_source_permissions method definition

await def describe_data_source_permissions(
    self,
    *,
    AwsAccountId: str,
    DataSourceId: str,
) -> DescribeDataSourcePermissionsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeDataSourcePermissionsResponseTypeDef](./type_defs.md#describedatasourcepermissionsresponsetypedef) 


```python
# describe_data_source_permissions method usage example with argument unpacking

kwargs: DescribeDataSourcePermissionsRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "DataSourceId": ...,
}

parent.describe_data_source_permissions(**kwargs)
```

1. See [:material-code-braces: DescribeDataSourcePermissionsRequestTypeDef](./type_defs.md#describedatasourcepermissionsrequesttypedef) 

### describe\_default\_q\_business\_application

Describes a Amazon Q Business application that is linked to an Amazon
QuickSight account.

Type annotations and code completion for `#!python session.create_client("quicksight").describe_default_q_business_application` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/describe_default_q_business_application.html)

```python
# describe_default_q_business_application method definition

await def describe_default_q_business_application(
    self,
    *,
    AwsAccountId: str,
    Namespace: str = ...,
) -> DescribeDefaultQBusinessApplicationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeDefaultQBusinessApplicationResponseTypeDef](./type_defs.md#describedefaultqbusinessapplicationresponsetypedef) 


```python
# describe_default_q_business_application method usage example with argument unpacking

kwargs: DescribeDefaultQBusinessApplicationRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
}

parent.describe_default_q_business_application(**kwargs)
```

1. See [:material-code-braces: DescribeDefaultQBusinessApplicationRequestTypeDef](./type_defs.md#describedefaultqbusinessapplicationrequesttypedef) 

### describe\_folder

Describes a folder.

Type annotations and code completion for `#!python session.create_client("quicksight").describe_folder` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/describe_folder.html)

```python
# describe_folder method definition

await def describe_folder(
    self,
    *,
    AwsAccountId: str,
    FolderId: str,
) -> DescribeFolderResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeFolderResponseTypeDef](./type_defs.md#describefolderresponsetypedef) 


```python
# describe_folder method usage example with argument unpacking

kwargs: DescribeFolderRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "FolderId": ...,
}

parent.describe_folder(**kwargs)
```

1. See [:material-code-braces: DescribeFolderRequestTypeDef](./type_defs.md#describefolderrequesttypedef) 

### describe\_folder\_permissions

Describes permissions for a folder.

Type annotations and code completion for `#!python session.create_client("quicksight").describe_folder_permissions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/describe_folder_permissions.html)

```python
# describe_folder_permissions method definition

await def describe_folder_permissions(
    self,
    *,
    AwsAccountId: str,
    FolderId: str,
    Namespace: str = ...,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> DescribeFolderPermissionsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeFolderPermissionsResponseTypeDef](./type_defs.md#describefolderpermissionsresponsetypedef) 


```python
# describe_folder_permissions method usage example with argument unpacking

kwargs: DescribeFolderPermissionsRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "FolderId": ...,
}

parent.describe_folder_permissions(**kwargs)
```

1. See [:material-code-braces: DescribeFolderPermissionsRequestTypeDef](./type_defs.md#describefolderpermissionsrequesttypedef) 

### describe\_folder\_resolved\_permissions

Describes the folder resolved permissions.

Type annotations and code completion for `#!python session.create_client("quicksight").describe_folder_resolved_permissions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/describe_folder_resolved_permissions.html)

```python
# describe_folder_resolved_permissions method definition

await def describe_folder_resolved_permissions(
    self,
    *,
    AwsAccountId: str,
    FolderId: str,
    Namespace: str = ...,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> DescribeFolderResolvedPermissionsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeFolderResolvedPermissionsResponseTypeDef](./type_defs.md#describefolderresolvedpermissionsresponsetypedef) 


```python
# describe_folder_resolved_permissions method usage example with argument unpacking

kwargs: DescribeFolderResolvedPermissionsRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "FolderId": ...,
}

parent.describe_folder_resolved_permissions(**kwargs)
```

1. See [:material-code-braces: DescribeFolderResolvedPermissionsRequestTypeDef](./type_defs.md#describefolderresolvedpermissionsrequesttypedef) 

### describe\_group

Returns an Amazon QuickSight group's description and Amazon Resource Name (ARN).

Type annotations and code completion for `#!python session.create_client("quicksight").describe_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/describe_group.html)

```python
# describe_group method definition

await def describe_group(
    self,
    *,
    GroupName: str,
    AwsAccountId: str,
    Namespace: str,
) -> DescribeGroupResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeGroupResponseTypeDef](./type_defs.md#describegroupresponsetypedef) 


```python
# describe_group method usage example with argument unpacking

kwargs: DescribeGroupRequestTypeDef = {  # (1)
    "GroupName": ...,
    "AwsAccountId": ...,
    "Namespace": ...,
}

parent.describe_group(**kwargs)
```

1. See [:material-code-braces: DescribeGroupRequestTypeDef](./type_defs.md#describegrouprequesttypedef) 

### describe\_group\_membership

Use the <code>DescribeGroupMembership</code> operation to determine if a user
is a member of the specified group.

Type annotations and code completion for `#!python session.create_client("quicksight").describe_group_membership` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/describe_group_membership.html)

```python
# describe_group_membership method definition

await def describe_group_membership(
    self,
    *,
    MemberName: str,
    GroupName: str,
    AwsAccountId: str,
    Namespace: str,
) -> DescribeGroupMembershipResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeGroupMembershipResponseTypeDef](./type_defs.md#describegroupmembershipresponsetypedef) 


```python
# describe_group_membership method usage example with argument unpacking

kwargs: DescribeGroupMembershipRequestTypeDef = {  # (1)
    "MemberName": ...,
    "GroupName": ...,
    "AwsAccountId": ...,
    "Namespace": ...,
}

parent.describe_group_membership(**kwargs)
```

1. See [:material-code-braces: DescribeGroupMembershipRequestTypeDef](./type_defs.md#describegroupmembershiprequesttypedef) 

### describe\_iam\_policy\_assignment

Describes an existing IAM policy assignment, as specified by the assignment
name.

Type annotations and code completion for `#!python session.create_client("quicksight").describe_iam_policy_assignment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/describe_iam_policy_assignment.html)

```python
# describe_iam_policy_assignment method definition

await def describe_iam_policy_assignment(
    self,
    *,
    AwsAccountId: str,
    AssignmentName: str,
    Namespace: str,
) -> DescribeIAMPolicyAssignmentResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeIAMPolicyAssignmentResponseTypeDef](./type_defs.md#describeiampolicyassignmentresponsetypedef) 


```python
# describe_iam_policy_assignment method usage example with argument unpacking

kwargs: DescribeIAMPolicyAssignmentRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "AssignmentName": ...,
    "Namespace": ...,
}

parent.describe_iam_policy_assignment(**kwargs)
```

1. See [:material-code-braces: DescribeIAMPolicyAssignmentRequestTypeDef](./type_defs.md#describeiampolicyassignmentrequesttypedef) 

### describe\_ingestion

Describes a SPICE ingestion.

Type annotations and code completion for `#!python session.create_client("quicksight").describe_ingestion` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/describe_ingestion.html)

```python
# describe_ingestion method definition

await def describe_ingestion(
    self,
    *,
    AwsAccountId: str,
    DataSetId: str,
    IngestionId: str,
) -> DescribeIngestionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeIngestionResponseTypeDef](./type_defs.md#describeingestionresponsetypedef) 


```python
# describe_ingestion method usage example with argument unpacking

kwargs: DescribeIngestionRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "DataSetId": ...,
    "IngestionId": ...,
}

parent.describe_ingestion(**kwargs)
```

1. See [:material-code-braces: DescribeIngestionRequestTypeDef](./type_defs.md#describeingestionrequesttypedef) 

### describe\_ip\_restriction

Provides a summary and status of IP rules.

Type annotations and code completion for `#!python session.create_client("quicksight").describe_ip_restriction` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/describe_ip_restriction.html)

```python
# describe_ip_restriction method definition

await def describe_ip_restriction(
    self,
    *,
    AwsAccountId: str,
) -> DescribeIpRestrictionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeIpRestrictionResponseTypeDef](./type_defs.md#describeiprestrictionresponsetypedef) 


```python
# describe_ip_restriction method usage example with argument unpacking

kwargs: DescribeIpRestrictionRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
}

parent.describe_ip_restriction(**kwargs)
```

1. See [:material-code-braces: DescribeIpRestrictionRequestTypeDef](./type_defs.md#describeiprestrictionrequesttypedef) 

### describe\_key\_registration

Describes all customer managed key registrations in a Amazon QuickSight account.

Type annotations and code completion for `#!python session.create_client("quicksight").describe_key_registration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/describe_key_registration.html)

```python
# describe_key_registration method definition

await def describe_key_registration(
    self,
    *,
    AwsAccountId: str,
    DefaultKeyOnly: bool = ...,
) -> DescribeKeyRegistrationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeKeyRegistrationResponseTypeDef](./type_defs.md#describekeyregistrationresponsetypedef) 


```python
# describe_key_registration method usage example with argument unpacking

kwargs: DescribeKeyRegistrationRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
}

parent.describe_key_registration(**kwargs)
```

1. See [:material-code-braces: DescribeKeyRegistrationRequestTypeDef](./type_defs.md#describekeyregistrationrequesttypedef) 

### describe\_namespace

Describes the current namespace.

Type annotations and code completion for `#!python session.create_client("quicksight").describe_namespace` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/describe_namespace.html)

```python
# describe_namespace method definition

await def describe_namespace(
    self,
    *,
    AwsAccountId: str,
    Namespace: str,
) -> DescribeNamespaceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeNamespaceResponseTypeDef](./type_defs.md#describenamespaceresponsetypedef) 


```python
# describe_namespace method usage example with argument unpacking

kwargs: DescribeNamespaceRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "Namespace": ...,
}

parent.describe_namespace(**kwargs)
```

1. See [:material-code-braces: DescribeNamespaceRequestTypeDef](./type_defs.md#describenamespacerequesttypedef) 

### describe\_q\_personalization\_configuration

Describes a personalization configuration.

Type annotations and code completion for `#!python session.create_client("quicksight").describe_q_personalization_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/describe_q_personalization_configuration.html)

```python
# describe_q_personalization_configuration method definition

await def describe_q_personalization_configuration(
    self,
    *,
    AwsAccountId: str,
) -> DescribeQPersonalizationConfigurationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeQPersonalizationConfigurationResponseTypeDef](./type_defs.md#describeqpersonalizationconfigurationresponsetypedef) 


```python
# describe_q_personalization_configuration method usage example with argument unpacking

kwargs: DescribeQPersonalizationConfigurationRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
}

parent.describe_q_personalization_configuration(**kwargs)
```

1. See [:material-code-braces: DescribeQPersonalizationConfigurationRequestTypeDef](./type_defs.md#describeqpersonalizationconfigurationrequesttypedef) 

### describe\_quick\_sight\_q\_search\_configuration

Describes the state of a Amazon QuickSight Q Search configuration.

Type annotations and code completion for `#!python session.create_client("quicksight").describe_quick_sight_q_search_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/describe_quick_sight_q_search_configuration.html)

```python
# describe_quick_sight_q_search_configuration method definition

await def describe_quick_sight_q_search_configuration(
    self,
    *,
    AwsAccountId: str,
) -> DescribeQuickSightQSearchConfigurationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeQuickSightQSearchConfigurationResponseTypeDef](./type_defs.md#describequicksightqsearchconfigurationresponsetypedef) 


```python
# describe_quick_sight_q_search_configuration method usage example with argument unpacking

kwargs: DescribeQuickSightQSearchConfigurationRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
}

parent.describe_quick_sight_q_search_configuration(**kwargs)
```

1. See [:material-code-braces: DescribeQuickSightQSearchConfigurationRequestTypeDef](./type_defs.md#describequicksightqsearchconfigurationrequesttypedef) 

### describe\_refresh\_schedule

Provides a summary of a refresh schedule.

Type annotations and code completion for `#!python session.create_client("quicksight").describe_refresh_schedule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/describe_refresh_schedule.html)

```python
# describe_refresh_schedule method definition

await def describe_refresh_schedule(
    self,
    *,
    AwsAccountId: str,
    DataSetId: str,
    ScheduleId: str,
) -> DescribeRefreshScheduleResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeRefreshScheduleResponseTypeDef](./type_defs.md#describerefreshscheduleresponsetypedef) 


```python
# describe_refresh_schedule method usage example with argument unpacking

kwargs: DescribeRefreshScheduleRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "DataSetId": ...,
    "ScheduleId": ...,
}

parent.describe_refresh_schedule(**kwargs)
```

1. See [:material-code-braces: DescribeRefreshScheduleRequestTypeDef](./type_defs.md#describerefreshschedulerequesttypedef) 

### describe\_role\_custom\_permission

Describes all custom permissions that are mapped to a role.

Type annotations and code completion for `#!python session.create_client("quicksight").describe_role_custom_permission` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/describe_role_custom_permission.html)

```python
# describe_role_custom_permission method definition

await def describe_role_custom_permission(
    self,
    *,
    Role: RoleType,  # (1)
    AwsAccountId: str,
    Namespace: str,
) -> DescribeRoleCustomPermissionResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: RoleType](./literals.md#roletype) 
2. See [:material-code-braces: DescribeRoleCustomPermissionResponseTypeDef](./type_defs.md#describerolecustompermissionresponsetypedef) 


```python
# describe_role_custom_permission method usage example with argument unpacking

kwargs: DescribeRoleCustomPermissionRequestTypeDef = {  # (1)
    "Role": ...,
    "AwsAccountId": ...,
    "Namespace": ...,
}

parent.describe_role_custom_permission(**kwargs)
```

1. See [:material-code-braces: DescribeRoleCustomPermissionRequestTypeDef](./type_defs.md#describerolecustompermissionrequesttypedef) 

### describe\_template

Describes a template's metadata.

Type annotations and code completion for `#!python session.create_client("quicksight").describe_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/describe_template.html)

```python
# describe_template method definition

await def describe_template(
    self,
    *,
    AwsAccountId: str,
    TemplateId: str,
    VersionNumber: int = ...,
    AliasName: str = ...,
) -> DescribeTemplateResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeTemplateResponseTypeDef](./type_defs.md#describetemplateresponsetypedef) 


```python
# describe_template method usage example with argument unpacking

kwargs: DescribeTemplateRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "TemplateId": ...,
}

parent.describe_template(**kwargs)
```

1. See [:material-code-braces: DescribeTemplateRequestTypeDef](./type_defs.md#describetemplaterequesttypedef) 

### describe\_template\_alias

Describes the template alias for a template.

Type annotations and code completion for `#!python session.create_client("quicksight").describe_template_alias` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/describe_template_alias.html)

```python
# describe_template_alias method definition

await def describe_template_alias(
    self,
    *,
    AwsAccountId: str,
    TemplateId: str,
    AliasName: str,
) -> DescribeTemplateAliasResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeTemplateAliasResponseTypeDef](./type_defs.md#describetemplatealiasresponsetypedef) 


```python
# describe_template_alias method usage example with argument unpacking

kwargs: DescribeTemplateAliasRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "TemplateId": ...,
    "AliasName": ...,
}

parent.describe_template_alias(**kwargs)
```

1. See [:material-code-braces: DescribeTemplateAliasRequestTypeDef](./type_defs.md#describetemplatealiasrequesttypedef) 

### describe\_template\_definition

Provides a detailed description of the definition of a template.

Type annotations and code completion for `#!python session.create_client("quicksight").describe_template_definition` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/describe_template_definition.html)

```python
# describe_template_definition method definition

await def describe_template_definition(
    self,
    *,
    AwsAccountId: str,
    TemplateId: str,
    VersionNumber: int = ...,
    AliasName: str = ...,
) -> DescribeTemplateDefinitionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeTemplateDefinitionResponseTypeDef](./type_defs.md#describetemplatedefinitionresponsetypedef) 


```python
# describe_template_definition method usage example with argument unpacking

kwargs: DescribeTemplateDefinitionRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "TemplateId": ...,
}

parent.describe_template_definition(**kwargs)
```

1. See [:material-code-braces: DescribeTemplateDefinitionRequestTypeDef](./type_defs.md#describetemplatedefinitionrequesttypedef) 

### describe\_template\_permissions

Describes read and write permissions on a template.

Type annotations and code completion for `#!python session.create_client("quicksight").describe_template_permissions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/describe_template_permissions.html)

```python
# describe_template_permissions method definition

await def describe_template_permissions(
    self,
    *,
    AwsAccountId: str,
    TemplateId: str,
) -> DescribeTemplatePermissionsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeTemplatePermissionsResponseTypeDef](./type_defs.md#describetemplatepermissionsresponsetypedef) 


```python
# describe_template_permissions method usage example with argument unpacking

kwargs: DescribeTemplatePermissionsRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "TemplateId": ...,
}

parent.describe_template_permissions(**kwargs)
```

1. See [:material-code-braces: DescribeTemplatePermissionsRequestTypeDef](./type_defs.md#describetemplatepermissionsrequesttypedef) 

### describe\_theme

Describes a theme.

Type annotations and code completion for `#!python session.create_client("quicksight").describe_theme` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/describe_theme.html)

```python
# describe_theme method definition

await def describe_theme(
    self,
    *,
    AwsAccountId: str,
    ThemeId: str,
    VersionNumber: int = ...,
    AliasName: str = ...,
) -> DescribeThemeResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeThemeResponseTypeDef](./type_defs.md#describethemeresponsetypedef) 


```python
# describe_theme method usage example with argument unpacking

kwargs: DescribeThemeRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "ThemeId": ...,
}

parent.describe_theme(**kwargs)
```

1. See [:material-code-braces: DescribeThemeRequestTypeDef](./type_defs.md#describethemerequesttypedef) 

### describe\_theme\_alias

Describes the alias for a theme.

Type annotations and code completion for `#!python session.create_client("quicksight").describe_theme_alias` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/describe_theme_alias.html)

```python
# describe_theme_alias method definition

await def describe_theme_alias(
    self,
    *,
    AwsAccountId: str,
    ThemeId: str,
    AliasName: str,
) -> DescribeThemeAliasResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeThemeAliasResponseTypeDef](./type_defs.md#describethemealiasresponsetypedef) 


```python
# describe_theme_alias method usage example with argument unpacking

kwargs: DescribeThemeAliasRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "ThemeId": ...,
    "AliasName": ...,
}

parent.describe_theme_alias(**kwargs)
```

1. See [:material-code-braces: DescribeThemeAliasRequestTypeDef](./type_defs.md#describethemealiasrequesttypedef) 

### describe\_theme\_permissions

Describes the read and write permissions for a theme.

Type annotations and code completion for `#!python session.create_client("quicksight").describe_theme_permissions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/describe_theme_permissions.html)

```python
# describe_theme_permissions method definition

await def describe_theme_permissions(
    self,
    *,
    AwsAccountId: str,
    ThemeId: str,
) -> DescribeThemePermissionsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeThemePermissionsResponseTypeDef](./type_defs.md#describethemepermissionsresponsetypedef) 


```python
# describe_theme_permissions method usage example with argument unpacking

kwargs: DescribeThemePermissionsRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "ThemeId": ...,
}

parent.describe_theme_permissions(**kwargs)
```

1. See [:material-code-braces: DescribeThemePermissionsRequestTypeDef](./type_defs.md#describethemepermissionsrequesttypedef) 

### describe\_topic

Describes a topic.

Type annotations and code completion for `#!python session.create_client("quicksight").describe_topic` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/describe_topic.html)

```python
# describe_topic method definition

await def describe_topic(
    self,
    *,
    AwsAccountId: str,
    TopicId: str,
) -> DescribeTopicResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeTopicResponseTypeDef](./type_defs.md#describetopicresponsetypedef) 


```python
# describe_topic method usage example with argument unpacking

kwargs: DescribeTopicRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "TopicId": ...,
}

parent.describe_topic(**kwargs)
```

1. See [:material-code-braces: DescribeTopicRequestTypeDef](./type_defs.md#describetopicrequesttypedef) 

### describe\_topic\_permissions

Describes the permissions of a topic.

Type annotations and code completion for `#!python session.create_client("quicksight").describe_topic_permissions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/describe_topic_permissions.html)

```python
# describe_topic_permissions method definition

await def describe_topic_permissions(
    self,
    *,
    AwsAccountId: str,
    TopicId: str,
) -> DescribeTopicPermissionsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeTopicPermissionsResponseTypeDef](./type_defs.md#describetopicpermissionsresponsetypedef) 


```python
# describe_topic_permissions method usage example with argument unpacking

kwargs: DescribeTopicPermissionsRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "TopicId": ...,
}

parent.describe_topic_permissions(**kwargs)
```

1. See [:material-code-braces: DescribeTopicPermissionsRequestTypeDef](./type_defs.md#describetopicpermissionsrequesttypedef) 

### describe\_topic\_refresh

Describes the status of a topic refresh.

Type annotations and code completion for `#!python session.create_client("quicksight").describe_topic_refresh` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/describe_topic_refresh.html)

```python
# describe_topic_refresh method definition

await def describe_topic_refresh(
    self,
    *,
    AwsAccountId: str,
    TopicId: str,
    RefreshId: str,
) -> DescribeTopicRefreshResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeTopicRefreshResponseTypeDef](./type_defs.md#describetopicrefreshresponsetypedef) 


```python
# describe_topic_refresh method usage example with argument unpacking

kwargs: DescribeTopicRefreshRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "TopicId": ...,
    "RefreshId": ...,
}

parent.describe_topic_refresh(**kwargs)
```

1. See [:material-code-braces: DescribeTopicRefreshRequestTypeDef](./type_defs.md#describetopicrefreshrequesttypedef) 

### describe\_topic\_refresh\_schedule

Deletes a topic refresh schedule.

Type annotations and code completion for `#!python session.create_client("quicksight").describe_topic_refresh_schedule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/describe_topic_refresh_schedule.html)

```python
# describe_topic_refresh_schedule method definition

await def describe_topic_refresh_schedule(
    self,
    *,
    AwsAccountId: str,
    TopicId: str,
    DatasetId: str,
) -> DescribeTopicRefreshScheduleResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeTopicRefreshScheduleResponseTypeDef](./type_defs.md#describetopicrefreshscheduleresponsetypedef) 


```python
# describe_topic_refresh_schedule method usage example with argument unpacking

kwargs: DescribeTopicRefreshScheduleRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "TopicId": ...,
    "DatasetId": ...,
}

parent.describe_topic_refresh_schedule(**kwargs)
```

1. See [:material-code-braces: DescribeTopicRefreshScheduleRequestTypeDef](./type_defs.md#describetopicrefreshschedulerequesttypedef) 

### describe\_user

Returns information about a user, given the user name.

Type annotations and code completion for `#!python session.create_client("quicksight").describe_user` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/describe_user.html)

```python
# describe_user method definition

await def describe_user(
    self,
    *,
    UserName: str,
    AwsAccountId: str,
    Namespace: str,
) -> DescribeUserResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeUserResponseTypeDef](./type_defs.md#describeuserresponsetypedef) 


```python
# describe_user method usage example with argument unpacking

kwargs: DescribeUserRequestTypeDef = {  # (1)
    "UserName": ...,
    "AwsAccountId": ...,
    "Namespace": ...,
}

parent.describe_user(**kwargs)
```

1. See [:material-code-braces: DescribeUserRequestTypeDef](./type_defs.md#describeuserrequesttypedef) 

### describe\_vpc\_connection

Describes a VPC connection.

Type annotations and code completion for `#!python session.create_client("quicksight").describe_vpc_connection` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/describe_vpc_connection.html)

```python
# describe_vpc_connection method definition

await def describe_vpc_connection(
    self,
    *,
    AwsAccountId: str,
    VPCConnectionId: str,
) -> DescribeVPCConnectionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeVPCConnectionResponseTypeDef](./type_defs.md#describevpcconnectionresponsetypedef) 


```python
# describe_vpc_connection method usage example with argument unpacking

kwargs: DescribeVPCConnectionRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "VPCConnectionId": ...,
}

parent.describe_vpc_connection(**kwargs)
```

1. See [:material-code-braces: DescribeVPCConnectionRequestTypeDef](./type_defs.md#describevpcconnectionrequesttypedef) 

### generate\_embed\_url\_for\_anonymous\_user

Generates an embed URL that you can use to embed an Amazon QuickSight dashboard
or visual in your website, without having to register any reader users.

Type annotations and code completion for `#!python session.create_client("quicksight").generate_embed_url_for_anonymous_user` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/generate_embed_url_for_anonymous_user.html)

```python
# generate_embed_url_for_anonymous_user method definition

await def generate_embed_url_for_anonymous_user(
    self,
    *,
    AwsAccountId: str,
    Namespace: str,
    AuthorizedResourceArns: Sequence[str],
    ExperienceConfiguration: AnonymousUserEmbeddingExperienceConfigurationTypeDef,  # (1)
    SessionLifetimeInMinutes: int = ...,
    SessionTags: Sequence[SessionTagTypeDef] = ...,  # (2)
    AllowedDomains: Sequence[str] = ...,
) -> GenerateEmbedUrlForAnonymousUserResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: AnonymousUserEmbeddingExperienceConfigurationTypeDef](./type_defs.md#anonymoususerembeddingexperienceconfigurationtypedef) 
2. See [:material-code-braces: SessionTagTypeDef](./type_defs.md#sessiontagtypedef) 
3. See [:material-code-braces: GenerateEmbedUrlForAnonymousUserResponseTypeDef](./type_defs.md#generateembedurlforanonymoususerresponsetypedef) 


```python
# generate_embed_url_for_anonymous_user method usage example with argument unpacking

kwargs: GenerateEmbedUrlForAnonymousUserRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "Namespace": ...,
    "AuthorizedResourceArns": ...,
    "ExperienceConfiguration": ...,
}

parent.generate_embed_url_for_anonymous_user(**kwargs)
```

1. See [:material-code-braces: GenerateEmbedUrlForAnonymousUserRequestTypeDef](./type_defs.md#generateembedurlforanonymoususerrequesttypedef) 

### generate\_embed\_url\_for\_registered\_user

Generates an embed URL that you can use to embed an Amazon QuickSight
experience in your website.

Type annotations and code completion for `#!python session.create_client("quicksight").generate_embed_url_for_registered_user` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/generate_embed_url_for_registered_user.html)

```python
# generate_embed_url_for_registered_user method definition

await def generate_embed_url_for_registered_user(
    self,
    *,
    AwsAccountId: str,
    UserArn: str,
    ExperienceConfiguration: RegisteredUserEmbeddingExperienceConfigurationTypeDef,  # (1)
    SessionLifetimeInMinutes: int = ...,
    AllowedDomains: Sequence[str] = ...,
) -> GenerateEmbedUrlForRegisteredUserResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: RegisteredUserEmbeddingExperienceConfigurationTypeDef](./type_defs.md#registereduserembeddingexperienceconfigurationtypedef) 
2. See [:material-code-braces: GenerateEmbedUrlForRegisteredUserResponseTypeDef](./type_defs.md#generateembedurlforregistereduserresponsetypedef) 


```python
# generate_embed_url_for_registered_user method usage example with argument unpacking

kwargs: GenerateEmbedUrlForRegisteredUserRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "UserArn": ...,
    "ExperienceConfiguration": ...,
}

parent.generate_embed_url_for_registered_user(**kwargs)
```

1. See [:material-code-braces: GenerateEmbedUrlForRegisteredUserRequestTypeDef](./type_defs.md#generateembedurlforregistereduserrequesttypedef) 

### generate\_embed\_url\_for\_registered\_user\_with\_identity

Generates an embed URL that you can use to embed an Amazon QuickSight
experience in your website.

Type annotations and code completion for `#!python session.create_client("quicksight").generate_embed_url_for_registered_user_with_identity` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/generate_embed_url_for_registered_user_with_identity.html)

```python
# generate_embed_url_for_registered_user_with_identity method definition

await def generate_embed_url_for_registered_user_with_identity(
    self,
    *,
    AwsAccountId: str,
    ExperienceConfiguration: RegisteredUserEmbeddingExperienceConfigurationTypeDef,  # (1)
    SessionLifetimeInMinutes: int = ...,
    AllowedDomains: Sequence[str] = ...,
) -> GenerateEmbedUrlForRegisteredUserWithIdentityResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: RegisteredUserEmbeddingExperienceConfigurationTypeDef](./type_defs.md#registereduserembeddingexperienceconfigurationtypedef) 
2. See [:material-code-braces: GenerateEmbedUrlForRegisteredUserWithIdentityResponseTypeDef](./type_defs.md#generateembedurlforregistereduserwithidentityresponsetypedef) 


```python
# generate_embed_url_for_registered_user_with_identity method usage example with argument unpacking

kwargs: GenerateEmbedUrlForRegisteredUserWithIdentityRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "ExperienceConfiguration": ...,
}

parent.generate_embed_url_for_registered_user_with_identity(**kwargs)
```

1. See [:material-code-braces: GenerateEmbedUrlForRegisteredUserWithIdentityRequestTypeDef](./type_defs.md#generateembedurlforregistereduserwithidentityrequesttypedef) 

### get\_dashboard\_embed\_url

Generates a temporary session URL and authorization code(bearer token) that you
can use to embed an Amazon QuickSight read-only dashboard in your website or
application.

Type annotations and code completion for `#!python session.create_client("quicksight").get_dashboard_embed_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/get_dashboard_embed_url.html)

```python
# get_dashboard_embed_url method definition

await def get_dashboard_embed_url(
    self,
    *,
    AwsAccountId: str,
    DashboardId: str,
    IdentityType: EmbeddingIdentityTypeType,  # (1)
    SessionLifetimeInMinutes: int = ...,
    UndoRedoDisabled: bool = ...,
    ResetDisabled: bool = ...,
    StatePersistenceEnabled: bool = ...,
    UserArn: str = ...,
    Namespace: str = ...,
    AdditionalDashboardIds: Sequence[str] = ...,
) -> GetDashboardEmbedUrlResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: EmbeddingIdentityTypeType](./literals.md#embeddingidentitytypetype) 
2. See [:material-code-braces: GetDashboardEmbedUrlResponseTypeDef](./type_defs.md#getdashboardembedurlresponsetypedef) 


```python
# get_dashboard_embed_url method usage example with argument unpacking

kwargs: GetDashboardEmbedUrlRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "DashboardId": ...,
    "IdentityType": ...,
}

parent.get_dashboard_embed_url(**kwargs)
```

1. See [:material-code-braces: GetDashboardEmbedUrlRequestTypeDef](./type_defs.md#getdashboardembedurlrequesttypedef) 

### get\_session\_embed\_url

Generates a session URL and authorization code that you can use to embed the
Amazon Amazon QuickSight console in your web server code.

Type annotations and code completion for `#!python session.create_client("quicksight").get_session_embed_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/get_session_embed_url.html)

```python
# get_session_embed_url method definition

await def get_session_embed_url(
    self,
    *,
    AwsAccountId: str,
    EntryPoint: str = ...,
    SessionLifetimeInMinutes: int = ...,
    UserArn: str = ...,
) -> GetSessionEmbedUrlResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetSessionEmbedUrlResponseTypeDef](./type_defs.md#getsessionembedurlresponsetypedef) 


```python
# get_session_embed_url method usage example with argument unpacking

kwargs: GetSessionEmbedUrlRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
}

parent.get_session_embed_url(**kwargs)
```

1. See [:material-code-braces: GetSessionEmbedUrlRequestTypeDef](./type_defs.md#getsessionembedurlrequesttypedef) 

### list\_analyses

Lists Amazon QuickSight analyses that exist in the specified Amazon Web
Services account.

Type annotations and code completion for `#!python session.create_client("quicksight").list_analyses` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/list_analyses.html)

```python
# list_analyses method definition

await def list_analyses(
    self,
    *,
    AwsAccountId: str,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListAnalysesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListAnalysesResponseTypeDef](./type_defs.md#listanalysesresponsetypedef) 


```python
# list_analyses method usage example with argument unpacking

kwargs: ListAnalysesRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
}

parent.list_analyses(**kwargs)
```

1. See [:material-code-braces: ListAnalysesRequestTypeDef](./type_defs.md#listanalysesrequesttypedef) 

### list\_asset\_bundle\_export\_jobs

Lists all asset bundle export jobs that have been taken place in the last 14
days.

Type annotations and code completion for `#!python session.create_client("quicksight").list_asset_bundle_export_jobs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/list_asset_bundle_export_jobs.html)

```python
# list_asset_bundle_export_jobs method definition

await def list_asset_bundle_export_jobs(
    self,
    *,
    AwsAccountId: str,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListAssetBundleExportJobsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListAssetBundleExportJobsResponseTypeDef](./type_defs.md#listassetbundleexportjobsresponsetypedef) 


```python
# list_asset_bundle_export_jobs method usage example with argument unpacking

kwargs: ListAssetBundleExportJobsRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
}

parent.list_asset_bundle_export_jobs(**kwargs)
```

1. See [:material-code-braces: ListAssetBundleExportJobsRequestTypeDef](./type_defs.md#listassetbundleexportjobsrequesttypedef) 

### list\_asset\_bundle\_import\_jobs

Lists all asset bundle import jobs that have taken place in the last 14 days.

Type annotations and code completion for `#!python session.create_client("quicksight").list_asset_bundle_import_jobs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/list_asset_bundle_import_jobs.html)

```python
# list_asset_bundle_import_jobs method definition

await def list_asset_bundle_import_jobs(
    self,
    *,
    AwsAccountId: str,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListAssetBundleImportJobsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListAssetBundleImportJobsResponseTypeDef](./type_defs.md#listassetbundleimportjobsresponsetypedef) 


```python
# list_asset_bundle_import_jobs method usage example with argument unpacking

kwargs: ListAssetBundleImportJobsRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
}

parent.list_asset_bundle_import_jobs(**kwargs)
```

1. See [:material-code-braces: ListAssetBundleImportJobsRequestTypeDef](./type_defs.md#listassetbundleimportjobsrequesttypedef) 

### list\_brands

Lists all brands in an Amazon QuickSight account.

Type annotations and code completion for `#!python session.create_client("quicksight").list_brands` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/list_brands.html)

```python
# list_brands method definition

await def list_brands(
    self,
    *,
    AwsAccountId: str,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListBrandsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListBrandsResponseTypeDef](./type_defs.md#listbrandsresponsetypedef) 


```python
# list_brands method usage example with argument unpacking

kwargs: ListBrandsRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
}

parent.list_brands(**kwargs)
```

1. See [:material-code-braces: ListBrandsRequestTypeDef](./type_defs.md#listbrandsrequesttypedef) 

### list\_custom\_permissions

Returns a list of all the custom permissions profiles.

Type annotations and code completion for `#!python session.create_client("quicksight").list_custom_permissions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/list_custom_permissions.html)

```python
# list_custom_permissions method definition

await def list_custom_permissions(
    self,
    *,
    AwsAccountId: str,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListCustomPermissionsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListCustomPermissionsResponseTypeDef](./type_defs.md#listcustompermissionsresponsetypedef) 


```python
# list_custom_permissions method usage example with argument unpacking

kwargs: ListCustomPermissionsRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
}

parent.list_custom_permissions(**kwargs)
```

1. See [:material-code-braces: ListCustomPermissionsRequestTypeDef](./type_defs.md#listcustompermissionsrequesttypedef) 

### list\_dashboard\_versions

Lists all the versions of the dashboards in the Amazon QuickSight subscription.

Type annotations and code completion for `#!python session.create_client("quicksight").list_dashboard_versions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/list_dashboard_versions.html)

```python
# list_dashboard_versions method definition

await def list_dashboard_versions(
    self,
    *,
    AwsAccountId: str,
    DashboardId: str,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListDashboardVersionsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListDashboardVersionsResponseTypeDef](./type_defs.md#listdashboardversionsresponsetypedef) 


```python
# list_dashboard_versions method usage example with argument unpacking

kwargs: ListDashboardVersionsRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "DashboardId": ...,
}

parent.list_dashboard_versions(**kwargs)
```

1. See [:material-code-braces: ListDashboardVersionsRequestTypeDef](./type_defs.md#listdashboardversionsrequesttypedef) 

### list\_dashboards

Lists dashboards in an Amazon Web Services account.

Type annotations and code completion for `#!python session.create_client("quicksight").list_dashboards` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/list_dashboards.html)

```python
# list_dashboards method definition

await def list_dashboards(
    self,
    *,
    AwsAccountId: str,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListDashboardsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListDashboardsResponseTypeDef](./type_defs.md#listdashboardsresponsetypedef) 


```python
# list_dashboards method usage example with argument unpacking

kwargs: ListDashboardsRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
}

parent.list_dashboards(**kwargs)
```

1. See [:material-code-braces: ListDashboardsRequestTypeDef](./type_defs.md#listdashboardsrequesttypedef) 

### list\_data\_sets

Lists all of the datasets belonging to the current Amazon Web Services account
in an Amazon Web Services Region.

Type annotations and code completion for `#!python session.create_client("quicksight").list_data_sets` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/list_data_sets.html)

```python
# list_data_sets method definition

await def list_data_sets(
    self,
    *,
    AwsAccountId: str,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListDataSetsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListDataSetsResponseTypeDef](./type_defs.md#listdatasetsresponsetypedef) 


```python
# list_data_sets method usage example with argument unpacking

kwargs: ListDataSetsRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
}

parent.list_data_sets(**kwargs)
```

1. See [:material-code-braces: ListDataSetsRequestTypeDef](./type_defs.md#listdatasetsrequesttypedef) 

### list\_data\_sources

Lists data sources in current Amazon Web Services Region that belong to this
Amazon Web Services account.

Type annotations and code completion for `#!python session.create_client("quicksight").list_data_sources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/list_data_sources.html)

```python
# list_data_sources method definition

await def list_data_sources(
    self,
    *,
    AwsAccountId: str,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListDataSourcesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListDataSourcesResponseTypeDef](./type_defs.md#listdatasourcesresponsetypedef) 


```python
# list_data_sources method usage example with argument unpacking

kwargs: ListDataSourcesRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
}

parent.list_data_sources(**kwargs)
```

1. See [:material-code-braces: ListDataSourcesRequestTypeDef](./type_defs.md#listdatasourcesrequesttypedef) 

### list\_folder\_members

List all assets (<code>DASHBOARD</code>, <code>ANALYSIS</code>, and
<code>DATASET</code>) in a folder.

Type annotations and code completion for `#!python session.create_client("quicksight").list_folder_members` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/list_folder_members.html)

```python
# list_folder_members method definition

await def list_folder_members(
    self,
    *,
    AwsAccountId: str,
    FolderId: str,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListFolderMembersResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListFolderMembersResponseTypeDef](./type_defs.md#listfoldermembersresponsetypedef) 


```python
# list_folder_members method usage example with argument unpacking

kwargs: ListFolderMembersRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "FolderId": ...,
}

parent.list_folder_members(**kwargs)
```

1. See [:material-code-braces: ListFolderMembersRequestTypeDef](./type_defs.md#listfoldermembersrequesttypedef) 

### list\_folders

Lists all folders in an account.

Type annotations and code completion for `#!python session.create_client("quicksight").list_folders` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/list_folders.html)

```python
# list_folders method definition

await def list_folders(
    self,
    *,
    AwsAccountId: str,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListFoldersResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListFoldersResponseTypeDef](./type_defs.md#listfoldersresponsetypedef) 


```python
# list_folders method usage example with argument unpacking

kwargs: ListFoldersRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
}

parent.list_folders(**kwargs)
```

1. See [:material-code-braces: ListFoldersRequestTypeDef](./type_defs.md#listfoldersrequesttypedef) 

### list\_folders\_for\_resource

List all folders that a resource is a member of.

Type annotations and code completion for `#!python session.create_client("quicksight").list_folders_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/list_folders_for_resource.html)

```python
# list_folders_for_resource method definition

await def list_folders_for_resource(
    self,
    *,
    AwsAccountId: str,
    ResourceArn: str,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListFoldersForResourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListFoldersForResourceResponseTypeDef](./type_defs.md#listfoldersforresourceresponsetypedef) 


```python
# list_folders_for_resource method usage example with argument unpacking

kwargs: ListFoldersForResourceRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "ResourceArn": ...,
}

parent.list_folders_for_resource(**kwargs)
```

1. See [:material-code-braces: ListFoldersForResourceRequestTypeDef](./type_defs.md#listfoldersforresourcerequesttypedef) 

### list\_group\_memberships

Lists member users in a group.

Type annotations and code completion for `#!python session.create_client("quicksight").list_group_memberships` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/list_group_memberships.html)

```python
# list_group_memberships method definition

await def list_group_memberships(
    self,
    *,
    GroupName: str,
    AwsAccountId: str,
    Namespace: str,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListGroupMembershipsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListGroupMembershipsResponseTypeDef](./type_defs.md#listgroupmembershipsresponsetypedef) 


```python
# list_group_memberships method usage example with argument unpacking

kwargs: ListGroupMembershipsRequestTypeDef = {  # (1)
    "GroupName": ...,
    "AwsAccountId": ...,
    "Namespace": ...,
}

parent.list_group_memberships(**kwargs)
```

1. See [:material-code-braces: ListGroupMembershipsRequestTypeDef](./type_defs.md#listgroupmembershipsrequesttypedef) 

### list\_groups

Lists all user groups in Amazon QuickSight.

Type annotations and code completion for `#!python session.create_client("quicksight").list_groups` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/list_groups.html)

```python
# list_groups method definition

await def list_groups(
    self,
    *,
    AwsAccountId: str,
    Namespace: str,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListGroupsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListGroupsResponseTypeDef](./type_defs.md#listgroupsresponsetypedef) 


```python
# list_groups method usage example with argument unpacking

kwargs: ListGroupsRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "Namespace": ...,
}

parent.list_groups(**kwargs)
```

1. See [:material-code-braces: ListGroupsRequestTypeDef](./type_defs.md#listgroupsrequesttypedef) 

### list\_iam\_policy\_assignments

Lists the IAM policy assignments in the current Amazon QuickSight account.

Type annotations and code completion for `#!python session.create_client("quicksight").list_iam_policy_assignments` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/list_iam_policy_assignments.html)

```python
# list_iam_policy_assignments method definition

await def list_iam_policy_assignments(
    self,
    *,
    AwsAccountId: str,
    Namespace: str,
    AssignmentStatus: AssignmentStatusType = ...,  # (1)
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListIAMPolicyAssignmentsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: AssignmentStatusType](./literals.md#assignmentstatustype) 
2. See [:material-code-braces: ListIAMPolicyAssignmentsResponseTypeDef](./type_defs.md#listiampolicyassignmentsresponsetypedef) 


```python
# list_iam_policy_assignments method usage example with argument unpacking

kwargs: ListIAMPolicyAssignmentsRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "Namespace": ...,
}

parent.list_iam_policy_assignments(**kwargs)
```

1. See [:material-code-braces: ListIAMPolicyAssignmentsRequestTypeDef](./type_defs.md#listiampolicyassignmentsrequesttypedef) 

### list\_iam\_policy\_assignments\_for\_user

Lists all of the IAM policy assignments, including the Amazon Resource Names
(ARNs), for the IAM policies assigned to the specified user and group, or
groups that the user belongs to.

Type annotations and code completion for `#!python session.create_client("quicksight").list_iam_policy_assignments_for_user` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/list_iam_policy_assignments_for_user.html)

```python
# list_iam_policy_assignments_for_user method definition

await def list_iam_policy_assignments_for_user(
    self,
    *,
    AwsAccountId: str,
    UserName: str,
    Namespace: str,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListIAMPolicyAssignmentsForUserResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListIAMPolicyAssignmentsForUserResponseTypeDef](./type_defs.md#listiampolicyassignmentsforuserresponsetypedef) 


```python
# list_iam_policy_assignments_for_user method usage example with argument unpacking

kwargs: ListIAMPolicyAssignmentsForUserRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "UserName": ...,
    "Namespace": ...,
}

parent.list_iam_policy_assignments_for_user(**kwargs)
```

1. See [:material-code-braces: ListIAMPolicyAssignmentsForUserRequestTypeDef](./type_defs.md#listiampolicyassignmentsforuserrequesttypedef) 

### list\_identity\_propagation\_configs

Lists all services and authorized targets that the Amazon QuickSight IAM
Identity Center application can access.

Type annotations and code completion for `#!python session.create_client("quicksight").list_identity_propagation_configs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/list_identity_propagation_configs.html)

```python
# list_identity_propagation_configs method definition

await def list_identity_propagation_configs(
    self,
    *,
    AwsAccountId: str,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListIdentityPropagationConfigsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListIdentityPropagationConfigsResponseTypeDef](./type_defs.md#listidentitypropagationconfigsresponsetypedef) 


```python
# list_identity_propagation_configs method usage example with argument unpacking

kwargs: ListIdentityPropagationConfigsRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
}

parent.list_identity_propagation_configs(**kwargs)
```

1. See [:material-code-braces: ListIdentityPropagationConfigsRequestTypeDef](./type_defs.md#listidentitypropagationconfigsrequesttypedef) 

### list\_ingestions

Lists the history of SPICE ingestions for a dataset.

Type annotations and code completion for `#!python session.create_client("quicksight").list_ingestions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/list_ingestions.html)

```python
# list_ingestions method definition

await def list_ingestions(
    self,
    *,
    DataSetId: str,
    AwsAccountId: str,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListIngestionsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListIngestionsResponseTypeDef](./type_defs.md#listingestionsresponsetypedef) 


```python
# list_ingestions method usage example with argument unpacking

kwargs: ListIngestionsRequestTypeDef = {  # (1)
    "DataSetId": ...,
    "AwsAccountId": ...,
}

parent.list_ingestions(**kwargs)
```

1. See [:material-code-braces: ListIngestionsRequestTypeDef](./type_defs.md#listingestionsrequesttypedef) 

### list\_namespaces

Lists the namespaces for the specified Amazon Web Services account.

Type annotations and code completion for `#!python session.create_client("quicksight").list_namespaces` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/list_namespaces.html)

```python
# list_namespaces method definition

await def list_namespaces(
    self,
    *,
    AwsAccountId: str,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListNamespacesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListNamespacesResponseTypeDef](./type_defs.md#listnamespacesresponsetypedef) 


```python
# list_namespaces method usage example with argument unpacking

kwargs: ListNamespacesRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
}

parent.list_namespaces(**kwargs)
```

1. See [:material-code-braces: ListNamespacesRequestTypeDef](./type_defs.md#listnamespacesrequesttypedef) 

### list\_refresh\_schedules

Lists the refresh schedules of a dataset.

Type annotations and code completion for `#!python session.create_client("quicksight").list_refresh_schedules` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/list_refresh_schedules.html)

```python
# list_refresh_schedules method definition

await def list_refresh_schedules(
    self,
    *,
    AwsAccountId: str,
    DataSetId: str,
) -> ListRefreshSchedulesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListRefreshSchedulesResponseTypeDef](./type_defs.md#listrefreshschedulesresponsetypedef) 


```python
# list_refresh_schedules method usage example with argument unpacking

kwargs: ListRefreshSchedulesRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "DataSetId": ...,
}

parent.list_refresh_schedules(**kwargs)
```

1. See [:material-code-braces: ListRefreshSchedulesRequestTypeDef](./type_defs.md#listrefreshschedulesrequesttypedef) 

### list\_role\_memberships

Lists all groups that are associated with a role.

Type annotations and code completion for `#!python session.create_client("quicksight").list_role_memberships` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/list_role_memberships.html)

```python
# list_role_memberships method definition

await def list_role_memberships(
    self,
    *,
    Role: RoleType,  # (1)
    AwsAccountId: str,
    Namespace: str,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListRoleMembershipsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: RoleType](./literals.md#roletype) 
2. See [:material-code-braces: ListRoleMembershipsResponseTypeDef](./type_defs.md#listrolemembershipsresponsetypedef) 


```python
# list_role_memberships method usage example with argument unpacking

kwargs: ListRoleMembershipsRequestTypeDef = {  # (1)
    "Role": ...,
    "AwsAccountId": ...,
    "Namespace": ...,
}

parent.list_role_memberships(**kwargs)
```

1. See [:material-code-braces: ListRoleMembershipsRequestTypeDef](./type_defs.md#listrolemembershipsrequesttypedef) 

### list\_tags\_for\_resource

Lists the tags assigned to a resource.

Type annotations and code completion for `#!python session.create_client("quicksight").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/list_tags_for_resource.html)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    ResourceArn: str,
) -> ListTagsForResourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef) 


```python
# list_tags_for_resource method usage example with argument unpacking

kwargs: ListTagsForResourceRequestTypeDef = {  # (1)
    "ResourceArn": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestTypeDef](./type_defs.md#listtagsforresourcerequesttypedef) 

### list\_template\_aliases

Lists all the aliases of a template.

Type annotations and code completion for `#!python session.create_client("quicksight").list_template_aliases` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/list_template_aliases.html)

```python
# list_template_aliases method definition

await def list_template_aliases(
    self,
    *,
    AwsAccountId: str,
    TemplateId: str,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListTemplateAliasesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTemplateAliasesResponseTypeDef](./type_defs.md#listtemplatealiasesresponsetypedef) 


```python
# list_template_aliases method usage example with argument unpacking

kwargs: ListTemplateAliasesRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "TemplateId": ...,
}

parent.list_template_aliases(**kwargs)
```

1. See [:material-code-braces: ListTemplateAliasesRequestTypeDef](./type_defs.md#listtemplatealiasesrequesttypedef) 

### list\_template\_versions

Lists all the versions of the templates in the current Amazon QuickSight
account.

Type annotations and code completion for `#!python session.create_client("quicksight").list_template_versions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/list_template_versions.html)

```python
# list_template_versions method definition

await def list_template_versions(
    self,
    *,
    AwsAccountId: str,
    TemplateId: str,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListTemplateVersionsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTemplateVersionsResponseTypeDef](./type_defs.md#listtemplateversionsresponsetypedef) 


```python
# list_template_versions method usage example with argument unpacking

kwargs: ListTemplateVersionsRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "TemplateId": ...,
}

parent.list_template_versions(**kwargs)
```

1. See [:material-code-braces: ListTemplateVersionsRequestTypeDef](./type_defs.md#listtemplateversionsrequesttypedef) 

### list\_templates

Lists all the templates in the current Amazon QuickSight account.

Type annotations and code completion for `#!python session.create_client("quicksight").list_templates` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/list_templates.html)

```python
# list_templates method definition

await def list_templates(
    self,
    *,
    AwsAccountId: str,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListTemplatesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTemplatesResponseTypeDef](./type_defs.md#listtemplatesresponsetypedef) 


```python
# list_templates method usage example with argument unpacking

kwargs: ListTemplatesRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
}

parent.list_templates(**kwargs)
```

1. See [:material-code-braces: ListTemplatesRequestTypeDef](./type_defs.md#listtemplatesrequesttypedef) 

### list\_theme\_aliases

Lists all the aliases of a theme.

Type annotations and code completion for `#!python session.create_client("quicksight").list_theme_aliases` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/list_theme_aliases.html)

```python
# list_theme_aliases method definition

await def list_theme_aliases(
    self,
    *,
    AwsAccountId: str,
    ThemeId: str,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListThemeAliasesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListThemeAliasesResponseTypeDef](./type_defs.md#listthemealiasesresponsetypedef) 


```python
# list_theme_aliases method usage example with argument unpacking

kwargs: ListThemeAliasesRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "ThemeId": ...,
}

parent.list_theme_aliases(**kwargs)
```

1. See [:material-code-braces: ListThemeAliasesRequestTypeDef](./type_defs.md#listthemealiasesrequesttypedef) 

### list\_theme\_versions

Lists all the versions of the themes in the current Amazon Web Services account.

Type annotations and code completion for `#!python session.create_client("quicksight").list_theme_versions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/list_theme_versions.html)

```python
# list_theme_versions method definition

await def list_theme_versions(
    self,
    *,
    AwsAccountId: str,
    ThemeId: str,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListThemeVersionsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListThemeVersionsResponseTypeDef](./type_defs.md#listthemeversionsresponsetypedef) 


```python
# list_theme_versions method usage example with argument unpacking

kwargs: ListThemeVersionsRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "ThemeId": ...,
}

parent.list_theme_versions(**kwargs)
```

1. See [:material-code-braces: ListThemeVersionsRequestTypeDef](./type_defs.md#listthemeversionsrequesttypedef) 

### list\_themes

Lists all the themes in the current Amazon Web Services account.

Type annotations and code completion for `#!python session.create_client("quicksight").list_themes` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/list_themes.html)

```python
# list_themes method definition

await def list_themes(
    self,
    *,
    AwsAccountId: str,
    NextToken: str = ...,
    MaxResults: int = ...,
    Type: ThemeTypeType = ...,  # (1)
) -> ListThemesResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ThemeTypeType](./literals.md#themetypetype) 
2. See [:material-code-braces: ListThemesResponseTypeDef](./type_defs.md#listthemesresponsetypedef) 


```python
# list_themes method usage example with argument unpacking

kwargs: ListThemesRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
}

parent.list_themes(**kwargs)
```

1. See [:material-code-braces: ListThemesRequestTypeDef](./type_defs.md#listthemesrequesttypedef) 

### list\_topic\_refresh\_schedules

Lists all of the refresh schedules for a topic.

Type annotations and code completion for `#!python session.create_client("quicksight").list_topic_refresh_schedules` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/list_topic_refresh_schedules.html)

```python
# list_topic_refresh_schedules method definition

await def list_topic_refresh_schedules(
    self,
    *,
    AwsAccountId: str,
    TopicId: str,
) -> ListTopicRefreshSchedulesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTopicRefreshSchedulesResponseTypeDef](./type_defs.md#listtopicrefreshschedulesresponsetypedef) 


```python
# list_topic_refresh_schedules method usage example with argument unpacking

kwargs: ListTopicRefreshSchedulesRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "TopicId": ...,
}

parent.list_topic_refresh_schedules(**kwargs)
```

1. See [:material-code-braces: ListTopicRefreshSchedulesRequestTypeDef](./type_defs.md#listtopicrefreshschedulesrequesttypedef) 

### list\_topic\_reviewed\_answers

Lists all reviewed answers for a Q Topic.

Type annotations and code completion for `#!python session.create_client("quicksight").list_topic_reviewed_answers` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/list_topic_reviewed_answers.html)

```python
# list_topic_reviewed_answers method definition

await def list_topic_reviewed_answers(
    self,
    *,
    AwsAccountId: str,
    TopicId: str,
) -> ListTopicReviewedAnswersResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTopicReviewedAnswersResponseTypeDef](./type_defs.md#listtopicreviewedanswersresponsetypedef) 


```python
# list_topic_reviewed_answers method usage example with argument unpacking

kwargs: ListTopicReviewedAnswersRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "TopicId": ...,
}

parent.list_topic_reviewed_answers(**kwargs)
```

1. See [:material-code-braces: ListTopicReviewedAnswersRequestTypeDef](./type_defs.md#listtopicreviewedanswersrequesttypedef) 

### list\_topics

Lists all of the topics within an account.

Type annotations and code completion for `#!python session.create_client("quicksight").list_topics` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/list_topics.html)

```python
# list_topics method definition

await def list_topics(
    self,
    *,
    AwsAccountId: str,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListTopicsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTopicsResponseTypeDef](./type_defs.md#listtopicsresponsetypedef) 


```python
# list_topics method usage example with argument unpacking

kwargs: ListTopicsRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
}

parent.list_topics(**kwargs)
```

1. See [:material-code-braces: ListTopicsRequestTypeDef](./type_defs.md#listtopicsrequesttypedef) 

### list\_user\_groups

Lists the Amazon QuickSight groups that an Amazon QuickSight user is a member
of.

Type annotations and code completion for `#!python session.create_client("quicksight").list_user_groups` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/list_user_groups.html)

```python
# list_user_groups method definition

await def list_user_groups(
    self,
    *,
    UserName: str,
    AwsAccountId: str,
    Namespace: str,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListUserGroupsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListUserGroupsResponseTypeDef](./type_defs.md#listusergroupsresponsetypedef) 


```python
# list_user_groups method usage example with argument unpacking

kwargs: ListUserGroupsRequestTypeDef = {  # (1)
    "UserName": ...,
    "AwsAccountId": ...,
    "Namespace": ...,
}

parent.list_user_groups(**kwargs)
```

1. See [:material-code-braces: ListUserGroupsRequestTypeDef](./type_defs.md#listusergroupsrequesttypedef) 

### list\_users

Returns a list of all of the Amazon QuickSight users belonging to this account.

Type annotations and code completion for `#!python session.create_client("quicksight").list_users` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/list_users.html)

```python
# list_users method definition

await def list_users(
    self,
    *,
    AwsAccountId: str,
    Namespace: str,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListUsersResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListUsersResponseTypeDef](./type_defs.md#listusersresponsetypedef) 


```python
# list_users method usage example with argument unpacking

kwargs: ListUsersRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "Namespace": ...,
}

parent.list_users(**kwargs)
```

1. See [:material-code-braces: ListUsersRequestTypeDef](./type_defs.md#listusersrequesttypedef) 

### list\_vpc\_connections

Lists all of the VPC connections in the current set Amazon Web Services Region
of an Amazon Web Services account.

Type annotations and code completion for `#!python session.create_client("quicksight").list_vpc_connections` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/list_vpc_connections.html)

```python
# list_vpc_connections method definition

await def list_vpc_connections(
    self,
    *,
    AwsAccountId: str,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListVPCConnectionsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListVPCConnectionsResponseTypeDef](./type_defs.md#listvpcconnectionsresponsetypedef) 


```python
# list_vpc_connections method usage example with argument unpacking

kwargs: ListVPCConnectionsRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
}

parent.list_vpc_connections(**kwargs)
```

1. See [:material-code-braces: ListVPCConnectionsRequestTypeDef](./type_defs.md#listvpcconnectionsrequesttypedef) 

### predict\_qa\_results

Predicts existing visuals or generates new visuals to answer a given query.

Type annotations and code completion for `#!python session.create_client("quicksight").predict_qa_results` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/predict_qa_results.html)

```python
# predict_qa_results method definition

await def predict_qa_results(
    self,
    *,
    AwsAccountId: str,
    QueryText: str,
    IncludeQuickSightQIndex: IncludeQuickSightQIndexType = ...,  # (1)
    IncludeGeneratedAnswer: IncludeGeneratedAnswerType = ...,  # (2)
    MaxTopicsToConsider: int = ...,
) -> PredictQAResultsResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: IncludeQuickSightQIndexType](./literals.md#includequicksightqindextype) 
2. See [:material-code-brackets: IncludeGeneratedAnswerType](./literals.md#includegeneratedanswertype) 
3. See [:material-code-braces: PredictQAResultsResponseTypeDef](./type_defs.md#predictqaresultsresponsetypedef) 


```python
# predict_qa_results method usage example with argument unpacking

kwargs: PredictQAResultsRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "QueryText": ...,
}

parent.predict_qa_results(**kwargs)
```

1. See [:material-code-braces: PredictQAResultsRequestTypeDef](./type_defs.md#predictqaresultsrequesttypedef) 

### put\_data\_set\_refresh\_properties

Creates or updates the dataset refresh properties for the dataset.

Type annotations and code completion for `#!python session.create_client("quicksight").put_data_set_refresh_properties` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/put_data_set_refresh_properties.html)

```python
# put_data_set_refresh_properties method definition

await def put_data_set_refresh_properties(
    self,
    *,
    AwsAccountId: str,
    DataSetId: str,
    DataSetRefreshProperties: DataSetRefreshPropertiesTypeDef,  # (1)
) -> PutDataSetRefreshPropertiesResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: DataSetRefreshPropertiesTypeDef](./type_defs.md#datasetrefreshpropertiestypedef) 
2. See [:material-code-braces: PutDataSetRefreshPropertiesResponseTypeDef](./type_defs.md#putdatasetrefreshpropertiesresponsetypedef) 


```python
# put_data_set_refresh_properties method usage example with argument unpacking

kwargs: PutDataSetRefreshPropertiesRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "DataSetId": ...,
    "DataSetRefreshProperties": ...,
}

parent.put_data_set_refresh_properties(**kwargs)
```

1. See [:material-code-braces: PutDataSetRefreshPropertiesRequestTypeDef](./type_defs.md#putdatasetrefreshpropertiesrequesttypedef) 

### register\_user

Creates an Amazon QuickSight user whose identity is associated with the
Identity and Access Management (IAM) identity or role specified in the request.

Type annotations and code completion for `#!python session.create_client("quicksight").register_user` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/register_user.html)

```python
# register_user method definition

await def register_user(
    self,
    *,
    IdentityType: IdentityTypeType,  # (1)
    Email: str,
    UserRole: UserRoleType,  # (2)
    AwsAccountId: str,
    Namespace: str,
    IamArn: str = ...,
    SessionName: str = ...,
    UserName: str = ...,
    CustomPermissionsName: str = ...,
    ExternalLoginFederationProviderType: str = ...,
    CustomFederationProviderUrl: str = ...,
    ExternalLoginId: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (3)
) -> RegisterUserResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: IdentityTypeType](./literals.md#identitytypetype) 
2. See [:material-code-brackets: UserRoleType](./literals.md#userroletype) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
4. See [:material-code-braces: RegisterUserResponseTypeDef](./type_defs.md#registeruserresponsetypedef) 


```python
# register_user method usage example with argument unpacking

kwargs: RegisterUserRequestTypeDef = {  # (1)
    "IdentityType": ...,
    "Email": ...,
    "UserRole": ...,
    "AwsAccountId": ...,
    "Namespace": ...,
}

parent.register_user(**kwargs)
```

1. See [:material-code-braces: RegisterUserRequestTypeDef](./type_defs.md#registeruserrequesttypedef) 

### restore\_analysis

Restores an analysis.

Type annotations and code completion for `#!python session.create_client("quicksight").restore_analysis` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/restore_analysis.html)

```python
# restore_analysis method definition

await def restore_analysis(
    self,
    *,
    AwsAccountId: str,
    AnalysisId: str,
    RestoreToFolders: bool = ...,
) -> RestoreAnalysisResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: RestoreAnalysisResponseTypeDef](./type_defs.md#restoreanalysisresponsetypedef) 


```python
# restore_analysis method usage example with argument unpacking

kwargs: RestoreAnalysisRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "AnalysisId": ...,
}

parent.restore_analysis(**kwargs)
```

1. See [:material-code-braces: RestoreAnalysisRequestTypeDef](./type_defs.md#restoreanalysisrequesttypedef) 

### search\_analyses

Searches for analyses that belong to the user specified in the filter.

Type annotations and code completion for `#!python session.create_client("quicksight").search_analyses` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/search_analyses.html)

```python
# search_analyses method definition

await def search_analyses(
    self,
    *,
    AwsAccountId: str,
    Filters: Sequence[AnalysisSearchFilterTypeDef],  # (1)
    NextToken: str = ...,
    MaxResults: int = ...,
) -> SearchAnalysesResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: AnalysisSearchFilterTypeDef](./type_defs.md#analysissearchfiltertypedef) 
2. See [:material-code-braces: SearchAnalysesResponseTypeDef](./type_defs.md#searchanalysesresponsetypedef) 


```python
# search_analyses method usage example with argument unpacking

kwargs: SearchAnalysesRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "Filters": ...,
}

parent.search_analyses(**kwargs)
```

1. See [:material-code-braces: SearchAnalysesRequestTypeDef](./type_defs.md#searchanalysesrequesttypedef) 

### search\_dashboards

Searches for dashboards that belong to a user.

Type annotations and code completion for `#!python session.create_client("quicksight").search_dashboards` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/search_dashboards.html)

```python
# search_dashboards method definition

await def search_dashboards(
    self,
    *,
    AwsAccountId: str,
    Filters: Sequence[DashboardSearchFilterTypeDef],  # (1)
    NextToken: str = ...,
    MaxResults: int = ...,
) -> SearchDashboardsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: DashboardSearchFilterTypeDef](./type_defs.md#dashboardsearchfiltertypedef) 
2. See [:material-code-braces: SearchDashboardsResponseTypeDef](./type_defs.md#searchdashboardsresponsetypedef) 


```python
# search_dashboards method usage example with argument unpacking

kwargs: SearchDashboardsRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "Filters": ...,
}

parent.search_dashboards(**kwargs)
```

1. See [:material-code-braces: SearchDashboardsRequestTypeDef](./type_defs.md#searchdashboardsrequesttypedef) 

### search\_data\_sets

Use the <code>SearchDataSets</code> operation to search for datasets that
belong to an account.

Type annotations and code completion for `#!python session.create_client("quicksight").search_data_sets` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/search_data_sets.html)

```python
# search_data_sets method definition

await def search_data_sets(
    self,
    *,
    AwsAccountId: str,
    Filters: Sequence[DataSetSearchFilterTypeDef],  # (1)
    NextToken: str = ...,
    MaxResults: int = ...,
) -> SearchDataSetsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: DataSetSearchFilterTypeDef](./type_defs.md#datasetsearchfiltertypedef) 
2. See [:material-code-braces: SearchDataSetsResponseTypeDef](./type_defs.md#searchdatasetsresponsetypedef) 


```python
# search_data_sets method usage example with argument unpacking

kwargs: SearchDataSetsRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "Filters": ...,
}

parent.search_data_sets(**kwargs)
```

1. See [:material-code-braces: SearchDataSetsRequestTypeDef](./type_defs.md#searchdatasetsrequesttypedef) 

### search\_data\_sources

Use the <code>SearchDataSources</code> operation to search for data sources
that belong to an account.

Type annotations and code completion for `#!python session.create_client("quicksight").search_data_sources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/search_data_sources.html)

```python
# search_data_sources method definition

await def search_data_sources(
    self,
    *,
    AwsAccountId: str,
    Filters: Sequence[DataSourceSearchFilterTypeDef],  # (1)
    NextToken: str = ...,
    MaxResults: int = ...,
) -> SearchDataSourcesResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: DataSourceSearchFilterTypeDef](./type_defs.md#datasourcesearchfiltertypedef) 
2. See [:material-code-braces: SearchDataSourcesResponseTypeDef](./type_defs.md#searchdatasourcesresponsetypedef) 


```python
# search_data_sources method usage example with argument unpacking

kwargs: SearchDataSourcesRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "Filters": ...,
}

parent.search_data_sources(**kwargs)
```

1. See [:material-code-braces: SearchDataSourcesRequestTypeDef](./type_defs.md#searchdatasourcesrequesttypedef) 

### search\_folders

Searches the subfolders in a folder.

Type annotations and code completion for `#!python session.create_client("quicksight").search_folders` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/search_folders.html)

```python
# search_folders method definition

await def search_folders(
    self,
    *,
    AwsAccountId: str,
    Filters: Sequence[FolderSearchFilterTypeDef],  # (1)
    NextToken: str = ...,
    MaxResults: int = ...,
) -> SearchFoldersResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: FolderSearchFilterTypeDef](./type_defs.md#foldersearchfiltertypedef) 
2. See [:material-code-braces: SearchFoldersResponseTypeDef](./type_defs.md#searchfoldersresponsetypedef) 


```python
# search_folders method usage example with argument unpacking

kwargs: SearchFoldersRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "Filters": ...,
}

parent.search_folders(**kwargs)
```

1. See [:material-code-braces: SearchFoldersRequestTypeDef](./type_defs.md#searchfoldersrequesttypedef) 

### search\_groups

Use the <code>SearchGroups</code> operation to search groups in a specified
Amazon QuickSight namespace using the supplied filters.

Type annotations and code completion for `#!python session.create_client("quicksight").search_groups` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/search_groups.html)

```python
# search_groups method definition

await def search_groups(
    self,
    *,
    AwsAccountId: str,
    Namespace: str,
    Filters: Sequence[GroupSearchFilterTypeDef],  # (1)
    NextToken: str = ...,
    MaxResults: int = ...,
) -> SearchGroupsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: GroupSearchFilterTypeDef](./type_defs.md#groupsearchfiltertypedef) 
2. See [:material-code-braces: SearchGroupsResponseTypeDef](./type_defs.md#searchgroupsresponsetypedef) 


```python
# search_groups method usage example with argument unpacking

kwargs: SearchGroupsRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "Namespace": ...,
    "Filters": ...,
}

parent.search_groups(**kwargs)
```

1. See [:material-code-braces: SearchGroupsRequestTypeDef](./type_defs.md#searchgroupsrequesttypedef) 

### search\_topics

Searches for any Q topic that exists in an Amazon QuickSight account.

Type annotations and code completion for `#!python session.create_client("quicksight").search_topics` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/search_topics.html)

```python
# search_topics method definition

await def search_topics(
    self,
    *,
    AwsAccountId: str,
    Filters: Sequence[TopicSearchFilterTypeDef],  # (1)
    NextToken: str = ...,
    MaxResults: int = ...,
) -> SearchTopicsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TopicSearchFilterTypeDef](./type_defs.md#topicsearchfiltertypedef) 
2. See [:material-code-braces: SearchTopicsResponseTypeDef](./type_defs.md#searchtopicsresponsetypedef) 


```python
# search_topics method usage example with argument unpacking

kwargs: SearchTopicsRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "Filters": ...,
}

parent.search_topics(**kwargs)
```

1. See [:material-code-braces: SearchTopicsRequestTypeDef](./type_defs.md#searchtopicsrequesttypedef) 

### start\_asset\_bundle\_export\_job

Starts an Asset Bundle export job.

Type annotations and code completion for `#!python session.create_client("quicksight").start_asset_bundle_export_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/start_asset_bundle_export_job.html)

```python
# start_asset_bundle_export_job method definition

await def start_asset_bundle_export_job(
    self,
    *,
    AwsAccountId: str,
    AssetBundleExportJobId: str,
    ResourceArns: Sequence[str],
    ExportFormat: AssetBundleExportFormatType,  # (1)
    IncludeAllDependencies: bool = ...,
    CloudFormationOverridePropertyConfiguration: AssetBundleCloudFormationOverridePropertyConfigurationUnionTypeDef = ...,  # (2)
    IncludePermissions: bool = ...,
    IncludeTags: bool = ...,
    ValidationStrategy: AssetBundleExportJobValidationStrategyTypeDef = ...,  # (3)
    IncludeFolderMemberships: bool = ...,
    IncludeFolderMembers: IncludeFolderMembersType = ...,  # (4)
) -> StartAssetBundleExportJobResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-brackets: AssetBundleExportFormatType](./literals.md#assetbundleexportformattype) 
2. See [:material-code-braces: AssetBundleCloudFormationOverridePropertyConfigurationTypeDef](./type_defs.md#assetbundlecloudformationoverridepropertyconfigurationtypedef) [:material-code-braces: AssetBundleCloudFormationOverridePropertyConfigurationOutputTypeDef](./type_defs.md#assetbundlecloudformationoverridepropertyconfigurationoutputtypedef) 
3. See [:material-code-braces: AssetBundleExportJobValidationStrategyTypeDef](./type_defs.md#assetbundleexportjobvalidationstrategytypedef) 
4. See [:material-code-brackets: IncludeFolderMembersType](./literals.md#includefoldermemberstype) 
5. See [:material-code-braces: StartAssetBundleExportJobResponseTypeDef](./type_defs.md#startassetbundleexportjobresponsetypedef) 


```python
# start_asset_bundle_export_job method usage example with argument unpacking

kwargs: StartAssetBundleExportJobRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "AssetBundleExportJobId": ...,
    "ResourceArns": ...,
    "ExportFormat": ...,
}

parent.start_asset_bundle_export_job(**kwargs)
```

1. See [:material-code-braces: StartAssetBundleExportJobRequestTypeDef](./type_defs.md#startassetbundleexportjobrequesttypedef) 

### start\_asset\_bundle\_import\_job

Starts an Asset Bundle import job.

Type annotations and code completion for `#!python session.create_client("quicksight").start_asset_bundle_import_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/start_asset_bundle_import_job.html)

```python
# start_asset_bundle_import_job method definition

await def start_asset_bundle_import_job(
    self,
    *,
    AwsAccountId: str,
    AssetBundleImportJobId: str,
    AssetBundleImportSource: AssetBundleImportSourceTypeDef,  # (1)
    OverrideParameters: AssetBundleImportJobOverrideParametersUnionTypeDef = ...,  # (2)
    FailureAction: AssetBundleImportFailureActionType = ...,  # (3)
    OverridePermissions: AssetBundleImportJobOverridePermissionsUnionTypeDef = ...,  # (4)
    OverrideTags: AssetBundleImportJobOverrideTagsUnionTypeDef = ...,  # (5)
    OverrideValidationStrategy: AssetBundleImportJobOverrideValidationStrategyTypeDef = ...,  # (6)
) -> StartAssetBundleImportJobResponseTypeDef:  # (7)
    ...
```

1. See [:material-code-braces: AssetBundleImportSourceTypeDef](./type_defs.md#assetbundleimportsourcetypedef) 
2. See [:material-code-braces: AssetBundleImportJobOverrideParametersTypeDef](./type_defs.md#assetbundleimportjoboverrideparameterstypedef) [:material-code-braces: AssetBundleImportJobOverrideParametersOutputTypeDef](./type_defs.md#assetbundleimportjoboverrideparametersoutputtypedef) 
3. See [:material-code-brackets: AssetBundleImportFailureActionType](./literals.md#assetbundleimportfailureactiontype) 
4. See [:material-code-braces: AssetBundleImportJobOverridePermissionsTypeDef](./type_defs.md#assetbundleimportjoboverridepermissionstypedef) [:material-code-braces: AssetBundleImportJobOverridePermissionsOutputTypeDef](./type_defs.md#assetbundleimportjoboverridepermissionsoutputtypedef) 
5. See [:material-code-braces: AssetBundleImportJobOverrideTagsTypeDef](./type_defs.md#assetbundleimportjoboverridetagstypedef) [:material-code-braces: AssetBundleImportJobOverrideTagsOutputTypeDef](./type_defs.md#assetbundleimportjoboverridetagsoutputtypedef) 
6. See [:material-code-braces: AssetBundleImportJobOverrideValidationStrategyTypeDef](./type_defs.md#assetbundleimportjoboverridevalidationstrategytypedef) 
7. See [:material-code-braces: StartAssetBundleImportJobResponseTypeDef](./type_defs.md#startassetbundleimportjobresponsetypedef) 


```python
# start_asset_bundle_import_job method usage example with argument unpacking

kwargs: StartAssetBundleImportJobRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "AssetBundleImportJobId": ...,
    "AssetBundleImportSource": ...,
}

parent.start_asset_bundle_import_job(**kwargs)
```

1. See [:material-code-braces: StartAssetBundleImportJobRequestTypeDef](./type_defs.md#startassetbundleimportjobrequesttypedef) 

### start\_dashboard\_snapshot\_job

Starts an asynchronous job that generates a snapshot of a dashboard's output.

Type annotations and code completion for `#!python session.create_client("quicksight").start_dashboard_snapshot_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/start_dashboard_snapshot_job.html)

```python
# start_dashboard_snapshot_job method definition

await def start_dashboard_snapshot_job(
    self,
    *,
    AwsAccountId: str,
    DashboardId: str,
    SnapshotJobId: str,
    UserConfiguration: SnapshotUserConfigurationTypeDef,  # (1)
    SnapshotConfiguration: SnapshotConfigurationUnionTypeDef,  # (2)
) -> StartDashboardSnapshotJobResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: SnapshotUserConfigurationTypeDef](./type_defs.md#snapshotuserconfigurationtypedef) 
2. See [:material-code-braces: SnapshotConfigurationTypeDef](./type_defs.md#snapshotconfigurationtypedef) [:material-code-braces: SnapshotConfigurationOutputTypeDef](./type_defs.md#snapshotconfigurationoutputtypedef) 
3. See [:material-code-braces: StartDashboardSnapshotJobResponseTypeDef](./type_defs.md#startdashboardsnapshotjobresponsetypedef) 


```python
# start_dashboard_snapshot_job method usage example with argument unpacking

kwargs: StartDashboardSnapshotJobRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "DashboardId": ...,
    "SnapshotJobId": ...,
    "UserConfiguration": ...,
    "SnapshotConfiguration": ...,
}

parent.start_dashboard_snapshot_job(**kwargs)
```

1. See [:material-code-braces: StartDashboardSnapshotJobRequestTypeDef](./type_defs.md#startdashboardsnapshotjobrequesttypedef) 

### start\_dashboard\_snapshot\_job\_schedule

Starts an asynchronous job that runs an existing dashboard schedule and sends
the dashboard snapshot through email.

Type annotations and code completion for `#!python session.create_client("quicksight").start_dashboard_snapshot_job_schedule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/start_dashboard_snapshot_job_schedule.html)

```python
# start_dashboard_snapshot_job_schedule method definition

await def start_dashboard_snapshot_job_schedule(
    self,
    *,
    AwsAccountId: str,
    DashboardId: str,
    ScheduleId: str,
) -> StartDashboardSnapshotJobScheduleResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StartDashboardSnapshotJobScheduleResponseTypeDef](./type_defs.md#startdashboardsnapshotjobscheduleresponsetypedef) 


```python
# start_dashboard_snapshot_job_schedule method usage example with argument unpacking

kwargs: StartDashboardSnapshotJobScheduleRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "DashboardId": ...,
    "ScheduleId": ...,
}

parent.start_dashboard_snapshot_job_schedule(**kwargs)
```

1. See [:material-code-braces: StartDashboardSnapshotJobScheduleRequestTypeDef](./type_defs.md#startdashboardsnapshotjobschedulerequesttypedef) 

### tag\_resource

Assigns one or more tags (key-value pairs) to the specified Amazon QuickSight
resource.

Type annotations and code completion for `#!python session.create_client("quicksight").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/tag_resource.html)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    ResourceArn: str,
    Tags: Sequence[TagTypeDef],  # (1)
) -> TagResourceResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: TagResourceResponseTypeDef](./type_defs.md#tagresourceresponsetypedef) 


```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceRequestTypeDef = {  # (1)
    "ResourceArn": ...,
    "Tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestTypeDef](./type_defs.md#tagresourcerequesttypedef) 

### untag\_resource

Removes a tag or tags from a resource.

Type annotations and code completion for `#!python session.create_client("quicksight").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/untag_resource.html)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    ResourceArn: str,
    TagKeys: Sequence[str],
) -> UntagResourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UntagResourceResponseTypeDef](./type_defs.md#untagresourceresponsetypedef) 


```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceRequestTypeDef = {  # (1)
    "ResourceArn": ...,
    "TagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestTypeDef](./type_defs.md#untagresourcerequesttypedef) 

### update\_account\_customization

Updates Amazon QuickSight customizations for the current Amazon Web Services
Region.

Type annotations and code completion for `#!python session.create_client("quicksight").update_account_customization` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/update_account_customization.html)

```python
# update_account_customization method definition

await def update_account_customization(
    self,
    *,
    AwsAccountId: str,
    AccountCustomization: AccountCustomizationTypeDef,  # (1)
    Namespace: str = ...,
) -> UpdateAccountCustomizationResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: AccountCustomizationTypeDef](./type_defs.md#accountcustomizationtypedef) 
2. See [:material-code-braces: UpdateAccountCustomizationResponseTypeDef](./type_defs.md#updateaccountcustomizationresponsetypedef) 


```python
# update_account_customization method usage example with argument unpacking

kwargs: UpdateAccountCustomizationRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "AccountCustomization": ...,
}

parent.update_account_customization(**kwargs)
```

1. See [:material-code-braces: UpdateAccountCustomizationRequestTypeDef](./type_defs.md#updateaccountcustomizationrequesttypedef) 

### update\_account\_settings

Updates the Amazon QuickSight settings in your Amazon Web Services account.

Type annotations and code completion for `#!python session.create_client("quicksight").update_account_settings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/update_account_settings.html)

```python
# update_account_settings method definition

await def update_account_settings(
    self,
    *,
    AwsAccountId: str,
    DefaultNamespace: str,
    NotificationEmail: str = ...,
    TerminationProtectionEnabled: bool = ...,
) -> UpdateAccountSettingsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateAccountSettingsResponseTypeDef](./type_defs.md#updateaccountsettingsresponsetypedef) 


```python
# update_account_settings method usage example with argument unpacking

kwargs: UpdateAccountSettingsRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "DefaultNamespace": ...,
}

parent.update_account_settings(**kwargs)
```

1. See [:material-code-braces: UpdateAccountSettingsRequestTypeDef](./type_defs.md#updateaccountsettingsrequesttypedef) 

### update\_analysis

Updates an analysis in Amazon QuickSight.

Type annotations and code completion for `#!python session.create_client("quicksight").update_analysis` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/update_analysis.html)

```python
# update_analysis method definition

await def update_analysis(
    self,
    *,
    AwsAccountId: str,
    AnalysisId: str,
    Name: str,
    Parameters: ParametersUnionTypeDef = ...,  # (1)
    SourceEntity: AnalysisSourceEntityTypeDef = ...,  # (2)
    ThemeArn: str = ...,
    Definition: AnalysisDefinitionUnionTypeDef = ...,  # (3)
    ValidationStrategy: ValidationStrategyTypeDef = ...,  # (4)
) -> UpdateAnalysisResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-braces: ParametersTypeDef](./type_defs.md#parameterstypedef) [:material-code-braces: ParametersOutputTypeDef](./type_defs.md#parametersoutputtypedef) 
2. See [:material-code-braces: AnalysisSourceEntityTypeDef](./type_defs.md#analysissourceentitytypedef) 
3. See [:material-code-braces: AnalysisDefinitionTypeDef](./type_defs.md#analysisdefinitiontypedef) [:material-code-braces: AnalysisDefinitionOutputTypeDef](./type_defs.md#analysisdefinitionoutputtypedef) 
4. See [:material-code-braces: ValidationStrategyTypeDef](./type_defs.md#validationstrategytypedef) 
5. See [:material-code-braces: UpdateAnalysisResponseTypeDef](./type_defs.md#updateanalysisresponsetypedef) 


```python
# update_analysis method usage example with argument unpacking

kwargs: UpdateAnalysisRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "AnalysisId": ...,
    "Name": ...,
}

parent.update_analysis(**kwargs)
```

1. See [:material-code-braces: UpdateAnalysisRequestTypeDef](./type_defs.md#updateanalysisrequesttypedef) 

### update\_analysis\_permissions

Updates the read and write permissions for an analysis.

Type annotations and code completion for `#!python session.create_client("quicksight").update_analysis_permissions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/update_analysis_permissions.html)

```python
# update_analysis_permissions method definition

await def update_analysis_permissions(
    self,
    *,
    AwsAccountId: str,
    AnalysisId: str,
    GrantPermissions: Sequence[ResourcePermissionUnionTypeDef] = ...,  # (1)
    RevokePermissions: Sequence[ResourcePermissionUnionTypeDef] = ...,  # (1)
) -> UpdateAnalysisPermissionsResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: ResourcePermissionTypeDef](./type_defs.md#resourcepermissiontypedef) [:material-code-braces: ResourcePermissionOutputTypeDef](./type_defs.md#resourcepermissionoutputtypedef) 
2. See [:material-code-braces: ResourcePermissionTypeDef](./type_defs.md#resourcepermissiontypedef) [:material-code-braces: ResourcePermissionOutputTypeDef](./type_defs.md#resourcepermissionoutputtypedef) 
3. See [:material-code-braces: UpdateAnalysisPermissionsResponseTypeDef](./type_defs.md#updateanalysispermissionsresponsetypedef) 


```python
# update_analysis_permissions method usage example with argument unpacking

kwargs: UpdateAnalysisPermissionsRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "AnalysisId": ...,
}

parent.update_analysis_permissions(**kwargs)
```

1. See [:material-code-braces: UpdateAnalysisPermissionsRequestTypeDef](./type_defs.md#updateanalysispermissionsrequesttypedef) 

### update\_application\_with\_token\_exchange\_grant

Updates an Amazon QuickSight application with a token exchange grant.

Type annotations and code completion for `#!python session.create_client("quicksight").update_application_with_token_exchange_grant` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/update_application_with_token_exchange_grant.html)

```python
# update_application_with_token_exchange_grant method definition

await def update_application_with_token_exchange_grant(
    self,
    *,
    AwsAccountId: str,
    Namespace: str,
) -> UpdateApplicationWithTokenExchangeGrantResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateApplicationWithTokenExchangeGrantResponseTypeDef](./type_defs.md#updateapplicationwithtokenexchangegrantresponsetypedef) 


```python
# update_application_with_token_exchange_grant method usage example with argument unpacking

kwargs: UpdateApplicationWithTokenExchangeGrantRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "Namespace": ...,
}

parent.update_application_with_token_exchange_grant(**kwargs)
```

1. See [:material-code-braces: UpdateApplicationWithTokenExchangeGrantRequestTypeDef](./type_defs.md#updateapplicationwithtokenexchangegrantrequesttypedef) 

### update\_brand

Updates a brand.

Type annotations and code completion for `#!python session.create_client("quicksight").update_brand` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/update_brand.html)

```python
# update_brand method definition

await def update_brand(
    self,
    *,
    AwsAccountId: str,
    BrandId: str,
    BrandDefinition: BrandDefinitionTypeDef = ...,  # (1)
) -> UpdateBrandResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: BrandDefinitionTypeDef](./type_defs.md#branddefinitiontypedef) 
2. See [:material-code-braces: UpdateBrandResponseTypeDef](./type_defs.md#updatebrandresponsetypedef) 


```python
# update_brand method usage example with argument unpacking

kwargs: UpdateBrandRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "BrandId": ...,
}

parent.update_brand(**kwargs)
```

1. See [:material-code-braces: UpdateBrandRequestTypeDef](./type_defs.md#updatebrandrequesttypedef) 

### update\_brand\_assignment

Updates a brand assignment.

Type annotations and code completion for `#!python session.create_client("quicksight").update_brand_assignment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/update_brand_assignment.html)

```python
# update_brand_assignment method definition

await def update_brand_assignment(
    self,
    *,
    AwsAccountId: str,
    BrandArn: str,
) -> UpdateBrandAssignmentResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateBrandAssignmentResponseTypeDef](./type_defs.md#updatebrandassignmentresponsetypedef) 


```python
# update_brand_assignment method usage example with argument unpacking

kwargs: UpdateBrandAssignmentRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "BrandArn": ...,
}

parent.update_brand_assignment(**kwargs)
```

1. See [:material-code-braces: UpdateBrandAssignmentRequestTypeDef](./type_defs.md#updatebrandassignmentrequesttypedef) 

### update\_brand\_published\_version

Updates the published version of a brand.

Type annotations and code completion for `#!python session.create_client("quicksight").update_brand_published_version` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/update_brand_published_version.html)

```python
# update_brand_published_version method definition

await def update_brand_published_version(
    self,
    *,
    AwsAccountId: str,
    BrandId: str,
    VersionId: str,
) -> UpdateBrandPublishedVersionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateBrandPublishedVersionResponseTypeDef](./type_defs.md#updatebrandpublishedversionresponsetypedef) 


```python
# update_brand_published_version method usage example with argument unpacking

kwargs: UpdateBrandPublishedVersionRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "BrandId": ...,
    "VersionId": ...,
}

parent.update_brand_published_version(**kwargs)
```

1. See [:material-code-braces: UpdateBrandPublishedVersionRequestTypeDef](./type_defs.md#updatebrandpublishedversionrequesttypedef) 

### update\_custom\_permissions

Updates a custom permissions profile.

Type annotations and code completion for `#!python session.create_client("quicksight").update_custom_permissions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/update_custom_permissions.html)

```python
# update_custom_permissions method definition

await def update_custom_permissions(
    self,
    *,
    AwsAccountId: str,
    CustomPermissionsName: str,
    Capabilities: CapabilitiesTypeDef = ...,  # (1)
) -> UpdateCustomPermissionsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: CapabilitiesTypeDef](./type_defs.md#capabilitiestypedef) 
2. See [:material-code-braces: UpdateCustomPermissionsResponseTypeDef](./type_defs.md#updatecustompermissionsresponsetypedef) 


```python
# update_custom_permissions method usage example with argument unpacking

kwargs: UpdateCustomPermissionsRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "CustomPermissionsName": ...,
}

parent.update_custom_permissions(**kwargs)
```

1. See [:material-code-braces: UpdateCustomPermissionsRequestTypeDef](./type_defs.md#updatecustompermissionsrequesttypedef) 

### update\_dashboard

Updates a dashboard in an Amazon Web Services account.

Type annotations and code completion for `#!python session.create_client("quicksight").update_dashboard` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/update_dashboard.html)

```python
# update_dashboard method definition

await def update_dashboard(
    self,
    *,
    AwsAccountId: str,
    DashboardId: str,
    Name: str,
    SourceEntity: DashboardSourceEntityTypeDef = ...,  # (1)
    Parameters: ParametersUnionTypeDef = ...,  # (2)
    VersionDescription: str = ...,
    DashboardPublishOptions: DashboardPublishOptionsTypeDef = ...,  # (3)
    ThemeArn: str = ...,
    Definition: DashboardVersionDefinitionUnionTypeDef = ...,  # (4)
    ValidationStrategy: ValidationStrategyTypeDef = ...,  # (5)
) -> UpdateDashboardResponseTypeDef:  # (6)
    ...
```

1. See [:material-code-braces: DashboardSourceEntityTypeDef](./type_defs.md#dashboardsourceentitytypedef) 
2. See [:material-code-braces: ParametersTypeDef](./type_defs.md#parameterstypedef) [:material-code-braces: ParametersOutputTypeDef](./type_defs.md#parametersoutputtypedef) 
3. See [:material-code-braces: DashboardPublishOptionsTypeDef](./type_defs.md#dashboardpublishoptionstypedef) 
4. See [:material-code-braces: DashboardVersionDefinitionTypeDef](./type_defs.md#dashboardversiondefinitiontypedef) [:material-code-braces: DashboardVersionDefinitionOutputTypeDef](./type_defs.md#dashboardversiondefinitionoutputtypedef) 
5. See [:material-code-braces: ValidationStrategyTypeDef](./type_defs.md#validationstrategytypedef) 
6. See [:material-code-braces: UpdateDashboardResponseTypeDef](./type_defs.md#updatedashboardresponsetypedef) 


```python
# update_dashboard method usage example with argument unpacking

kwargs: UpdateDashboardRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "DashboardId": ...,
    "Name": ...,
}

parent.update_dashboard(**kwargs)
```

1. See [:material-code-braces: UpdateDashboardRequestTypeDef](./type_defs.md#updatedashboardrequesttypedef) 

### update\_dashboard\_links

Updates the linked analyses on a dashboard.

Type annotations and code completion for `#!python session.create_client("quicksight").update_dashboard_links` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/update_dashboard_links.html)

```python
# update_dashboard_links method definition

await def update_dashboard_links(
    self,
    *,
    AwsAccountId: str,
    DashboardId: str,
    LinkEntities: Sequence[str],
) -> UpdateDashboardLinksResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateDashboardLinksResponseTypeDef](./type_defs.md#updatedashboardlinksresponsetypedef) 


```python
# update_dashboard_links method usage example with argument unpacking

kwargs: UpdateDashboardLinksRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "DashboardId": ...,
    "LinkEntities": ...,
}

parent.update_dashboard_links(**kwargs)
```

1. See [:material-code-braces: UpdateDashboardLinksRequestTypeDef](./type_defs.md#updatedashboardlinksrequesttypedef) 

### update\_dashboard\_permissions

Updates read and write permissions on a dashboard.

Type annotations and code completion for `#!python session.create_client("quicksight").update_dashboard_permissions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/update_dashboard_permissions.html)

```python
# update_dashboard_permissions method definition

await def update_dashboard_permissions(
    self,
    *,
    AwsAccountId: str,
    DashboardId: str,
    GrantPermissions: Sequence[ResourcePermissionUnionTypeDef] = ...,  # (1)
    RevokePermissions: Sequence[ResourcePermissionUnionTypeDef] = ...,  # (1)
    GrantLinkPermissions: Sequence[ResourcePermissionUnionTypeDef] = ...,  # (1)
    RevokeLinkPermissions: Sequence[ResourcePermissionUnionTypeDef] = ...,  # (1)
) -> UpdateDashboardPermissionsResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-braces: ResourcePermissionTypeDef](./type_defs.md#resourcepermissiontypedef) [:material-code-braces: ResourcePermissionOutputTypeDef](./type_defs.md#resourcepermissionoutputtypedef) 
2. See [:material-code-braces: ResourcePermissionTypeDef](./type_defs.md#resourcepermissiontypedef) [:material-code-braces: ResourcePermissionOutputTypeDef](./type_defs.md#resourcepermissionoutputtypedef) 
3. See [:material-code-braces: ResourcePermissionTypeDef](./type_defs.md#resourcepermissiontypedef) [:material-code-braces: ResourcePermissionOutputTypeDef](./type_defs.md#resourcepermissionoutputtypedef) 
4. See [:material-code-braces: ResourcePermissionTypeDef](./type_defs.md#resourcepermissiontypedef) [:material-code-braces: ResourcePermissionOutputTypeDef](./type_defs.md#resourcepermissionoutputtypedef) 
5. See [:material-code-braces: UpdateDashboardPermissionsResponseTypeDef](./type_defs.md#updatedashboardpermissionsresponsetypedef) 


```python
# update_dashboard_permissions method usage example with argument unpacking

kwargs: UpdateDashboardPermissionsRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "DashboardId": ...,
}

parent.update_dashboard_permissions(**kwargs)
```

1. See [:material-code-braces: UpdateDashboardPermissionsRequestTypeDef](./type_defs.md#updatedashboardpermissionsrequesttypedef) 

### update\_dashboard\_published\_version

Updates the published version of a dashboard.

Type annotations and code completion for `#!python session.create_client("quicksight").update_dashboard_published_version` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/update_dashboard_published_version.html)

```python
# update_dashboard_published_version method definition

await def update_dashboard_published_version(
    self,
    *,
    AwsAccountId: str,
    DashboardId: str,
    VersionNumber: int,
) -> UpdateDashboardPublishedVersionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateDashboardPublishedVersionResponseTypeDef](./type_defs.md#updatedashboardpublishedversionresponsetypedef) 


```python
# update_dashboard_published_version method usage example with argument unpacking

kwargs: UpdateDashboardPublishedVersionRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "DashboardId": ...,
    "VersionNumber": ...,
}

parent.update_dashboard_published_version(**kwargs)
```

1. See [:material-code-braces: UpdateDashboardPublishedVersionRequestTypeDef](./type_defs.md#updatedashboardpublishedversionrequesttypedef) 

### update\_dashboards\_qa\_configuration

Updates a Dashboard QA configuration.

Type annotations and code completion for `#!python session.create_client("quicksight").update_dashboards_qa_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/update_dashboards_qa_configuration.html)

```python
# update_dashboards_qa_configuration method definition

await def update_dashboards_qa_configuration(
    self,
    *,
    AwsAccountId: str,
    DashboardsQAStatus: DashboardsQAStatusType,  # (1)
) -> UpdateDashboardsQAConfigurationResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: DashboardsQAStatusType](./literals.md#dashboardsqastatustype) 
2. See [:material-code-braces: UpdateDashboardsQAConfigurationResponseTypeDef](./type_defs.md#updatedashboardsqaconfigurationresponsetypedef) 


```python
# update_dashboards_qa_configuration method usage example with argument unpacking

kwargs: UpdateDashboardsQAConfigurationRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "DashboardsQAStatus": ...,
}

parent.update_dashboards_qa_configuration(**kwargs)
```

1. See [:material-code-braces: UpdateDashboardsQAConfigurationRequestTypeDef](./type_defs.md#updatedashboardsqaconfigurationrequesttypedef) 

### update\_data\_set

Updates a dataset.

Type annotations and code completion for `#!python session.create_client("quicksight").update_data_set` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/update_data_set.html)

```python
# update_data_set method definition

await def update_data_set(
    self,
    *,
    AwsAccountId: str,
    DataSetId: str,
    Name: str,
    PhysicalTableMap: Mapping[str, PhysicalTableUnionTypeDef],  # (1)
    ImportMode: DataSetImportModeType,  # (2)
    LogicalTableMap: Mapping[str, LogicalTableUnionTypeDef] = ...,  # (3)
    ColumnGroups: Sequence[ColumnGroupUnionTypeDef] = ...,  # (4)
    FieldFolders: Mapping[str, FieldFolderUnionTypeDef] = ...,  # (5)
    RowLevelPermissionDataSet: RowLevelPermissionDataSetTypeDef = ...,  # (6)
    RowLevelPermissionTagConfiguration: RowLevelPermissionTagConfigurationUnionTypeDef = ...,  # (7)
    ColumnLevelPermissionRules: Sequence[ColumnLevelPermissionRuleUnionTypeDef] = ...,  # (8)
    DataSetUsageConfiguration: DataSetUsageConfigurationTypeDef = ...,  # (9)
    DatasetParameters: Sequence[DatasetParameterUnionTypeDef] = ...,  # (10)
    PerformanceConfiguration: PerformanceConfigurationUnionTypeDef = ...,  # (11)
) -> UpdateDataSetResponseTypeDef:  # (12)
    ...
```

1. See [:material-code-braces: PhysicalTableTypeDef](./type_defs.md#physicaltabletypedef) [:material-code-braces: PhysicalTableOutputTypeDef](./type_defs.md#physicaltableoutputtypedef) 
2. See [:material-code-brackets: DataSetImportModeType](./literals.md#datasetimportmodetype) 
3. See [:material-code-braces: LogicalTableTypeDef](./type_defs.md#logicaltabletypedef) [:material-code-braces: LogicalTableOutputTypeDef](./type_defs.md#logicaltableoutputtypedef) 
4. See [:material-code-braces: ColumnGroupTypeDef](./type_defs.md#columngrouptypedef) [:material-code-braces: ColumnGroupOutputTypeDef](./type_defs.md#columngroupoutputtypedef) 
5. See [:material-code-braces: FieldFolderTypeDef](./type_defs.md#fieldfoldertypedef) [:material-code-braces: FieldFolderOutputTypeDef](./type_defs.md#fieldfolderoutputtypedef) 
6. See [:material-code-braces: RowLevelPermissionDataSetTypeDef](./type_defs.md#rowlevelpermissiondatasettypedef) 
7. See [:material-code-braces: RowLevelPermissionTagConfigurationTypeDef](./type_defs.md#rowlevelpermissiontagconfigurationtypedef) [:material-code-braces: RowLevelPermissionTagConfigurationOutputTypeDef](./type_defs.md#rowlevelpermissiontagconfigurationoutputtypedef) 
8. See [:material-code-braces: ColumnLevelPermissionRuleTypeDef](./type_defs.md#columnlevelpermissionruletypedef) [:material-code-braces: ColumnLevelPermissionRuleOutputTypeDef](./type_defs.md#columnlevelpermissionruleoutputtypedef) 
9. See [:material-code-braces: DataSetUsageConfigurationTypeDef](./type_defs.md#datasetusageconfigurationtypedef) 
10. See [:material-code-braces: DatasetParameterTypeDef](./type_defs.md#datasetparametertypedef) [:material-code-braces: DatasetParameterOutputTypeDef](./type_defs.md#datasetparameteroutputtypedef) 
11. See [:material-code-braces: PerformanceConfigurationTypeDef](./type_defs.md#performanceconfigurationtypedef) [:material-code-braces: PerformanceConfigurationOutputTypeDef](./type_defs.md#performanceconfigurationoutputtypedef) 
12. See [:material-code-braces: UpdateDataSetResponseTypeDef](./type_defs.md#updatedatasetresponsetypedef) 


```python
# update_data_set method usage example with argument unpacking

kwargs: UpdateDataSetRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "DataSetId": ...,
    "Name": ...,
    "PhysicalTableMap": ...,
    "ImportMode": ...,
}

parent.update_data_set(**kwargs)
```

1. See [:material-code-braces: UpdateDataSetRequestTypeDef](./type_defs.md#updatedatasetrequesttypedef) 

### update\_data\_set\_permissions

Updates the permissions on a dataset.

Type annotations and code completion for `#!python session.create_client("quicksight").update_data_set_permissions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/update_data_set_permissions.html)

```python
# update_data_set_permissions method definition

await def update_data_set_permissions(
    self,
    *,
    AwsAccountId: str,
    DataSetId: str,
    GrantPermissions: Sequence[ResourcePermissionUnionTypeDef] = ...,  # (1)
    RevokePermissions: Sequence[ResourcePermissionUnionTypeDef] = ...,  # (1)
) -> UpdateDataSetPermissionsResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: ResourcePermissionTypeDef](./type_defs.md#resourcepermissiontypedef) [:material-code-braces: ResourcePermissionOutputTypeDef](./type_defs.md#resourcepermissionoutputtypedef) 
2. See [:material-code-braces: ResourcePermissionTypeDef](./type_defs.md#resourcepermissiontypedef) [:material-code-braces: ResourcePermissionOutputTypeDef](./type_defs.md#resourcepermissionoutputtypedef) 
3. See [:material-code-braces: UpdateDataSetPermissionsResponseTypeDef](./type_defs.md#updatedatasetpermissionsresponsetypedef) 


```python
# update_data_set_permissions method usage example with argument unpacking

kwargs: UpdateDataSetPermissionsRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "DataSetId": ...,
}

parent.update_data_set_permissions(**kwargs)
```

1. See [:material-code-braces: UpdateDataSetPermissionsRequestTypeDef](./type_defs.md#updatedatasetpermissionsrequesttypedef) 

### update\_data\_source

Updates a data source.

Type annotations and code completion for `#!python session.create_client("quicksight").update_data_source` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/update_data_source.html)

```python
# update_data_source method definition

await def update_data_source(
    self,
    *,
    AwsAccountId: str,
    DataSourceId: str,
    Name: str,
    DataSourceParameters: DataSourceParametersUnionTypeDef = ...,  # (1)
    Credentials: DataSourceCredentialsTypeDef = ...,  # (2)
    VpcConnectionProperties: VpcConnectionPropertiesTypeDef = ...,  # (3)
    SslProperties: SslPropertiesTypeDef = ...,  # (4)
) -> UpdateDataSourceResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-braces: DataSourceParametersTypeDef](./type_defs.md#datasourceparameterstypedef) [:material-code-braces: DataSourceParametersOutputTypeDef](./type_defs.md#datasourceparametersoutputtypedef) 
2. See [:material-code-braces: DataSourceCredentialsTypeDef](./type_defs.md#datasourcecredentialstypedef) 
3. See [:material-code-braces: VpcConnectionPropertiesTypeDef](./type_defs.md#vpcconnectionpropertiestypedef) 
4. See [:material-code-braces: SslPropertiesTypeDef](./type_defs.md#sslpropertiestypedef) 
5. See [:material-code-braces: UpdateDataSourceResponseTypeDef](./type_defs.md#updatedatasourceresponsetypedef) 


```python
# update_data_source method usage example with argument unpacking

kwargs: UpdateDataSourceRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "DataSourceId": ...,
    "Name": ...,
}

parent.update_data_source(**kwargs)
```

1. See [:material-code-braces: UpdateDataSourceRequestTypeDef](./type_defs.md#updatedatasourcerequesttypedef) 

### update\_data\_source\_permissions

Updates the permissions to a data source.

Type annotations and code completion for `#!python session.create_client("quicksight").update_data_source_permissions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/update_data_source_permissions.html)

```python
# update_data_source_permissions method definition

await def update_data_source_permissions(
    self,
    *,
    AwsAccountId: str,
    DataSourceId: str,
    GrantPermissions: Sequence[ResourcePermissionUnionTypeDef] = ...,  # (1)
    RevokePermissions: Sequence[ResourcePermissionUnionTypeDef] = ...,  # (1)
) -> UpdateDataSourcePermissionsResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: ResourcePermissionTypeDef](./type_defs.md#resourcepermissiontypedef) [:material-code-braces: ResourcePermissionOutputTypeDef](./type_defs.md#resourcepermissionoutputtypedef) 
2. See [:material-code-braces: ResourcePermissionTypeDef](./type_defs.md#resourcepermissiontypedef) [:material-code-braces: ResourcePermissionOutputTypeDef](./type_defs.md#resourcepermissionoutputtypedef) 
3. See [:material-code-braces: UpdateDataSourcePermissionsResponseTypeDef](./type_defs.md#updatedatasourcepermissionsresponsetypedef) 


```python
# update_data_source_permissions method usage example with argument unpacking

kwargs: UpdateDataSourcePermissionsRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "DataSourceId": ...,
}

parent.update_data_source_permissions(**kwargs)
```

1. See [:material-code-braces: UpdateDataSourcePermissionsRequestTypeDef](./type_defs.md#updatedatasourcepermissionsrequesttypedef) 

### update\_default\_q\_business\_application

Updates a Amazon Q Business application that is linked to a Amazon QuickSight
account.

Type annotations and code completion for `#!python session.create_client("quicksight").update_default_q_business_application` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/update_default_q_business_application.html)

```python
# update_default_q_business_application method definition

await def update_default_q_business_application(
    self,
    *,
    AwsAccountId: str,
    ApplicationId: str,
    Namespace: str = ...,
) -> UpdateDefaultQBusinessApplicationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateDefaultQBusinessApplicationResponseTypeDef](./type_defs.md#updatedefaultqbusinessapplicationresponsetypedef) 


```python
# update_default_q_business_application method usage example with argument unpacking

kwargs: UpdateDefaultQBusinessApplicationRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "ApplicationId": ...,
}

parent.update_default_q_business_application(**kwargs)
```

1. See [:material-code-braces: UpdateDefaultQBusinessApplicationRequestTypeDef](./type_defs.md#updatedefaultqbusinessapplicationrequesttypedef) 

### update\_folder

Updates the name of a folder.

Type annotations and code completion for `#!python session.create_client("quicksight").update_folder` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/update_folder.html)

```python
# update_folder method definition

await def update_folder(
    self,
    *,
    AwsAccountId: str,
    FolderId: str,
    Name: str,
) -> UpdateFolderResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateFolderResponseTypeDef](./type_defs.md#updatefolderresponsetypedef) 


```python
# update_folder method usage example with argument unpacking

kwargs: UpdateFolderRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "FolderId": ...,
    "Name": ...,
}

parent.update_folder(**kwargs)
```

1. See [:material-code-braces: UpdateFolderRequestTypeDef](./type_defs.md#updatefolderrequesttypedef) 

### update\_folder\_permissions

Updates permissions of a folder.

Type annotations and code completion for `#!python session.create_client("quicksight").update_folder_permissions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/update_folder_permissions.html)

```python
# update_folder_permissions method definition

await def update_folder_permissions(
    self,
    *,
    AwsAccountId: str,
    FolderId: str,
    GrantPermissions: Sequence[ResourcePermissionUnionTypeDef] = ...,  # (1)
    RevokePermissions: Sequence[ResourcePermissionUnionTypeDef] = ...,  # (1)
) -> UpdateFolderPermissionsResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: ResourcePermissionTypeDef](./type_defs.md#resourcepermissiontypedef) [:material-code-braces: ResourcePermissionOutputTypeDef](./type_defs.md#resourcepermissionoutputtypedef) 
2. See [:material-code-braces: ResourcePermissionTypeDef](./type_defs.md#resourcepermissiontypedef) [:material-code-braces: ResourcePermissionOutputTypeDef](./type_defs.md#resourcepermissionoutputtypedef) 
3. See [:material-code-braces: UpdateFolderPermissionsResponseTypeDef](./type_defs.md#updatefolderpermissionsresponsetypedef) 


```python
# update_folder_permissions method usage example with argument unpacking

kwargs: UpdateFolderPermissionsRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "FolderId": ...,
}

parent.update_folder_permissions(**kwargs)
```

1. See [:material-code-braces: UpdateFolderPermissionsRequestTypeDef](./type_defs.md#updatefolderpermissionsrequesttypedef) 

### update\_group

Changes a group description.

Type annotations and code completion for `#!python session.create_client("quicksight").update_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/update_group.html)

```python
# update_group method definition

await def update_group(
    self,
    *,
    GroupName: str,
    AwsAccountId: str,
    Namespace: str,
    Description: str = ...,
) -> UpdateGroupResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateGroupResponseTypeDef](./type_defs.md#updategroupresponsetypedef) 


```python
# update_group method usage example with argument unpacking

kwargs: UpdateGroupRequestTypeDef = {  # (1)
    "GroupName": ...,
    "AwsAccountId": ...,
    "Namespace": ...,
}

parent.update_group(**kwargs)
```

1. See [:material-code-braces: UpdateGroupRequestTypeDef](./type_defs.md#updategrouprequesttypedef) 

### update\_iam\_policy\_assignment

Updates an existing IAM policy assignment.

Type annotations and code completion for `#!python session.create_client("quicksight").update_iam_policy_assignment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/update_iam_policy_assignment.html)

```python
# update_iam_policy_assignment method definition

await def update_iam_policy_assignment(
    self,
    *,
    AwsAccountId: str,
    AssignmentName: str,
    Namespace: str,
    AssignmentStatus: AssignmentStatusType = ...,  # (1)
    PolicyArn: str = ...,
    Identities: Mapping[str, Sequence[str]] = ...,
) -> UpdateIAMPolicyAssignmentResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: AssignmentStatusType](./literals.md#assignmentstatustype) 
2. See [:material-code-braces: UpdateIAMPolicyAssignmentResponseTypeDef](./type_defs.md#updateiampolicyassignmentresponsetypedef) 


```python
# update_iam_policy_assignment method usage example with argument unpacking

kwargs: UpdateIAMPolicyAssignmentRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "AssignmentName": ...,
    "Namespace": ...,
}

parent.update_iam_policy_assignment(**kwargs)
```

1. See [:material-code-braces: UpdateIAMPolicyAssignmentRequestTypeDef](./type_defs.md#updateiampolicyassignmentrequesttypedef) 

### update\_identity\_propagation\_config

Adds or updates services and authorized targets to configure what the Amazon
QuickSight IAM Identity Center application can access.

Type annotations and code completion for `#!python session.create_client("quicksight").update_identity_propagation_config` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/update_identity_propagation_config.html)

```python
# update_identity_propagation_config method definition

await def update_identity_propagation_config(
    self,
    *,
    AwsAccountId: str,
    Service: ServiceTypeType,  # (1)
    AuthorizedTargets: Sequence[str] = ...,
) -> UpdateIdentityPropagationConfigResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ServiceTypeType](./literals.md#servicetypetype) 
2. See [:material-code-braces: UpdateIdentityPropagationConfigResponseTypeDef](./type_defs.md#updateidentitypropagationconfigresponsetypedef) 


```python
# update_identity_propagation_config method usage example with argument unpacking

kwargs: UpdateIdentityPropagationConfigRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "Service": ...,
}

parent.update_identity_propagation_config(**kwargs)
```

1. See [:material-code-braces: UpdateIdentityPropagationConfigRequestTypeDef](./type_defs.md#updateidentitypropagationconfigrequesttypedef) 

### update\_ip\_restriction

Updates the content and status of IP rules.

Type annotations and code completion for `#!python session.create_client("quicksight").update_ip_restriction` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/update_ip_restriction.html)

```python
# update_ip_restriction method definition

await def update_ip_restriction(
    self,
    *,
    AwsAccountId: str,
    IpRestrictionRuleMap: Mapping[str, str] = ...,
    VpcIdRestrictionRuleMap: Mapping[str, str] = ...,
    VpcEndpointIdRestrictionRuleMap: Mapping[str, str] = ...,
    Enabled: bool = ...,
) -> UpdateIpRestrictionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateIpRestrictionResponseTypeDef](./type_defs.md#updateiprestrictionresponsetypedef) 


```python
# update_ip_restriction method usage example with argument unpacking

kwargs: UpdateIpRestrictionRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
}

parent.update_ip_restriction(**kwargs)
```

1. See [:material-code-braces: UpdateIpRestrictionRequestTypeDef](./type_defs.md#updateiprestrictionrequesttypedef) 

### update\_key\_registration

Updates a customer managed key in a Amazon QuickSight account.

Type annotations and code completion for `#!python session.create_client("quicksight").update_key_registration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/update_key_registration.html)

```python
# update_key_registration method definition

await def update_key_registration(
    self,
    *,
    AwsAccountId: str,
    KeyRegistration: Sequence[RegisteredCustomerManagedKeyTypeDef],  # (1)
) -> UpdateKeyRegistrationResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: RegisteredCustomerManagedKeyTypeDef](./type_defs.md#registeredcustomermanagedkeytypedef) 
2. See [:material-code-braces: UpdateKeyRegistrationResponseTypeDef](./type_defs.md#updatekeyregistrationresponsetypedef) 


```python
# update_key_registration method usage example with argument unpacking

kwargs: UpdateKeyRegistrationRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "KeyRegistration": ...,
}

parent.update_key_registration(**kwargs)
```

1. See [:material-code-braces: UpdateKeyRegistrationRequestTypeDef](./type_defs.md#updatekeyregistrationrequesttypedef) 

### update\_public\_sharing\_settings

Use the <code>UpdatePublicSharingSettings</code> operation to turn on or turn
off the public sharing settings of an Amazon QuickSight dashboard.

Type annotations and code completion for `#!python session.create_client("quicksight").update_public_sharing_settings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/update_public_sharing_settings.html)

```python
# update_public_sharing_settings method definition

await def update_public_sharing_settings(
    self,
    *,
    AwsAccountId: str,
    PublicSharingEnabled: bool = ...,
) -> UpdatePublicSharingSettingsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdatePublicSharingSettingsResponseTypeDef](./type_defs.md#updatepublicsharingsettingsresponsetypedef) 


```python
# update_public_sharing_settings method usage example with argument unpacking

kwargs: UpdatePublicSharingSettingsRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
}

parent.update_public_sharing_settings(**kwargs)
```

1. See [:material-code-braces: UpdatePublicSharingSettingsRequestTypeDef](./type_defs.md#updatepublicsharingsettingsrequesttypedef) 

### update\_q\_personalization\_configuration

Updates a personalization configuration.

Type annotations and code completion for `#!python session.create_client("quicksight").update_q_personalization_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/update_q_personalization_configuration.html)

```python
# update_q_personalization_configuration method definition

await def update_q_personalization_configuration(
    self,
    *,
    AwsAccountId: str,
    PersonalizationMode: PersonalizationModeType,  # (1)
) -> UpdateQPersonalizationConfigurationResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: PersonalizationModeType](./literals.md#personalizationmodetype) 
2. See [:material-code-braces: UpdateQPersonalizationConfigurationResponseTypeDef](./type_defs.md#updateqpersonalizationconfigurationresponsetypedef) 


```python
# update_q_personalization_configuration method usage example with argument unpacking

kwargs: UpdateQPersonalizationConfigurationRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "PersonalizationMode": ...,
}

parent.update_q_personalization_configuration(**kwargs)
```

1. See [:material-code-braces: UpdateQPersonalizationConfigurationRequestTypeDef](./type_defs.md#updateqpersonalizationconfigurationrequesttypedef) 

### update\_quick\_sight\_q\_search\_configuration

Updates the state of a Amazon QuickSight Q Search configuration.

Type annotations and code completion for `#!python session.create_client("quicksight").update_quick_sight_q_search_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/update_quick_sight_q_search_configuration.html)

```python
# update_quick_sight_q_search_configuration method definition

await def update_quick_sight_q_search_configuration(
    self,
    *,
    AwsAccountId: str,
    QSearchStatus: QSearchStatusType,  # (1)
) -> UpdateQuickSightQSearchConfigurationResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: QSearchStatusType](./literals.md#qsearchstatustype) 
2. See [:material-code-braces: UpdateQuickSightQSearchConfigurationResponseTypeDef](./type_defs.md#updatequicksightqsearchconfigurationresponsetypedef) 


```python
# update_quick_sight_q_search_configuration method usage example with argument unpacking

kwargs: UpdateQuickSightQSearchConfigurationRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "QSearchStatus": ...,
}

parent.update_quick_sight_q_search_configuration(**kwargs)
```

1. See [:material-code-braces: UpdateQuickSightQSearchConfigurationRequestTypeDef](./type_defs.md#updatequicksightqsearchconfigurationrequesttypedef) 

### update\_refresh\_schedule

Updates a refresh schedule for a dataset.

Type annotations and code completion for `#!python session.create_client("quicksight").update_refresh_schedule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/update_refresh_schedule.html)

```python
# update_refresh_schedule method definition

await def update_refresh_schedule(
    self,
    *,
    DataSetId: str,
    AwsAccountId: str,
    Schedule: RefreshScheduleUnionTypeDef,  # (1)
) -> UpdateRefreshScheduleResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: RefreshScheduleTypeDef](./type_defs.md#refreshscheduletypedef) [:material-code-braces: RefreshScheduleOutputTypeDef](./type_defs.md#refreshscheduleoutputtypedef) 
2. See [:material-code-braces: UpdateRefreshScheduleResponseTypeDef](./type_defs.md#updaterefreshscheduleresponsetypedef) 


```python
# update_refresh_schedule method usage example with argument unpacking

kwargs: UpdateRefreshScheduleRequestTypeDef = {  # (1)
    "DataSetId": ...,
    "AwsAccountId": ...,
    "Schedule": ...,
}

parent.update_refresh_schedule(**kwargs)
```

1. See [:material-code-braces: UpdateRefreshScheduleRequestTypeDef](./type_defs.md#updaterefreshschedulerequesttypedef) 

### update\_role\_custom\_permission

Updates the custom permissions that are associated with a role.

Type annotations and code completion for `#!python session.create_client("quicksight").update_role_custom_permission` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/update_role_custom_permission.html)

```python
# update_role_custom_permission method definition

await def update_role_custom_permission(
    self,
    *,
    CustomPermissionsName: str,
    Role: RoleType,  # (1)
    AwsAccountId: str,
    Namespace: str,
) -> UpdateRoleCustomPermissionResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: RoleType](./literals.md#roletype) 
2. See [:material-code-braces: UpdateRoleCustomPermissionResponseTypeDef](./type_defs.md#updaterolecustompermissionresponsetypedef) 


```python
# update_role_custom_permission method usage example with argument unpacking

kwargs: UpdateRoleCustomPermissionRequestTypeDef = {  # (1)
    "CustomPermissionsName": ...,
    "Role": ...,
    "AwsAccountId": ...,
    "Namespace": ...,
}

parent.update_role_custom_permission(**kwargs)
```

1. See [:material-code-braces: UpdateRoleCustomPermissionRequestTypeDef](./type_defs.md#updaterolecustompermissionrequesttypedef) 

### update\_spice\_capacity\_configuration

Updates the SPICE capacity configuration for a Amazon QuickSight account.

Type annotations and code completion for `#!python session.create_client("quicksight").update_spice_capacity_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/update_spice_capacity_configuration.html)

```python
# update_spice_capacity_configuration method definition

await def update_spice_capacity_configuration(
    self,
    *,
    AwsAccountId: str,
    PurchaseMode: PurchaseModeType,  # (1)
) -> UpdateSPICECapacityConfigurationResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: PurchaseModeType](./literals.md#purchasemodetype) 
2. See [:material-code-braces: UpdateSPICECapacityConfigurationResponseTypeDef](./type_defs.md#updatespicecapacityconfigurationresponsetypedef) 


```python
# update_spice_capacity_configuration method usage example with argument unpacking

kwargs: UpdateSPICECapacityConfigurationRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "PurchaseMode": ...,
}

parent.update_spice_capacity_configuration(**kwargs)
```

1. See [:material-code-braces: UpdateSPICECapacityConfigurationRequestTypeDef](./type_defs.md#updatespicecapacityconfigurationrequesttypedef) 

### update\_template

Updates a template from an existing Amazon QuickSight analysis or another
template.

Type annotations and code completion for `#!python session.create_client("quicksight").update_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/update_template.html)

```python
# update_template method definition

await def update_template(
    self,
    *,
    AwsAccountId: str,
    TemplateId: str,
    SourceEntity: TemplateSourceEntityTypeDef = ...,  # (1)
    VersionDescription: str = ...,
    Name: str = ...,
    Definition: TemplateVersionDefinitionUnionTypeDef = ...,  # (2)
    ValidationStrategy: ValidationStrategyTypeDef = ...,  # (3)
) -> UpdateTemplateResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: TemplateSourceEntityTypeDef](./type_defs.md#templatesourceentitytypedef) 
2. See [:material-code-braces: TemplateVersionDefinitionTypeDef](./type_defs.md#templateversiondefinitiontypedef) [:material-code-braces: TemplateVersionDefinitionOutputTypeDef](./type_defs.md#templateversiondefinitionoutputtypedef) 
3. See [:material-code-braces: ValidationStrategyTypeDef](./type_defs.md#validationstrategytypedef) 
4. See [:material-code-braces: UpdateTemplateResponseTypeDef](./type_defs.md#updatetemplateresponsetypedef) 


```python
# update_template method usage example with argument unpacking

kwargs: UpdateTemplateRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "TemplateId": ...,
}

parent.update_template(**kwargs)
```

1. See [:material-code-braces: UpdateTemplateRequestTypeDef](./type_defs.md#updatetemplaterequesttypedef) 

### update\_template\_alias

Updates the template alias of a template.

Type annotations and code completion for `#!python session.create_client("quicksight").update_template_alias` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/update_template_alias.html)

```python
# update_template_alias method definition

await def update_template_alias(
    self,
    *,
    AwsAccountId: str,
    TemplateId: str,
    AliasName: str,
    TemplateVersionNumber: int,
) -> UpdateTemplateAliasResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateTemplateAliasResponseTypeDef](./type_defs.md#updatetemplatealiasresponsetypedef) 


```python
# update_template_alias method usage example with argument unpacking

kwargs: UpdateTemplateAliasRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "TemplateId": ...,
    "AliasName": ...,
    "TemplateVersionNumber": ...,
}

parent.update_template_alias(**kwargs)
```

1. See [:material-code-braces: UpdateTemplateAliasRequestTypeDef](./type_defs.md#updatetemplatealiasrequesttypedef) 

### update\_template\_permissions

Updates the resource permissions for a template.

Type annotations and code completion for `#!python session.create_client("quicksight").update_template_permissions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/update_template_permissions.html)

```python
# update_template_permissions method definition

await def update_template_permissions(
    self,
    *,
    AwsAccountId: str,
    TemplateId: str,
    GrantPermissions: Sequence[ResourcePermissionUnionTypeDef] = ...,  # (1)
    RevokePermissions: Sequence[ResourcePermissionUnionTypeDef] = ...,  # (1)
) -> UpdateTemplatePermissionsResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: ResourcePermissionTypeDef](./type_defs.md#resourcepermissiontypedef) [:material-code-braces: ResourcePermissionOutputTypeDef](./type_defs.md#resourcepermissionoutputtypedef) 
2. See [:material-code-braces: ResourcePermissionTypeDef](./type_defs.md#resourcepermissiontypedef) [:material-code-braces: ResourcePermissionOutputTypeDef](./type_defs.md#resourcepermissionoutputtypedef) 
3. See [:material-code-braces: UpdateTemplatePermissionsResponseTypeDef](./type_defs.md#updatetemplatepermissionsresponsetypedef) 


```python
# update_template_permissions method usage example with argument unpacking

kwargs: UpdateTemplatePermissionsRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "TemplateId": ...,
}

parent.update_template_permissions(**kwargs)
```

1. See [:material-code-braces: UpdateTemplatePermissionsRequestTypeDef](./type_defs.md#updatetemplatepermissionsrequesttypedef) 

### update\_theme

Updates a theme.

Type annotations and code completion for `#!python session.create_client("quicksight").update_theme` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/update_theme.html)

```python
# update_theme method definition

await def update_theme(
    self,
    *,
    AwsAccountId: str,
    ThemeId: str,
    BaseThemeId: str,
    Name: str = ...,
    VersionDescription: str = ...,
    Configuration: ThemeConfigurationUnionTypeDef = ...,  # (1)
) -> UpdateThemeResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ThemeConfigurationTypeDef](./type_defs.md#themeconfigurationtypedef) [:material-code-braces: ThemeConfigurationOutputTypeDef](./type_defs.md#themeconfigurationoutputtypedef) 
2. See [:material-code-braces: UpdateThemeResponseTypeDef](./type_defs.md#updatethemeresponsetypedef) 


```python
# update_theme method usage example with argument unpacking

kwargs: UpdateThemeRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "ThemeId": ...,
    "BaseThemeId": ...,
}

parent.update_theme(**kwargs)
```

1. See [:material-code-braces: UpdateThemeRequestTypeDef](./type_defs.md#updatethemerequesttypedef) 

### update\_theme\_alias

Updates an alias of a theme.

Type annotations and code completion for `#!python session.create_client("quicksight").update_theme_alias` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/update_theme_alias.html)

```python
# update_theme_alias method definition

await def update_theme_alias(
    self,
    *,
    AwsAccountId: str,
    ThemeId: str,
    AliasName: str,
    ThemeVersionNumber: int,
) -> UpdateThemeAliasResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateThemeAliasResponseTypeDef](./type_defs.md#updatethemealiasresponsetypedef) 


```python
# update_theme_alias method usage example with argument unpacking

kwargs: UpdateThemeAliasRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "ThemeId": ...,
    "AliasName": ...,
    "ThemeVersionNumber": ...,
}

parent.update_theme_alias(**kwargs)
```

1. See [:material-code-braces: UpdateThemeAliasRequestTypeDef](./type_defs.md#updatethemealiasrequesttypedef) 

### update\_theme\_permissions

Updates the resource permissions for a theme.

Type annotations and code completion for `#!python session.create_client("quicksight").update_theme_permissions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/update_theme_permissions.html)

```python
# update_theme_permissions method definition

await def update_theme_permissions(
    self,
    *,
    AwsAccountId: str,
    ThemeId: str,
    GrantPermissions: Sequence[ResourcePermissionUnionTypeDef] = ...,  # (1)
    RevokePermissions: Sequence[ResourcePermissionUnionTypeDef] = ...,  # (1)
) -> UpdateThemePermissionsResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: ResourcePermissionTypeDef](./type_defs.md#resourcepermissiontypedef) [:material-code-braces: ResourcePermissionOutputTypeDef](./type_defs.md#resourcepermissionoutputtypedef) 
2. See [:material-code-braces: ResourcePermissionTypeDef](./type_defs.md#resourcepermissiontypedef) [:material-code-braces: ResourcePermissionOutputTypeDef](./type_defs.md#resourcepermissionoutputtypedef) 
3. See [:material-code-braces: UpdateThemePermissionsResponseTypeDef](./type_defs.md#updatethemepermissionsresponsetypedef) 


```python
# update_theme_permissions method usage example with argument unpacking

kwargs: UpdateThemePermissionsRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "ThemeId": ...,
}

parent.update_theme_permissions(**kwargs)
```

1. See [:material-code-braces: UpdateThemePermissionsRequestTypeDef](./type_defs.md#updatethemepermissionsrequesttypedef) 

### update\_topic

Updates a topic.

Type annotations and code completion for `#!python session.create_client("quicksight").update_topic` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/update_topic.html)

```python
# update_topic method definition

await def update_topic(
    self,
    *,
    AwsAccountId: str,
    TopicId: str,
    Topic: TopicDetailsUnionTypeDef,  # (1)
) -> UpdateTopicResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TopicDetailsTypeDef](./type_defs.md#topicdetailstypedef) [:material-code-braces: TopicDetailsOutputTypeDef](./type_defs.md#topicdetailsoutputtypedef) 
2. See [:material-code-braces: UpdateTopicResponseTypeDef](./type_defs.md#updatetopicresponsetypedef) 


```python
# update_topic method usage example with argument unpacking

kwargs: UpdateTopicRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "TopicId": ...,
    "Topic": ...,
}

parent.update_topic(**kwargs)
```

1. See [:material-code-braces: UpdateTopicRequestTypeDef](./type_defs.md#updatetopicrequesttypedef) 

### update\_topic\_permissions

Updates the permissions of a topic.

Type annotations and code completion for `#!python session.create_client("quicksight").update_topic_permissions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/update_topic_permissions.html)

```python
# update_topic_permissions method definition

await def update_topic_permissions(
    self,
    *,
    AwsAccountId: str,
    TopicId: str,
    GrantPermissions: Sequence[ResourcePermissionUnionTypeDef] = ...,  # (1)
    RevokePermissions: Sequence[ResourcePermissionUnionTypeDef] = ...,  # (1)
) -> UpdateTopicPermissionsResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: ResourcePermissionTypeDef](./type_defs.md#resourcepermissiontypedef) [:material-code-braces: ResourcePermissionOutputTypeDef](./type_defs.md#resourcepermissionoutputtypedef) 
2. See [:material-code-braces: ResourcePermissionTypeDef](./type_defs.md#resourcepermissiontypedef) [:material-code-braces: ResourcePermissionOutputTypeDef](./type_defs.md#resourcepermissionoutputtypedef) 
3. See [:material-code-braces: UpdateTopicPermissionsResponseTypeDef](./type_defs.md#updatetopicpermissionsresponsetypedef) 


```python
# update_topic_permissions method usage example with argument unpacking

kwargs: UpdateTopicPermissionsRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "TopicId": ...,
}

parent.update_topic_permissions(**kwargs)
```

1. See [:material-code-braces: UpdateTopicPermissionsRequestTypeDef](./type_defs.md#updatetopicpermissionsrequesttypedef) 

### update\_topic\_refresh\_schedule

Updates a topic refresh schedule.

Type annotations and code completion for `#!python session.create_client("quicksight").update_topic_refresh_schedule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/update_topic_refresh_schedule.html)

```python
# update_topic_refresh_schedule method definition

await def update_topic_refresh_schedule(
    self,
    *,
    AwsAccountId: str,
    TopicId: str,
    DatasetId: str,
    RefreshSchedule: TopicRefreshScheduleUnionTypeDef,  # (1)
) -> UpdateTopicRefreshScheduleResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TopicRefreshScheduleTypeDef](./type_defs.md#topicrefreshscheduletypedef) [:material-code-braces: TopicRefreshScheduleOutputTypeDef](./type_defs.md#topicrefreshscheduleoutputtypedef) 
2. See [:material-code-braces: UpdateTopicRefreshScheduleResponseTypeDef](./type_defs.md#updatetopicrefreshscheduleresponsetypedef) 


```python
# update_topic_refresh_schedule method usage example with argument unpacking

kwargs: UpdateTopicRefreshScheduleRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "TopicId": ...,
    "DatasetId": ...,
    "RefreshSchedule": ...,
}

parent.update_topic_refresh_schedule(**kwargs)
```

1. See [:material-code-braces: UpdateTopicRefreshScheduleRequestTypeDef](./type_defs.md#updatetopicrefreshschedulerequesttypedef) 

### update\_user

Updates an Amazon QuickSight user.

Type annotations and code completion for `#!python session.create_client("quicksight").update_user` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/update_user.html)

```python
# update_user method definition

await def update_user(
    self,
    *,
    UserName: str,
    AwsAccountId: str,
    Namespace: str,
    Email: str,
    Role: UserRoleType,  # (1)
    CustomPermissionsName: str = ...,
    UnapplyCustomPermissions: bool = ...,
    ExternalLoginFederationProviderType: str = ...,
    CustomFederationProviderUrl: str = ...,
    ExternalLoginId: str = ...,
) -> UpdateUserResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: UserRoleType](./literals.md#userroletype) 
2. See [:material-code-braces: UpdateUserResponseTypeDef](./type_defs.md#updateuserresponsetypedef) 


```python
# update_user method usage example with argument unpacking

kwargs: UpdateUserRequestTypeDef = {  # (1)
    "UserName": ...,
    "AwsAccountId": ...,
    "Namespace": ...,
    "Email": ...,
    "Role": ...,
}

parent.update_user(**kwargs)
```

1. See [:material-code-braces: UpdateUserRequestTypeDef](./type_defs.md#updateuserrequesttypedef) 

### update\_user\_custom\_permission

Updates a custom permissions profile for a user.

Type annotations and code completion for `#!python session.create_client("quicksight").update_user_custom_permission` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/update_user_custom_permission.html)

```python
# update_user_custom_permission method definition

await def update_user_custom_permission(
    self,
    *,
    UserName: str,
    AwsAccountId: str,
    Namespace: str,
    CustomPermissionsName: str,
) -> UpdateUserCustomPermissionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateUserCustomPermissionResponseTypeDef](./type_defs.md#updateusercustompermissionresponsetypedef) 


```python
# update_user_custom_permission method usage example with argument unpacking

kwargs: UpdateUserCustomPermissionRequestTypeDef = {  # (1)
    "UserName": ...,
    "AwsAccountId": ...,
    "Namespace": ...,
    "CustomPermissionsName": ...,
}

parent.update_user_custom_permission(**kwargs)
```

1. See [:material-code-braces: UpdateUserCustomPermissionRequestTypeDef](./type_defs.md#updateusercustompermissionrequesttypedef) 

### update\_vpc\_connection

Updates a VPC connection.

Type annotations and code completion for `#!python session.create_client("quicksight").update_vpc_connection` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight/client/update_vpc_connection.html)

```python
# update_vpc_connection method definition

await def update_vpc_connection(
    self,
    *,
    AwsAccountId: str,
    VPCConnectionId: str,
    Name: str,
    SubnetIds: Sequence[str],
    SecurityGroupIds: Sequence[str],
    RoleArn: str,
    DnsResolvers: Sequence[str] = ...,
) -> UpdateVPCConnectionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateVPCConnectionResponseTypeDef](./type_defs.md#updatevpcconnectionresponsetypedef) 


```python
# update_vpc_connection method usage example with argument unpacking

kwargs: UpdateVPCConnectionRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "VPCConnectionId": ...,
    "Name": ...,
    "SubnetIds": ...,
    "SecurityGroupIds": ...,
    "RoleArn": ...,
}

parent.update_vpc_connection(**kwargs)
```

1. See [:material-code-braces: UpdateVPCConnectionRequestTypeDef](./type_defs.md#updatevpcconnectionrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("quicksight").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("quicksight").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client)

```python
# __aexit__ method definition

await def __aexit__(
    self,
    exc_type: Union[Type[BaseException], None],
    exc_val: Union[BaseException, None],
    exc_tb: Union[TracebackType, None],
) -> None:
    ...
```




### get_paginator

Type annotations and code completion for `#!python session.create_client("quicksight").get_paginator` method with overloads.

- `client.get_paginator("describe_folder_permissions")` -> [DescribeFolderPermissionsPaginator](./paginators.md#describefolderpermissionspaginator)
- `client.get_paginator("describe_folder_resolved_permissions")` -> [DescribeFolderResolvedPermissionsPaginator](./paginators.md#describefolderresolvedpermissionspaginator)
- `client.get_paginator("list_analyses")` -> [ListAnalysesPaginator](./paginators.md#listanalysespaginator)
- `client.get_paginator("list_asset_bundle_export_jobs")` -> [ListAssetBundleExportJobsPaginator](./paginators.md#listassetbundleexportjobspaginator)
- `client.get_paginator("list_asset_bundle_import_jobs")` -> [ListAssetBundleImportJobsPaginator](./paginators.md#listassetbundleimportjobspaginator)
- `client.get_paginator("list_brands")` -> [ListBrandsPaginator](./paginators.md#listbrandspaginator)
- `client.get_paginator("list_custom_permissions")` -> [ListCustomPermissionsPaginator](./paginators.md#listcustompermissionspaginator)
- `client.get_paginator("list_dashboard_versions")` -> [ListDashboardVersionsPaginator](./paginators.md#listdashboardversionspaginator)
- `client.get_paginator("list_dashboards")` -> [ListDashboardsPaginator](./paginators.md#listdashboardspaginator)
- `client.get_paginator("list_data_sets")` -> [ListDataSetsPaginator](./paginators.md#listdatasetspaginator)
- `client.get_paginator("list_data_sources")` -> [ListDataSourcesPaginator](./paginators.md#listdatasourcespaginator)
- `client.get_paginator("list_folder_members")` -> [ListFolderMembersPaginator](./paginators.md#listfoldermemberspaginator)
- `client.get_paginator("list_folders_for_resource")` -> [ListFoldersForResourcePaginator](./paginators.md#listfoldersforresourcepaginator)
- `client.get_paginator("list_folders")` -> [ListFoldersPaginator](./paginators.md#listfolderspaginator)
- `client.get_paginator("list_group_memberships")` -> [ListGroupMembershipsPaginator](./paginators.md#listgroupmembershipspaginator)
- `client.get_paginator("list_groups")` -> [ListGroupsPaginator](./paginators.md#listgroupspaginator)
- `client.get_paginator("list_iam_policy_assignments_for_user")` -> [ListIAMPolicyAssignmentsForUserPaginator](./paginators.md#listiampolicyassignmentsforuserpaginator)
- `client.get_paginator("list_iam_policy_assignments")` -> [ListIAMPolicyAssignmentsPaginator](./paginators.md#listiampolicyassignmentspaginator)
- `client.get_paginator("list_ingestions")` -> [ListIngestionsPaginator](./paginators.md#listingestionspaginator)
- `client.get_paginator("list_namespaces")` -> [ListNamespacesPaginator](./paginators.md#listnamespacespaginator)
- `client.get_paginator("list_role_memberships")` -> [ListRoleMembershipsPaginator](./paginators.md#listrolemembershipspaginator)
- `client.get_paginator("list_template_aliases")` -> [ListTemplateAliasesPaginator](./paginators.md#listtemplatealiasespaginator)
- `client.get_paginator("list_template_versions")` -> [ListTemplateVersionsPaginator](./paginators.md#listtemplateversionspaginator)
- `client.get_paginator("list_templates")` -> [ListTemplatesPaginator](./paginators.md#listtemplatespaginator)
- `client.get_paginator("list_theme_versions")` -> [ListThemeVersionsPaginator](./paginators.md#listthemeversionspaginator)
- `client.get_paginator("list_themes")` -> [ListThemesPaginator](./paginators.md#listthemespaginator)
- `client.get_paginator("list_user_groups")` -> [ListUserGroupsPaginator](./paginators.md#listusergroupspaginator)
- `client.get_paginator("list_users")` -> [ListUsersPaginator](./paginators.md#listuserspaginator)
- `client.get_paginator("search_analyses")` -> [SearchAnalysesPaginator](./paginators.md#searchanalysespaginator)
- `client.get_paginator("search_dashboards")` -> [SearchDashboardsPaginator](./paginators.md#searchdashboardspaginator)
- `client.get_paginator("search_data_sets")` -> [SearchDataSetsPaginator](./paginators.md#searchdatasetspaginator)
- `client.get_paginator("search_data_sources")` -> [SearchDataSourcesPaginator](./paginators.md#searchdatasourcespaginator)
- `client.get_paginator("search_folders")` -> [SearchFoldersPaginator](./paginators.md#searchfolderspaginator)
- `client.get_paginator("search_groups")` -> [SearchGroupsPaginator](./paginators.md#searchgroupspaginator)
- `client.get_paginator("search_topics")` -> [SearchTopicsPaginator](./paginators.md#searchtopicspaginator)



