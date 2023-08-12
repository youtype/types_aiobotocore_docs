# QuickSightClient

> [Index](../README.md) > [QuickSight](./README.md) > QuickSightClient

!!! note ""

    Auto-generated documentation for [QuickSight](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight)
    type annotations stubs module [types-aiobotocore-quicksight](https://pypi.org/project/types-aiobotocore-quicksight/).

## QuickSightClient

Type annotations and code completion for `#!python session.create_client("quicksight")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client)

```python
QuickSightClient usage example

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
QuickSightClient.exceptions usage example

async with session.create_client("quicksight") as client:
    try:
        do_something(client)
    except (
            client.AccessDeniedException,
        client.ClientError,
        client.ConcurrentUpdatingException,
        client.ConflictException,
        client.DomainNotWhitelistedException,
        client.IdentityTypeNotSupportedException,
        client.InternalFailureException,
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
QuickSightClient usage type checking example

from types_aiobotocore_quicksight.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate

Check if an operation can be paginated.

Type annotations and code completion for `#!python session.create_client("quicksight").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.can_paginate)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### cancel\_ingestion

Cancels an ongoing ingestion of data into SPICE.

Type annotations and code completion for `#!python session.create_client("quicksight").cancel_ingestion` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.cancel_ingestion)

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

kwargs: CancelIngestionRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "DataSetId": ...,
    "IngestionId": ...,
}

parent.cancel_ingestion(**kwargs)
```

1. See [:material-code-braces: CancelIngestionRequestRequestTypeDef](./type_defs.md#cancelingestionrequestrequesttypedef) 

### close

Closes underlying endpoint connections.

Type annotations and code completion for `#!python session.create_client("quicksight").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.close)

```python
# close method definition

await def close(
    self,
) -> None:
    ...
```


### create\_account\_customization

Creates Amazon QuickSight customizations for the current Amazon Web Services
Region.

Type annotations and code completion for `#!python session.create_client("quicksight").create_account_customization` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.create_account_customization)

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

kwargs: CreateAccountCustomizationRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "AccountCustomization": ...,
}

parent.create_account_customization(**kwargs)
```

1. See [:material-code-braces: CreateAccountCustomizationRequestRequestTypeDef](./type_defs.md#createaccountcustomizationrequestrequesttypedef) 

### create\_account\_subscription

Creates an Amazon QuickSight account, or subscribes to Amazon QuickSight Q.

Type annotations and code completion for `#!python session.create_client("quicksight").create_account_subscription` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.create_account_subscription)

```python
# create_account_subscription method definition

await def create_account_subscription(
    self,
    *,
    Edition: EditionType,  # (1)
    AuthenticationMethod: AuthenticationMethodOptionType,  # (2)
    AwsAccountId: str,
    AccountName: str,
    NotificationEmail: str,
    ActiveDirectoryName: str = ...,
    Realm: str = ...,
    DirectoryId: str = ...,
    AdminGroup: Sequence[str] = ...,
    AuthorGroup: Sequence[str] = ...,
    ReaderGroup: Sequence[str] = ...,
    FirstName: str = ...,
    LastName: str = ...,
    EmailAddress: str = ...,
    ContactNumber: str = ...,
) -> CreateAccountSubscriptionResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: EditionType](./literals.md#editiontype) 
2. See [:material-code-brackets: AuthenticationMethodOptionType](./literals.md#authenticationmethodoptiontype) 
3. See [:material-code-braces: CreateAccountSubscriptionResponseTypeDef](./type_defs.md#createaccountsubscriptionresponsetypedef) 


```python
# create_account_subscription method usage example with argument unpacking

kwargs: CreateAccountSubscriptionRequestRequestTypeDef = {  # (1)
    "Edition": ...,
    "AuthenticationMethod": ...,
    "AwsAccountId": ...,
    "AccountName": ...,
    "NotificationEmail": ...,
}

parent.create_account_subscription(**kwargs)
```

1. See [:material-code-braces: CreateAccountSubscriptionRequestRequestTypeDef](./type_defs.md#createaccountsubscriptionrequestrequesttypedef) 

### create\_analysis

Creates an analysis in Amazon QuickSight.

Type annotations and code completion for `#!python session.create_client("quicksight").create_analysis` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.create_analysis)

```python
# create_analysis method definition

await def create_analysis(
    self,
    *,
    AwsAccountId: str,
    AnalysisId: str,
    Name: str,
    Parameters: ParametersTypeDef = ...,  # (1)
    Permissions: Sequence[ResourcePermissionTypeDef] = ...,  # (2)
    SourceEntity: AnalysisSourceEntityTypeDef = ...,  # (3)
    ThemeArn: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (4)
    Definition: AnalysisDefinitionTypeDef = ...,  # (5)
) -> CreateAnalysisResponseTypeDef:  # (6)
    ...
```

1. See [:material-code-braces: ParametersTypeDef](./type_defs.md#parameterstypedef) 
2. See [:material-code-braces: ResourcePermissionTypeDef](./type_defs.md#resourcepermissiontypedef) 
3. See [:material-code-braces: AnalysisSourceEntityTypeDef](./type_defs.md#analysissourceentitytypedef) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
5. See [:material-code-braces: AnalysisDefinitionTypeDef](./type_defs.md#analysisdefinitiontypedef) 
6. See [:material-code-braces: CreateAnalysisResponseTypeDef](./type_defs.md#createanalysisresponsetypedef) 


```python
# create_analysis method usage example with argument unpacking

kwargs: CreateAnalysisRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "AnalysisId": ...,
    "Name": ...,
}

parent.create_analysis(**kwargs)
```

1. See [:material-code-braces: CreateAnalysisRequestRequestTypeDef](./type_defs.md#createanalysisrequestrequesttypedef) 

### create\_dashboard

Creates a dashboard from either a template or directly with a
`DashboardDefinition`.

Type annotations and code completion for `#!python session.create_client("quicksight").create_dashboard` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.create_dashboard)

```python
# create_dashboard method definition

await def create_dashboard(
    self,
    *,
    AwsAccountId: str,
    DashboardId: str,
    Name: str,
    Parameters: ParametersTypeDef = ...,  # (1)
    Permissions: Sequence[ResourcePermissionTypeDef] = ...,  # (2)
    SourceEntity: DashboardSourceEntityTypeDef = ...,  # (3)
    Tags: Sequence[TagTypeDef] = ...,  # (4)
    VersionDescription: str = ...,
    DashboardPublishOptions: DashboardPublishOptionsTypeDef = ...,  # (5)
    ThemeArn: str = ...,
    Definition: DashboardVersionDefinitionTypeDef = ...,  # (6)
) -> CreateDashboardResponseTypeDef:  # (7)
    ...
```

1. See [:material-code-braces: ParametersTypeDef](./type_defs.md#parameterstypedef) 
2. See [:material-code-braces: ResourcePermissionTypeDef](./type_defs.md#resourcepermissiontypedef) 
3. See [:material-code-braces: DashboardSourceEntityTypeDef](./type_defs.md#dashboardsourceentitytypedef) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
5. See [:material-code-braces: DashboardPublishOptionsTypeDef](./type_defs.md#dashboardpublishoptionstypedef) 
6. See [:material-code-braces: DashboardVersionDefinitionTypeDef](./type_defs.md#dashboardversiondefinitiontypedef) 
7. See [:material-code-braces: CreateDashboardResponseTypeDef](./type_defs.md#createdashboardresponsetypedef) 


```python
# create_dashboard method usage example with argument unpacking

kwargs: CreateDashboardRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "DashboardId": ...,
    "Name": ...,
}

parent.create_dashboard(**kwargs)
```

1. See [:material-code-braces: CreateDashboardRequestRequestTypeDef](./type_defs.md#createdashboardrequestrequesttypedef) 

### create\_data\_set

Creates a dataset.

Type annotations and code completion for `#!python session.create_client("quicksight").create_data_set` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.create_data_set)

```python
# create_data_set method definition

await def create_data_set(
    self,
    *,
    AwsAccountId: str,
    DataSetId: str,
    Name: str,
    PhysicalTableMap: Mapping[str, PhysicalTableTypeDef],  # (1)
    ImportMode: DataSetImportModeType,  # (2)
    LogicalTableMap: Mapping[str, LogicalTableTypeDef] = ...,  # (3)
    ColumnGroups: Sequence[ColumnGroupTypeDef] = ...,  # (4)
    FieldFolders: Mapping[str, FieldFolderTypeDef] = ...,  # (5)
    Permissions: Sequence[ResourcePermissionTypeDef] = ...,  # (6)
    RowLevelPermissionDataSet: RowLevelPermissionDataSetTypeDef = ...,  # (7)
    RowLevelPermissionTagConfiguration: RowLevelPermissionTagConfigurationTypeDef = ...,  # (8)
    ColumnLevelPermissionRules: Sequence[ColumnLevelPermissionRuleTypeDef] = ...,  # (9)
    Tags: Sequence[TagTypeDef] = ...,  # (10)
    DataSetUsageConfiguration: DataSetUsageConfigurationTypeDef = ...,  # (11)
    DatasetParameters: Sequence[DatasetParameterTypeDef] = ...,  # (12)
) -> CreateDataSetResponseTypeDef:  # (13)
    ...
```

1. See [:material-code-braces: PhysicalTableTypeDef](./type_defs.md#physicaltabletypedef) 
2. See [:material-code-brackets: DataSetImportModeType](./literals.md#datasetimportmodetype) 
3. See [:material-code-braces: LogicalTableTypeDef](./type_defs.md#logicaltabletypedef) 
4. See [:material-code-braces: ColumnGroupTypeDef](./type_defs.md#columngrouptypedef) 
5. See [:material-code-braces: FieldFolderTypeDef](./type_defs.md#fieldfoldertypedef) 
6. See [:material-code-braces: ResourcePermissionTypeDef](./type_defs.md#resourcepermissiontypedef) 
7. See [:material-code-braces: RowLevelPermissionDataSetTypeDef](./type_defs.md#rowlevelpermissiondatasettypedef) 
8. See [:material-code-braces: RowLevelPermissionTagConfigurationTypeDef](./type_defs.md#rowlevelpermissiontagconfigurationtypedef) 
9. See [:material-code-braces: ColumnLevelPermissionRuleTypeDef](./type_defs.md#columnlevelpermissionruletypedef) 
10. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
11. See [:material-code-braces: DataSetUsageConfigurationTypeDef](./type_defs.md#datasetusageconfigurationtypedef) 
12. See [:material-code-braces: DatasetParameterTypeDef](./type_defs.md#datasetparametertypedef) 
13. See [:material-code-braces: CreateDataSetResponseTypeDef](./type_defs.md#createdatasetresponsetypedef) 


```python
# create_data_set method usage example with argument unpacking

kwargs: CreateDataSetRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "DataSetId": ...,
    "Name": ...,
    "PhysicalTableMap": ...,
    "ImportMode": ...,
}

parent.create_data_set(**kwargs)
```

1. See [:material-code-braces: CreateDataSetRequestRequestTypeDef](./type_defs.md#createdatasetrequestrequesttypedef) 

### create\_data\_source

Creates a data source.

Type annotations and code completion for `#!python session.create_client("quicksight").create_data_source` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.create_data_source)

```python
# create_data_source method definition

await def create_data_source(
    self,
    *,
    AwsAccountId: str,
    DataSourceId: str,
    Name: str,
    Type: DataSourceTypeType,  # (1)
    DataSourceParameters: DataSourceParametersTypeDef = ...,  # (2)
    Credentials: DataSourceCredentialsTypeDef = ...,  # (3)
    Permissions: Sequence[ResourcePermissionTypeDef] = ...,  # (4)
    VpcConnectionProperties: VpcConnectionPropertiesTypeDef = ...,  # (5)
    SslProperties: SslPropertiesTypeDef = ...,  # (6)
    Tags: Sequence[TagTypeDef] = ...,  # (7)
) -> CreateDataSourceResponseTypeDef:  # (8)
    ...
```

1. See [:material-code-brackets: DataSourceTypeType](./literals.md#datasourcetypetype) 
2. See [:material-code-braces: DataSourceParametersTypeDef](./type_defs.md#datasourceparameterstypedef) 
3. See [:material-code-braces: DataSourceCredentialsTypeDef](./type_defs.md#datasourcecredentialstypedef) 
4. See [:material-code-braces: ResourcePermissionTypeDef](./type_defs.md#resourcepermissiontypedef) 
5. See [:material-code-braces: VpcConnectionPropertiesTypeDef](./type_defs.md#vpcconnectionpropertiestypedef) 
6. See [:material-code-braces: SslPropertiesTypeDef](./type_defs.md#sslpropertiestypedef) 
7. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
8. See [:material-code-braces: CreateDataSourceResponseTypeDef](./type_defs.md#createdatasourceresponsetypedef) 


```python
# create_data_source method usage example with argument unpacking

kwargs: CreateDataSourceRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "DataSourceId": ...,
    "Name": ...,
    "Type": ...,
}

parent.create_data_source(**kwargs)
```

1. See [:material-code-braces: CreateDataSourceRequestRequestTypeDef](./type_defs.md#createdatasourcerequestrequesttypedef) 

### create\_folder

Creates an empty shared folder.

Type annotations and code completion for `#!python session.create_client("quicksight").create_folder` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.create_folder)

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
    Permissions: Sequence[ResourcePermissionTypeDef] = ...,  # (2)
    Tags: Sequence[TagTypeDef] = ...,  # (3)
) -> CreateFolderResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: FolderTypeType](./literals.md#foldertypetype) 
2. See [:material-code-braces: ResourcePermissionTypeDef](./type_defs.md#resourcepermissiontypedef) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
4. See [:material-code-braces: CreateFolderResponseTypeDef](./type_defs.md#createfolderresponsetypedef) 


```python
# create_folder method usage example with argument unpacking

kwargs: CreateFolderRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "FolderId": ...,
}

parent.create_folder(**kwargs)
```

1. See [:material-code-braces: CreateFolderRequestRequestTypeDef](./type_defs.md#createfolderrequestrequesttypedef) 

### create\_folder\_membership

Adds an asset, such as a dashboard, analysis, or dataset into a folder.

Type annotations and code completion for `#!python session.create_client("quicksight").create_folder_membership` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.create_folder_membership)

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

kwargs: CreateFolderMembershipRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "FolderId": ...,
    "MemberId": ...,
    "MemberType": ...,
}

parent.create_folder_membership(**kwargs)
```

1. See [:material-code-braces: CreateFolderMembershipRequestRequestTypeDef](./type_defs.md#createfoldermembershiprequestrequesttypedef) 

### create\_group

Use the `CreateGroup` operation to create a group in Amazon QuickSight.

Type annotations and code completion for `#!python session.create_client("quicksight").create_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.create_group)

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

kwargs: CreateGroupRequestRequestTypeDef = {  # (1)
    "GroupName": ...,
    "AwsAccountId": ...,
    "Namespace": ...,
}

parent.create_group(**kwargs)
```

1. See [:material-code-braces: CreateGroupRequestRequestTypeDef](./type_defs.md#creategrouprequestrequesttypedef) 

### create\_group\_membership

Adds an Amazon QuickSight user to an Amazon QuickSight group.

Type annotations and code completion for `#!python session.create_client("quicksight").create_group_membership` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.create_group_membership)

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

kwargs: CreateGroupMembershipRequestRequestTypeDef = {  # (1)
    "MemberName": ...,
    "GroupName": ...,
    "AwsAccountId": ...,
    "Namespace": ...,
}

parent.create_group_membership(**kwargs)
```

1. See [:material-code-braces: CreateGroupMembershipRequestRequestTypeDef](./type_defs.md#creategroupmembershiprequestrequesttypedef) 

### create\_iam\_policy\_assignment

Creates an assignment with one specified IAM policy, identified by its Amazon
Resource Name (ARN).

Type annotations and code completion for `#!python session.create_client("quicksight").create_iam_policy_assignment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.create_iam_policy_assignment)

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

kwargs: CreateIAMPolicyAssignmentRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "AssignmentName": ...,
    "AssignmentStatus": ...,
    "Namespace": ...,
}

parent.create_iam_policy_assignment(**kwargs)
```

1. See [:material-code-braces: CreateIAMPolicyAssignmentRequestRequestTypeDef](./type_defs.md#createiampolicyassignmentrequestrequesttypedef) 

### create\_ingestion

Creates and starts a new SPICE ingestion for a dataset.

Type annotations and code completion for `#!python session.create_client("quicksight").create_ingestion` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.create_ingestion)

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

kwargs: CreateIngestionRequestRequestTypeDef = {  # (1)
    "DataSetId": ...,
    "IngestionId": ...,
    "AwsAccountId": ...,
}

parent.create_ingestion(**kwargs)
```

1. See [:material-code-braces: CreateIngestionRequestRequestTypeDef](./type_defs.md#createingestionrequestrequesttypedef) 

### create\_namespace

(Enterprise edition only) Creates a new namespace for you to use with Amazon
QuickSight.

Type annotations and code completion for `#!python session.create_client("quicksight").create_namespace` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.create_namespace)

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

kwargs: CreateNamespaceRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "Namespace": ...,
    "IdentityStore": ...,
}

parent.create_namespace(**kwargs)
```

1. See [:material-code-braces: CreateNamespaceRequestRequestTypeDef](./type_defs.md#createnamespacerequestrequesttypedef) 

### create\_refresh\_schedule

Creates a refresh schedule for a dataset.

Type annotations and code completion for `#!python session.create_client("quicksight").create_refresh_schedule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.create_refresh_schedule)

```python
# create_refresh_schedule method definition

await def create_refresh_schedule(
    self,
    *,
    DataSetId: str,
    AwsAccountId: str,
    Schedule: RefreshScheduleTypeDef,  # (1)
) -> CreateRefreshScheduleResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: RefreshScheduleTypeDef](./type_defs.md#refreshscheduletypedef) 
2. See [:material-code-braces: CreateRefreshScheduleResponseTypeDef](./type_defs.md#createrefreshscheduleresponsetypedef) 


```python
# create_refresh_schedule method usage example with argument unpacking

kwargs: CreateRefreshScheduleRequestRequestTypeDef = {  # (1)
    "DataSetId": ...,
    "AwsAccountId": ...,
    "Schedule": ...,
}

parent.create_refresh_schedule(**kwargs)
```

1. See [:material-code-braces: CreateRefreshScheduleRequestRequestTypeDef](./type_defs.md#createrefreshschedulerequestrequesttypedef) 

### create\_template

Creates a template either from a `TemplateDefinition` or from an existing Amazon
QuickSight analysis or template.

Type annotations and code completion for `#!python session.create_client("quicksight").create_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.create_template)

```python
# create_template method definition

await def create_template(
    self,
    *,
    AwsAccountId: str,
    TemplateId: str,
    Name: str = ...,
    Permissions: Sequence[ResourcePermissionTypeDef] = ...,  # (1)
    SourceEntity: TemplateSourceEntityTypeDef = ...,  # (2)
    Tags: Sequence[TagTypeDef] = ...,  # (3)
    VersionDescription: str = ...,
    Definition: TemplateVersionDefinitionTypeDef = ...,  # (4)
) -> CreateTemplateResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-braces: ResourcePermissionTypeDef](./type_defs.md#resourcepermissiontypedef) 
2. See [:material-code-braces: TemplateSourceEntityTypeDef](./type_defs.md#templatesourceentitytypedef) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
4. See [:material-code-braces: TemplateVersionDefinitionTypeDef](./type_defs.md#templateversiondefinitiontypedef) 
5. See [:material-code-braces: CreateTemplateResponseTypeDef](./type_defs.md#createtemplateresponsetypedef) 


```python
# create_template method usage example with argument unpacking

kwargs: CreateTemplateRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "TemplateId": ...,
}

parent.create_template(**kwargs)
```

1. See [:material-code-braces: CreateTemplateRequestRequestTypeDef](./type_defs.md#createtemplaterequestrequesttypedef) 

### create\_template\_alias

Creates a template alias for a template.

Type annotations and code completion for `#!python session.create_client("quicksight").create_template_alias` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.create_template_alias)

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

kwargs: CreateTemplateAliasRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "TemplateId": ...,
    "AliasName": ...,
    "TemplateVersionNumber": ...,
}

parent.create_template_alias(**kwargs)
```

1. See [:material-code-braces: CreateTemplateAliasRequestRequestTypeDef](./type_defs.md#createtemplatealiasrequestrequesttypedef) 

### create\_theme

Creates a theme.

Type annotations and code completion for `#!python session.create_client("quicksight").create_theme` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.create_theme)

```python
# create_theme method definition

await def create_theme(
    self,
    *,
    AwsAccountId: str,
    ThemeId: str,
    Name: str,
    BaseThemeId: str,
    Configuration: ThemeConfigurationTypeDef,  # (1)
    VersionDescription: str = ...,
    Permissions: Sequence[ResourcePermissionTypeDef] = ...,  # (2)
    Tags: Sequence[TagTypeDef] = ...,  # (3)
) -> CreateThemeResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: ThemeConfigurationTypeDef](./type_defs.md#themeconfigurationtypedef) 
2. See [:material-code-braces: ResourcePermissionTypeDef](./type_defs.md#resourcepermissiontypedef) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
4. See [:material-code-braces: CreateThemeResponseTypeDef](./type_defs.md#createthemeresponsetypedef) 


```python
# create_theme method usage example with argument unpacking

kwargs: CreateThemeRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "ThemeId": ...,
    "Name": ...,
    "BaseThemeId": ...,
    "Configuration": ...,
}

parent.create_theme(**kwargs)
```

1. See [:material-code-braces: CreateThemeRequestRequestTypeDef](./type_defs.md#createthemerequestrequesttypedef) 

### create\_theme\_alias

Creates a theme alias for a theme.

Type annotations and code completion for `#!python session.create_client("quicksight").create_theme_alias` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.create_theme_alias)

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

kwargs: CreateThemeAliasRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "ThemeId": ...,
    "AliasName": ...,
    "ThemeVersionNumber": ...,
}

parent.create_theme_alias(**kwargs)
```

1. See [:material-code-braces: CreateThemeAliasRequestRequestTypeDef](./type_defs.md#createthemealiasrequestrequesttypedef) 

### create\_topic

Creates a new Q topic.

Type annotations and code completion for `#!python session.create_client("quicksight").create_topic` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.create_topic)

```python
# create_topic method definition

await def create_topic(
    self,
    *,
    AwsAccountId: str,
    TopicId: str,
    Topic: TopicDetailsTypeDef,  # (1)
    Tags: Sequence[TagTypeDef] = ...,  # (2)
) -> CreateTopicResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: TopicDetailsTypeDef](./type_defs.md#topicdetailstypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: CreateTopicResponseTypeDef](./type_defs.md#createtopicresponsetypedef) 


```python
# create_topic method usage example with argument unpacking

kwargs: CreateTopicRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "TopicId": ...,
    "Topic": ...,
}

parent.create_topic(**kwargs)
```

1. See [:material-code-braces: CreateTopicRequestRequestTypeDef](./type_defs.md#createtopicrequestrequesttypedef) 

### create\_topic\_refresh\_schedule

Creates a topic refresh schedule.

Type annotations and code completion for `#!python session.create_client("quicksight").create_topic_refresh_schedule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.create_topic_refresh_schedule)

```python
# create_topic_refresh_schedule method definition

await def create_topic_refresh_schedule(
    self,
    *,
    AwsAccountId: str,
    TopicId: str,
    DatasetArn: str,
    RefreshSchedule: TopicRefreshScheduleTypeDef,  # (1)
    DatasetName: str = ...,
) -> CreateTopicRefreshScheduleResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TopicRefreshScheduleTypeDef](./type_defs.md#topicrefreshscheduletypedef) 
2. See [:material-code-braces: CreateTopicRefreshScheduleResponseTypeDef](./type_defs.md#createtopicrefreshscheduleresponsetypedef) 


```python
# create_topic_refresh_schedule method usage example with argument unpacking

kwargs: CreateTopicRefreshScheduleRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "TopicId": ...,
    "DatasetArn": ...,
    "RefreshSchedule": ...,
}

parent.create_topic_refresh_schedule(**kwargs)
```

1. See [:material-code-braces: CreateTopicRefreshScheduleRequestRequestTypeDef](./type_defs.md#createtopicrefreshschedulerequestrequesttypedef) 

### create\_vpc\_connection

Creates a new VPC connection.

Type annotations and code completion for `#!python session.create_client("quicksight").create_vpc_connection` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.create_vpc_connection)

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

kwargs: CreateVPCConnectionRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "VPCConnectionId": ...,
    "Name": ...,
    "SubnetIds": ...,
    "SecurityGroupIds": ...,
    "RoleArn": ...,
}

parent.create_vpc_connection(**kwargs)
```

1. See [:material-code-braces: CreateVPCConnectionRequestRequestTypeDef](./type_defs.md#createvpcconnectionrequestrequesttypedef) 

### delete\_account\_customization

Deletes all Amazon QuickSight customizations in this Amazon Web Services Region
for the specified Amazon Web Services account and Amazon QuickSight namespace.

Type annotations and code completion for `#!python session.create_client("quicksight").delete_account_customization` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.delete_account_customization)

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

kwargs: DeleteAccountCustomizationRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
}

parent.delete_account_customization(**kwargs)
```

1. See [:material-code-braces: DeleteAccountCustomizationRequestRequestTypeDef](./type_defs.md#deleteaccountcustomizationrequestrequesttypedef) 

### delete\_account\_subscription

Use the `DeleteAccountSubscription` operation to delete an Amazon QuickSight
account.

Type annotations and code completion for `#!python session.create_client("quicksight").delete_account_subscription` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.delete_account_subscription)

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

kwargs: DeleteAccountSubscriptionRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
}

parent.delete_account_subscription(**kwargs)
```

1. See [:material-code-braces: DeleteAccountSubscriptionRequestRequestTypeDef](./type_defs.md#deleteaccountsubscriptionrequestrequesttypedef) 

### delete\_analysis

Deletes an analysis from Amazon QuickSight.

Type annotations and code completion for `#!python session.create_client("quicksight").delete_analysis` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.delete_analysis)

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

kwargs: DeleteAnalysisRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "AnalysisId": ...,
}

parent.delete_analysis(**kwargs)
```

1. See [:material-code-braces: DeleteAnalysisRequestRequestTypeDef](./type_defs.md#deleteanalysisrequestrequesttypedef) 

### delete\_dashboard

Deletes a dashboard.

Type annotations and code completion for `#!python session.create_client("quicksight").delete_dashboard` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.delete_dashboard)

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

kwargs: DeleteDashboardRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "DashboardId": ...,
}

parent.delete_dashboard(**kwargs)
```

1. See [:material-code-braces: DeleteDashboardRequestRequestTypeDef](./type_defs.md#deletedashboardrequestrequesttypedef) 

### delete\_data\_set

Deletes a dataset.

Type annotations and code completion for `#!python session.create_client("quicksight").delete_data_set` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.delete_data_set)

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

kwargs: DeleteDataSetRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "DataSetId": ...,
}

parent.delete_data_set(**kwargs)
```

1. See [:material-code-braces: DeleteDataSetRequestRequestTypeDef](./type_defs.md#deletedatasetrequestrequesttypedef) 

### delete\_data\_set\_refresh\_properties

Deletes the dataset refresh properties of the dataset.

Type annotations and code completion for `#!python session.create_client("quicksight").delete_data_set_refresh_properties` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.delete_data_set_refresh_properties)

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

kwargs: DeleteDataSetRefreshPropertiesRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "DataSetId": ...,
}

parent.delete_data_set_refresh_properties(**kwargs)
```

1. See [:material-code-braces: DeleteDataSetRefreshPropertiesRequestRequestTypeDef](./type_defs.md#deletedatasetrefreshpropertiesrequestrequesttypedef) 

### delete\_data\_source

Deletes the data source permanently.

Type annotations and code completion for `#!python session.create_client("quicksight").delete_data_source` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.delete_data_source)

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

kwargs: DeleteDataSourceRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "DataSourceId": ...,
}

parent.delete_data_source(**kwargs)
```

1. See [:material-code-braces: DeleteDataSourceRequestRequestTypeDef](./type_defs.md#deletedatasourcerequestrequesttypedef) 

### delete\_folder

Deletes an empty folder.

Type annotations and code completion for `#!python session.create_client("quicksight").delete_folder` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.delete_folder)

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

kwargs: DeleteFolderRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "FolderId": ...,
}

parent.delete_folder(**kwargs)
```

1. See [:material-code-braces: DeleteFolderRequestRequestTypeDef](./type_defs.md#deletefolderrequestrequesttypedef) 

### delete\_folder\_membership

Removes an asset, such as a dashboard, analysis, or dataset, from a folder.

Type annotations and code completion for `#!python session.create_client("quicksight").delete_folder_membership` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.delete_folder_membership)

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

kwargs: DeleteFolderMembershipRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "FolderId": ...,
    "MemberId": ...,
    "MemberType": ...,
}

parent.delete_folder_membership(**kwargs)
```

1. See [:material-code-braces: DeleteFolderMembershipRequestRequestTypeDef](./type_defs.md#deletefoldermembershiprequestrequesttypedef) 

### delete\_group

Removes a user group from Amazon QuickSight.

Type annotations and code completion for `#!python session.create_client("quicksight").delete_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.delete_group)

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

kwargs: DeleteGroupRequestRequestTypeDef = {  # (1)
    "GroupName": ...,
    "AwsAccountId": ...,
    "Namespace": ...,
}

parent.delete_group(**kwargs)
```

1. See [:material-code-braces: DeleteGroupRequestRequestTypeDef](./type_defs.md#deletegrouprequestrequesttypedef) 

### delete\_group\_membership

Removes a user from a group so that the user is no longer a member of the group.

Type annotations and code completion for `#!python session.create_client("quicksight").delete_group_membership` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.delete_group_membership)

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

kwargs: DeleteGroupMembershipRequestRequestTypeDef = {  # (1)
    "MemberName": ...,
    "GroupName": ...,
    "AwsAccountId": ...,
    "Namespace": ...,
}

parent.delete_group_membership(**kwargs)
```

1. See [:material-code-braces: DeleteGroupMembershipRequestRequestTypeDef](./type_defs.md#deletegroupmembershiprequestrequesttypedef) 

### delete\_iam\_policy\_assignment

Deletes an existing IAM policy assignment.

Type annotations and code completion for `#!python session.create_client("quicksight").delete_iam_policy_assignment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.delete_iam_policy_assignment)

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

kwargs: DeleteIAMPolicyAssignmentRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "AssignmentName": ...,
    "Namespace": ...,
}

parent.delete_iam_policy_assignment(**kwargs)
```

1. See [:material-code-braces: DeleteIAMPolicyAssignmentRequestRequestTypeDef](./type_defs.md#deleteiampolicyassignmentrequestrequesttypedef) 

### delete\_namespace

Deletes a namespace and the users and groups that are associated with the
namespace.

Type annotations and code completion for `#!python session.create_client("quicksight").delete_namespace` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.delete_namespace)

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

kwargs: DeleteNamespaceRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "Namespace": ...,
}

parent.delete_namespace(**kwargs)
```

1. See [:material-code-braces: DeleteNamespaceRequestRequestTypeDef](./type_defs.md#deletenamespacerequestrequesttypedef) 

### delete\_refresh\_schedule

Deletes a refresh schedule from a dataset.

Type annotations and code completion for `#!python session.create_client("quicksight").delete_refresh_schedule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.delete_refresh_schedule)

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

kwargs: DeleteRefreshScheduleRequestRequestTypeDef = {  # (1)
    "DataSetId": ...,
    "AwsAccountId": ...,
    "ScheduleId": ...,
}

parent.delete_refresh_schedule(**kwargs)
```

1. See [:material-code-braces: DeleteRefreshScheduleRequestRequestTypeDef](./type_defs.md#deleterefreshschedulerequestrequesttypedef) 

### delete\_template

Deletes a template.

Type annotations and code completion for `#!python session.create_client("quicksight").delete_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.delete_template)

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

kwargs: DeleteTemplateRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "TemplateId": ...,
}

parent.delete_template(**kwargs)
```

1. See [:material-code-braces: DeleteTemplateRequestRequestTypeDef](./type_defs.md#deletetemplaterequestrequesttypedef) 

### delete\_template\_alias

Deletes the item that the specified template alias points to.

Type annotations and code completion for `#!python session.create_client("quicksight").delete_template_alias` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.delete_template_alias)

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

kwargs: DeleteTemplateAliasRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "TemplateId": ...,
    "AliasName": ...,
}

parent.delete_template_alias(**kwargs)
```

1. See [:material-code-braces: DeleteTemplateAliasRequestRequestTypeDef](./type_defs.md#deletetemplatealiasrequestrequesttypedef) 

### delete\_theme

Deletes a theme.

Type annotations and code completion for `#!python session.create_client("quicksight").delete_theme` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.delete_theme)

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

kwargs: DeleteThemeRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "ThemeId": ...,
}

parent.delete_theme(**kwargs)
```

1. See [:material-code-braces: DeleteThemeRequestRequestTypeDef](./type_defs.md#deletethemerequestrequesttypedef) 

### delete\_theme\_alias

Deletes the version of the theme that the specified theme alias points to.

Type annotations and code completion for `#!python session.create_client("quicksight").delete_theme_alias` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.delete_theme_alias)

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

kwargs: DeleteThemeAliasRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "ThemeId": ...,
    "AliasName": ...,
}

parent.delete_theme_alias(**kwargs)
```

1. See [:material-code-braces: DeleteThemeAliasRequestRequestTypeDef](./type_defs.md#deletethemealiasrequestrequesttypedef) 

### delete\_topic

Deletes a topic.

Type annotations and code completion for `#!python session.create_client("quicksight").delete_topic` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.delete_topic)

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

kwargs: DeleteTopicRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "TopicId": ...,
}

parent.delete_topic(**kwargs)
```

1. See [:material-code-braces: DeleteTopicRequestRequestTypeDef](./type_defs.md#deletetopicrequestrequesttypedef) 

### delete\_topic\_refresh\_schedule

Deletes a topic refresh schedule.

Type annotations and code completion for `#!python session.create_client("quicksight").delete_topic_refresh_schedule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.delete_topic_refresh_schedule)

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

kwargs: DeleteTopicRefreshScheduleRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "TopicId": ...,
    "DatasetId": ...,
}

parent.delete_topic_refresh_schedule(**kwargs)
```

1. See [:material-code-braces: DeleteTopicRefreshScheduleRequestRequestTypeDef](./type_defs.md#deletetopicrefreshschedulerequestrequesttypedef) 

### delete\_user

Deletes the Amazon QuickSight user that is associated with the identity of the
IAM user or role that's making the call.

Type annotations and code completion for `#!python session.create_client("quicksight").delete_user` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.delete_user)

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

kwargs: DeleteUserRequestRequestTypeDef = {  # (1)
    "UserName": ...,
    "AwsAccountId": ...,
    "Namespace": ...,
}

parent.delete_user(**kwargs)
```

1. See [:material-code-braces: DeleteUserRequestRequestTypeDef](./type_defs.md#deleteuserrequestrequesttypedef) 

### delete\_user\_by\_principal\_id

Deletes a user identified by its principal ID.

Type annotations and code completion for `#!python session.create_client("quicksight").delete_user_by_principal_id` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.delete_user_by_principal_id)

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

kwargs: DeleteUserByPrincipalIdRequestRequestTypeDef = {  # (1)
    "PrincipalId": ...,
    "AwsAccountId": ...,
    "Namespace": ...,
}

parent.delete_user_by_principal_id(**kwargs)
```

1. See [:material-code-braces: DeleteUserByPrincipalIdRequestRequestTypeDef](./type_defs.md#deleteuserbyprincipalidrequestrequesttypedef) 

### delete\_vpc\_connection

Deletes a VPC connection.

Type annotations and code completion for `#!python session.create_client("quicksight").delete_vpc_connection` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.delete_vpc_connection)

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

kwargs: DeleteVPCConnectionRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "VPCConnectionId": ...,
}

parent.delete_vpc_connection(**kwargs)
```

1. See [:material-code-braces: DeleteVPCConnectionRequestRequestTypeDef](./type_defs.md#deletevpcconnectionrequestrequesttypedef) 

### describe\_account\_customization

Describes the customizations associated with the provided Amazon Web Services
account and Amazon Amazon QuickSight namespace in an Amazon Web Services Region.

Type annotations and code completion for `#!python session.create_client("quicksight").describe_account_customization` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.describe_account_customization)

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

kwargs: DescribeAccountCustomizationRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
}

parent.describe_account_customization(**kwargs)
```

1. See [:material-code-braces: DescribeAccountCustomizationRequestRequestTypeDef](./type_defs.md#describeaccountcustomizationrequestrequesttypedef) 

### describe\_account\_settings

Describes the settings that were used when your Amazon QuickSight subscription
was first created in this Amazon Web Services account.

Type annotations and code completion for `#!python session.create_client("quicksight").describe_account_settings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.describe_account_settings)

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

kwargs: DescribeAccountSettingsRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
}

parent.describe_account_settings(**kwargs)
```

1. See [:material-code-braces: DescribeAccountSettingsRequestRequestTypeDef](./type_defs.md#describeaccountsettingsrequestrequesttypedef) 

### describe\_account\_subscription

Use the DescribeAccountSubscription operation to receive a description of an
Amazon QuickSight account's subscription.

Type annotations and code completion for `#!python session.create_client("quicksight").describe_account_subscription` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.describe_account_subscription)

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

kwargs: DescribeAccountSubscriptionRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
}

parent.describe_account_subscription(**kwargs)
```

1. See [:material-code-braces: DescribeAccountSubscriptionRequestRequestTypeDef](./type_defs.md#describeaccountsubscriptionrequestrequesttypedef) 

### describe\_analysis

Provides a summary of the metadata for an analysis.

Type annotations and code completion for `#!python session.create_client("quicksight").describe_analysis` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.describe_analysis)

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

kwargs: DescribeAnalysisRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "AnalysisId": ...,
}

parent.describe_analysis(**kwargs)
```

1. See [:material-code-braces: DescribeAnalysisRequestRequestTypeDef](./type_defs.md#describeanalysisrequestrequesttypedef) 

### describe\_analysis\_definition

Provides a detailed description of the definition of an analysis.

Type annotations and code completion for `#!python session.create_client("quicksight").describe_analysis_definition` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.describe_analysis_definition)

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

kwargs: DescribeAnalysisDefinitionRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "AnalysisId": ...,
}

parent.describe_analysis_definition(**kwargs)
```

1. See [:material-code-braces: DescribeAnalysisDefinitionRequestRequestTypeDef](./type_defs.md#describeanalysisdefinitionrequestrequesttypedef) 

### describe\_analysis\_permissions

Provides the read and write permissions for an analysis.

Type annotations and code completion for `#!python session.create_client("quicksight").describe_analysis_permissions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.describe_analysis_permissions)

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

kwargs: DescribeAnalysisPermissionsRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "AnalysisId": ...,
}

parent.describe_analysis_permissions(**kwargs)
```

1. See [:material-code-braces: DescribeAnalysisPermissionsRequestRequestTypeDef](./type_defs.md#describeanalysispermissionsrequestrequesttypedef) 

### describe\_asset\_bundle\_export\_job

Describes an existing export job.

Type annotations and code completion for `#!python session.create_client("quicksight").describe_asset_bundle_export_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.describe_asset_bundle_export_job)

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

kwargs: DescribeAssetBundleExportJobRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "AssetBundleExportJobId": ...,
}

parent.describe_asset_bundle_export_job(**kwargs)
```

1. See [:material-code-braces: DescribeAssetBundleExportJobRequestRequestTypeDef](./type_defs.md#describeassetbundleexportjobrequestrequesttypedef) 

### describe\_asset\_bundle\_import\_job

Describes an existing import job.

Type annotations and code completion for `#!python session.create_client("quicksight").describe_asset_bundle_import_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.describe_asset_bundle_import_job)

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

kwargs: DescribeAssetBundleImportJobRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "AssetBundleImportJobId": ...,
}

parent.describe_asset_bundle_import_job(**kwargs)
```

1. See [:material-code-braces: DescribeAssetBundleImportJobRequestRequestTypeDef](./type_defs.md#describeassetbundleimportjobrequestrequesttypedef) 

### describe\_dashboard

Provides a summary for a dashboard.

Type annotations and code completion for `#!python session.create_client("quicksight").describe_dashboard` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.describe_dashboard)

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

kwargs: DescribeDashboardRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "DashboardId": ...,
}

parent.describe_dashboard(**kwargs)
```

1. See [:material-code-braces: DescribeDashboardRequestRequestTypeDef](./type_defs.md#describedashboardrequestrequesttypedef) 

### describe\_dashboard\_definition

Provides a detailed description of the definition of a dashboard.

Type annotations and code completion for `#!python session.create_client("quicksight").describe_dashboard_definition` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.describe_dashboard_definition)

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

kwargs: DescribeDashboardDefinitionRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "DashboardId": ...,
}

parent.describe_dashboard_definition(**kwargs)
```

1. See [:material-code-braces: DescribeDashboardDefinitionRequestRequestTypeDef](./type_defs.md#describedashboarddefinitionrequestrequesttypedef) 

### describe\_dashboard\_permissions

Describes read and write permissions for a dashboard.

Type annotations and code completion for `#!python session.create_client("quicksight").describe_dashboard_permissions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.describe_dashboard_permissions)

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

kwargs: DescribeDashboardPermissionsRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "DashboardId": ...,
}

parent.describe_dashboard_permissions(**kwargs)
```

1. See [:material-code-braces: DescribeDashboardPermissionsRequestRequestTypeDef](./type_defs.md#describedashboardpermissionsrequestrequesttypedef) 

### describe\_dashboard\_snapshot\_job

Describes an existing snapshot job.

Type annotations and code completion for `#!python session.create_client("quicksight").describe_dashboard_snapshot_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.describe_dashboard_snapshot_job)

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

kwargs: DescribeDashboardSnapshotJobRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "DashboardId": ...,
    "SnapshotJobId": ...,
}

parent.describe_dashboard_snapshot_job(**kwargs)
```

1. See [:material-code-braces: DescribeDashboardSnapshotJobRequestRequestTypeDef](./type_defs.md#describedashboardsnapshotjobrequestrequesttypedef) 

### describe\_dashboard\_snapshot\_job\_result

Describes the result of an existing snapshot job that has finished running.

Type annotations and code completion for `#!python session.create_client("quicksight").describe_dashboard_snapshot_job_result` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.describe_dashboard_snapshot_job_result)

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

kwargs: DescribeDashboardSnapshotJobResultRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "DashboardId": ...,
    "SnapshotJobId": ...,
}

parent.describe_dashboard_snapshot_job_result(**kwargs)
```

1. See [:material-code-braces: DescribeDashboardSnapshotJobResultRequestRequestTypeDef](./type_defs.md#describedashboardsnapshotjobresultrequestrequesttypedef) 

### describe\_data\_set

Describes a dataset.

Type annotations and code completion for `#!python session.create_client("quicksight").describe_data_set` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.describe_data_set)

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

kwargs: DescribeDataSetRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "DataSetId": ...,
}

parent.describe_data_set(**kwargs)
```

1. See [:material-code-braces: DescribeDataSetRequestRequestTypeDef](./type_defs.md#describedatasetrequestrequesttypedef) 

### describe\_data\_set\_permissions

Describes the permissions on a dataset.

Type annotations and code completion for `#!python session.create_client("quicksight").describe_data_set_permissions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.describe_data_set_permissions)

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

kwargs: DescribeDataSetPermissionsRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "DataSetId": ...,
}

parent.describe_data_set_permissions(**kwargs)
```

1. See [:material-code-braces: DescribeDataSetPermissionsRequestRequestTypeDef](./type_defs.md#describedatasetpermissionsrequestrequesttypedef) 

### describe\_data\_set\_refresh\_properties

Describes the refresh properties of a dataset.

Type annotations and code completion for `#!python session.create_client("quicksight").describe_data_set_refresh_properties` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.describe_data_set_refresh_properties)

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

kwargs: DescribeDataSetRefreshPropertiesRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "DataSetId": ...,
}

parent.describe_data_set_refresh_properties(**kwargs)
```

1. See [:material-code-braces: DescribeDataSetRefreshPropertiesRequestRequestTypeDef](./type_defs.md#describedatasetrefreshpropertiesrequestrequesttypedef) 

### describe\_data\_source

Describes a data source.

Type annotations and code completion for `#!python session.create_client("quicksight").describe_data_source` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.describe_data_source)

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

kwargs: DescribeDataSourceRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "DataSourceId": ...,
}

parent.describe_data_source(**kwargs)
```

1. See [:material-code-braces: DescribeDataSourceRequestRequestTypeDef](./type_defs.md#describedatasourcerequestrequesttypedef) 

### describe\_data\_source\_permissions

Describes the resource permissions for a data source.

Type annotations and code completion for `#!python session.create_client("quicksight").describe_data_source_permissions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.describe_data_source_permissions)

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

kwargs: DescribeDataSourcePermissionsRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "DataSourceId": ...,
}

parent.describe_data_source_permissions(**kwargs)
```

1. See [:material-code-braces: DescribeDataSourcePermissionsRequestRequestTypeDef](./type_defs.md#describedatasourcepermissionsrequestrequesttypedef) 

### describe\_folder

Describes a folder.

Type annotations and code completion for `#!python session.create_client("quicksight").describe_folder` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.describe_folder)

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

kwargs: DescribeFolderRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "FolderId": ...,
}

parent.describe_folder(**kwargs)
```

1. See [:material-code-braces: DescribeFolderRequestRequestTypeDef](./type_defs.md#describefolderrequestrequesttypedef) 

### describe\_folder\_permissions

Describes permissions for a folder.

Type annotations and code completion for `#!python session.create_client("quicksight").describe_folder_permissions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.describe_folder_permissions)

```python
# describe_folder_permissions method definition

await def describe_folder_permissions(
    self,
    *,
    AwsAccountId: str,
    FolderId: str,
) -> DescribeFolderPermissionsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeFolderPermissionsResponseTypeDef](./type_defs.md#describefolderpermissionsresponsetypedef) 


```python
# describe_folder_permissions method usage example with argument unpacking

kwargs: DescribeFolderPermissionsRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "FolderId": ...,
}

parent.describe_folder_permissions(**kwargs)
```

1. See [:material-code-braces: DescribeFolderPermissionsRequestRequestTypeDef](./type_defs.md#describefolderpermissionsrequestrequesttypedef) 

### describe\_folder\_resolved\_permissions

Describes the folder resolved permissions.

Type annotations and code completion for `#!python session.create_client("quicksight").describe_folder_resolved_permissions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.describe_folder_resolved_permissions)

```python
# describe_folder_resolved_permissions method definition

await def describe_folder_resolved_permissions(
    self,
    *,
    AwsAccountId: str,
    FolderId: str,
) -> DescribeFolderResolvedPermissionsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeFolderResolvedPermissionsResponseTypeDef](./type_defs.md#describefolderresolvedpermissionsresponsetypedef) 


```python
# describe_folder_resolved_permissions method usage example with argument unpacking

kwargs: DescribeFolderResolvedPermissionsRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "FolderId": ...,
}

parent.describe_folder_resolved_permissions(**kwargs)
```

1. See [:material-code-braces: DescribeFolderResolvedPermissionsRequestRequestTypeDef](./type_defs.md#describefolderresolvedpermissionsrequestrequesttypedef) 

### describe\_group

Returns an Amazon QuickSight group's description and Amazon Resource Name (ARN).

Type annotations and code completion for `#!python session.create_client("quicksight").describe_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.describe_group)

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

kwargs: DescribeGroupRequestRequestTypeDef = {  # (1)
    "GroupName": ...,
    "AwsAccountId": ...,
    "Namespace": ...,
}

parent.describe_group(**kwargs)
```

1. See [:material-code-braces: DescribeGroupRequestRequestTypeDef](./type_defs.md#describegrouprequestrequesttypedef) 

### describe\_group\_membership

Use the `DescribeGroupMembership` operation to determine if a user is a member
of the specified group.

Type annotations and code completion for `#!python session.create_client("quicksight").describe_group_membership` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.describe_group_membership)

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

kwargs: DescribeGroupMembershipRequestRequestTypeDef = {  # (1)
    "MemberName": ...,
    "GroupName": ...,
    "AwsAccountId": ...,
    "Namespace": ...,
}

parent.describe_group_membership(**kwargs)
```

1. See [:material-code-braces: DescribeGroupMembershipRequestRequestTypeDef](./type_defs.md#describegroupmembershiprequestrequesttypedef) 

### describe\_iam\_policy\_assignment

Describes an existing IAM policy assignment, as specified by the assignment
name.

Type annotations and code completion for `#!python session.create_client("quicksight").describe_iam_policy_assignment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.describe_iam_policy_assignment)

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

kwargs: DescribeIAMPolicyAssignmentRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "AssignmentName": ...,
    "Namespace": ...,
}

parent.describe_iam_policy_assignment(**kwargs)
```

1. See [:material-code-braces: DescribeIAMPolicyAssignmentRequestRequestTypeDef](./type_defs.md#describeiampolicyassignmentrequestrequesttypedef) 

### describe\_ingestion

Describes a SPICE ingestion.

Type annotations and code completion for `#!python session.create_client("quicksight").describe_ingestion` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.describe_ingestion)

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

kwargs: DescribeIngestionRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "DataSetId": ...,
    "IngestionId": ...,
}

parent.describe_ingestion(**kwargs)
```

1. See [:material-code-braces: DescribeIngestionRequestRequestTypeDef](./type_defs.md#describeingestionrequestrequesttypedef) 

### describe\_ip\_restriction

Provides a summary and status of IP rules.

Type annotations and code completion for `#!python session.create_client("quicksight").describe_ip_restriction` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.describe_ip_restriction)

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

kwargs: DescribeIpRestrictionRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
}

parent.describe_ip_restriction(**kwargs)
```

1. See [:material-code-braces: DescribeIpRestrictionRequestRequestTypeDef](./type_defs.md#describeiprestrictionrequestrequesttypedef) 

### describe\_namespace

Describes the current namespace.

Type annotations and code completion for `#!python session.create_client("quicksight").describe_namespace` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.describe_namespace)

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

kwargs: DescribeNamespaceRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "Namespace": ...,
}

parent.describe_namespace(**kwargs)
```

1. See [:material-code-braces: DescribeNamespaceRequestRequestTypeDef](./type_defs.md#describenamespacerequestrequesttypedef) 

### describe\_refresh\_schedule

Provides a summary of a refresh schedule.

Type annotations and code completion for `#!python session.create_client("quicksight").describe_refresh_schedule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.describe_refresh_schedule)

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

kwargs: DescribeRefreshScheduleRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "DataSetId": ...,
    "ScheduleId": ...,
}

parent.describe_refresh_schedule(**kwargs)
```

1. See [:material-code-braces: DescribeRefreshScheduleRequestRequestTypeDef](./type_defs.md#describerefreshschedulerequestrequesttypedef) 

### describe\_template

Describes a template's metadata.

Type annotations and code completion for `#!python session.create_client("quicksight").describe_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.describe_template)

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

kwargs: DescribeTemplateRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "TemplateId": ...,
}

parent.describe_template(**kwargs)
```

1. See [:material-code-braces: DescribeTemplateRequestRequestTypeDef](./type_defs.md#describetemplaterequestrequesttypedef) 

### describe\_template\_alias

Describes the template alias for a template.

Type annotations and code completion for `#!python session.create_client("quicksight").describe_template_alias` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.describe_template_alias)

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

kwargs: DescribeTemplateAliasRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "TemplateId": ...,
    "AliasName": ...,
}

parent.describe_template_alias(**kwargs)
```

1. See [:material-code-braces: DescribeTemplateAliasRequestRequestTypeDef](./type_defs.md#describetemplatealiasrequestrequesttypedef) 

### describe\_template\_definition

Provides a detailed description of the definition of a template.

Type annotations and code completion for `#!python session.create_client("quicksight").describe_template_definition` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.describe_template_definition)

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

kwargs: DescribeTemplateDefinitionRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "TemplateId": ...,
}

parent.describe_template_definition(**kwargs)
```

1. See [:material-code-braces: DescribeTemplateDefinitionRequestRequestTypeDef](./type_defs.md#describetemplatedefinitionrequestrequesttypedef) 

### describe\_template\_permissions

Describes read and write permissions on a template.

Type annotations and code completion for `#!python session.create_client("quicksight").describe_template_permissions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.describe_template_permissions)

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

kwargs: DescribeTemplatePermissionsRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "TemplateId": ...,
}

parent.describe_template_permissions(**kwargs)
```

1. See [:material-code-braces: DescribeTemplatePermissionsRequestRequestTypeDef](./type_defs.md#describetemplatepermissionsrequestrequesttypedef) 

### describe\_theme

Describes a theme.

Type annotations and code completion for `#!python session.create_client("quicksight").describe_theme` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.describe_theme)

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

kwargs: DescribeThemeRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "ThemeId": ...,
}

parent.describe_theme(**kwargs)
```

1. See [:material-code-braces: DescribeThemeRequestRequestTypeDef](./type_defs.md#describethemerequestrequesttypedef) 

### describe\_theme\_alias

Describes the alias for a theme.

Type annotations and code completion for `#!python session.create_client("quicksight").describe_theme_alias` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.describe_theme_alias)

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

kwargs: DescribeThemeAliasRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "ThemeId": ...,
    "AliasName": ...,
}

parent.describe_theme_alias(**kwargs)
```

1. See [:material-code-braces: DescribeThemeAliasRequestRequestTypeDef](./type_defs.md#describethemealiasrequestrequesttypedef) 

### describe\_theme\_permissions

Describes the read and write permissions for a theme.

Type annotations and code completion for `#!python session.create_client("quicksight").describe_theme_permissions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.describe_theme_permissions)

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

kwargs: DescribeThemePermissionsRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "ThemeId": ...,
}

parent.describe_theme_permissions(**kwargs)
```

1. See [:material-code-braces: DescribeThemePermissionsRequestRequestTypeDef](./type_defs.md#describethemepermissionsrequestrequesttypedef) 

### describe\_topic

Describes a topic.

Type annotations and code completion for `#!python session.create_client("quicksight").describe_topic` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.describe_topic)

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

kwargs: DescribeTopicRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "TopicId": ...,
}

parent.describe_topic(**kwargs)
```

1. See [:material-code-braces: DescribeTopicRequestRequestTypeDef](./type_defs.md#describetopicrequestrequesttypedef) 

### describe\_topic\_permissions

Describes the permissions of a topic.

Type annotations and code completion for `#!python session.create_client("quicksight").describe_topic_permissions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.describe_topic_permissions)

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

kwargs: DescribeTopicPermissionsRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "TopicId": ...,
}

parent.describe_topic_permissions(**kwargs)
```

1. See [:material-code-braces: DescribeTopicPermissionsRequestRequestTypeDef](./type_defs.md#describetopicpermissionsrequestrequesttypedef) 

### describe\_topic\_refresh

Describes the status of a topic refresh.

Type annotations and code completion for `#!python session.create_client("quicksight").describe_topic_refresh` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.describe_topic_refresh)

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

kwargs: DescribeTopicRefreshRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "TopicId": ...,
    "RefreshId": ...,
}

parent.describe_topic_refresh(**kwargs)
```

1. See [:material-code-braces: DescribeTopicRefreshRequestRequestTypeDef](./type_defs.md#describetopicrefreshrequestrequesttypedef) 

### describe\_topic\_refresh\_schedule

Deletes a topic refresh schedule.

Type annotations and code completion for `#!python session.create_client("quicksight").describe_topic_refresh_schedule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.describe_topic_refresh_schedule)

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

kwargs: DescribeTopicRefreshScheduleRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "TopicId": ...,
    "DatasetId": ...,
}

parent.describe_topic_refresh_schedule(**kwargs)
```

1. See [:material-code-braces: DescribeTopicRefreshScheduleRequestRequestTypeDef](./type_defs.md#describetopicrefreshschedulerequestrequesttypedef) 

### describe\_user

Returns information about a user, given the user name.

Type annotations and code completion for `#!python session.create_client("quicksight").describe_user` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.describe_user)

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

kwargs: DescribeUserRequestRequestTypeDef = {  # (1)
    "UserName": ...,
    "AwsAccountId": ...,
    "Namespace": ...,
}

parent.describe_user(**kwargs)
```

1. See [:material-code-braces: DescribeUserRequestRequestTypeDef](./type_defs.md#describeuserrequestrequesttypedef) 

### describe\_vpc\_connection

Describes a VPC connection.

Type annotations and code completion for `#!python session.create_client("quicksight").describe_vpc_connection` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.describe_vpc_connection)

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

kwargs: DescribeVPCConnectionRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "VPCConnectionId": ...,
}

parent.describe_vpc_connection(**kwargs)
```

1. See [:material-code-braces: DescribeVPCConnectionRequestRequestTypeDef](./type_defs.md#describevpcconnectionrequestrequesttypedef) 

### generate\_embed\_url\_for\_anonymous\_user

Generates an embed URL that you can use to embed an Amazon QuickSight dashboard
or visual in your website, without having to register any reader users.

Type annotations and code completion for `#!python session.create_client("quicksight").generate_embed_url_for_anonymous_user` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.generate_embed_url_for_anonymous_user)

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

kwargs: GenerateEmbedUrlForAnonymousUserRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "Namespace": ...,
    "AuthorizedResourceArns": ...,
    "ExperienceConfiguration": ...,
}

parent.generate_embed_url_for_anonymous_user(**kwargs)
```

1. See [:material-code-braces: GenerateEmbedUrlForAnonymousUserRequestRequestTypeDef](./type_defs.md#generateembedurlforanonymoususerrequestrequesttypedef) 

### generate\_embed\_url\_for\_registered\_user

Generates an embed URL that you can use to embed an Amazon QuickSight experience
in your website.

Type annotations and code completion for `#!python session.create_client("quicksight").generate_embed_url_for_registered_user` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.generate_embed_url_for_registered_user)

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

kwargs: GenerateEmbedUrlForRegisteredUserRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "UserArn": ...,
    "ExperienceConfiguration": ...,
}

parent.generate_embed_url_for_registered_user(**kwargs)
```

1. See [:material-code-braces: GenerateEmbedUrlForRegisteredUserRequestRequestTypeDef](./type_defs.md#generateembedurlforregistereduserrequestrequesttypedef) 

### generate\_presigned\_url

Generate a presigned url given a client, its method, and arguments.

Type annotations and code completion for `#!python session.create_client("quicksight").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.generate_presigned_url)

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


### get\_dashboard\_embed\_url

Generates a temporary session URL and authorization code(bearer token) that you
can use to embed an Amazon QuickSight read-only dashboard in your website or
application.

Type annotations and code completion for `#!python session.create_client("quicksight").get_dashboard_embed_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.get_dashboard_embed_url)

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

kwargs: GetDashboardEmbedUrlRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "DashboardId": ...,
    "IdentityType": ...,
}

parent.get_dashboard_embed_url(**kwargs)
```

1. See [:material-code-braces: GetDashboardEmbedUrlRequestRequestTypeDef](./type_defs.md#getdashboardembedurlrequestrequesttypedef) 

### get\_session\_embed\_url

Generates a session URL and authorization code that you can use to embed the
Amazon Amazon QuickSight console in your web server code.

Type annotations and code completion for `#!python session.create_client("quicksight").get_session_embed_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.get_session_embed_url)

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

kwargs: GetSessionEmbedUrlRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
}

parent.get_session_embed_url(**kwargs)
```

1. See [:material-code-braces: GetSessionEmbedUrlRequestRequestTypeDef](./type_defs.md#getsessionembedurlrequestrequesttypedef) 

### list\_analyses

Lists Amazon QuickSight analyses that exist in the specified Amazon Web Services
account.

Type annotations and code completion for `#!python session.create_client("quicksight").list_analyses` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.list_analyses)

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

kwargs: ListAnalysesRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
}

parent.list_analyses(**kwargs)
```

1. See [:material-code-braces: ListAnalysesRequestRequestTypeDef](./type_defs.md#listanalysesrequestrequesttypedef) 

### list\_asset\_bundle\_export\_jobs

Lists all asset bundle export jobs that have been taken place in the last 14
days.

Type annotations and code completion for `#!python session.create_client("quicksight").list_asset_bundle_export_jobs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.list_asset_bundle_export_jobs)

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

kwargs: ListAssetBundleExportJobsRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
}

parent.list_asset_bundle_export_jobs(**kwargs)
```

1. See [:material-code-braces: ListAssetBundleExportJobsRequestRequestTypeDef](./type_defs.md#listassetbundleexportjobsrequestrequesttypedef) 

### list\_asset\_bundle\_import\_jobs

Lists all asset bundle import jobs that have taken place in the last 14 days.

Type annotations and code completion for `#!python session.create_client("quicksight").list_asset_bundle_import_jobs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.list_asset_bundle_import_jobs)

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

kwargs: ListAssetBundleImportJobsRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
}

parent.list_asset_bundle_import_jobs(**kwargs)
```

1. See [:material-code-braces: ListAssetBundleImportJobsRequestRequestTypeDef](./type_defs.md#listassetbundleimportjobsrequestrequesttypedef) 

### list\_dashboard\_versions

Lists all the versions of the dashboards in the Amazon QuickSight subscription.

Type annotations and code completion for `#!python session.create_client("quicksight").list_dashboard_versions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.list_dashboard_versions)

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

kwargs: ListDashboardVersionsRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "DashboardId": ...,
}

parent.list_dashboard_versions(**kwargs)
```

1. See [:material-code-braces: ListDashboardVersionsRequestRequestTypeDef](./type_defs.md#listdashboardversionsrequestrequesttypedef) 

### list\_dashboards

Lists dashboards in an Amazon Web Services account.

Type annotations and code completion for `#!python session.create_client("quicksight").list_dashboards` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.list_dashboards)

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

kwargs: ListDashboardsRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
}

parent.list_dashboards(**kwargs)
```

1. See [:material-code-braces: ListDashboardsRequestRequestTypeDef](./type_defs.md#listdashboardsrequestrequesttypedef) 

### list\_data\_sets

Lists all of the datasets belonging to the current Amazon Web Services account
in an Amazon Web Services Region.

Type annotations and code completion for `#!python session.create_client("quicksight").list_data_sets` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.list_data_sets)

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

kwargs: ListDataSetsRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
}

parent.list_data_sets(**kwargs)
```

1. See [:material-code-braces: ListDataSetsRequestRequestTypeDef](./type_defs.md#listdatasetsrequestrequesttypedef) 

### list\_data\_sources

Lists data sources in current Amazon Web Services Region that belong to this
Amazon Web Services account.

Type annotations and code completion for `#!python session.create_client("quicksight").list_data_sources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.list_data_sources)

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

kwargs: ListDataSourcesRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
}

parent.list_data_sources(**kwargs)
```

1. See [:material-code-braces: ListDataSourcesRequestRequestTypeDef](./type_defs.md#listdatasourcesrequestrequesttypedef) 

### list\_folder\_members

List all assets ( `DASHBOARD`, `ANALYSIS`, and `DATASET`) in a folder.

Type annotations and code completion for `#!python session.create_client("quicksight").list_folder_members` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.list_folder_members)

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

kwargs: ListFolderMembersRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "FolderId": ...,
}

parent.list_folder_members(**kwargs)
```

1. See [:material-code-braces: ListFolderMembersRequestRequestTypeDef](./type_defs.md#listfoldermembersrequestrequesttypedef) 

### list\_folders

Lists all folders in an account.

Type annotations and code completion for `#!python session.create_client("quicksight").list_folders` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.list_folders)

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

kwargs: ListFoldersRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
}

parent.list_folders(**kwargs)
```

1. See [:material-code-braces: ListFoldersRequestRequestTypeDef](./type_defs.md#listfoldersrequestrequesttypedef) 

### list\_group\_memberships

Lists member users in a group.

Type annotations and code completion for `#!python session.create_client("quicksight").list_group_memberships` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.list_group_memberships)

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

kwargs: ListGroupMembershipsRequestRequestTypeDef = {  # (1)
    "GroupName": ...,
    "AwsAccountId": ...,
    "Namespace": ...,
}

parent.list_group_memberships(**kwargs)
```

1. See [:material-code-braces: ListGroupMembershipsRequestRequestTypeDef](./type_defs.md#listgroupmembershipsrequestrequesttypedef) 

### list\_groups

Lists all user groups in Amazon QuickSight.

Type annotations and code completion for `#!python session.create_client("quicksight").list_groups` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.list_groups)

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

kwargs: ListGroupsRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "Namespace": ...,
}

parent.list_groups(**kwargs)
```

1. See [:material-code-braces: ListGroupsRequestRequestTypeDef](./type_defs.md#listgroupsrequestrequesttypedef) 

### list\_iam\_policy\_assignments

Lists the IAM policy assignments in the current Amazon QuickSight account.

Type annotations and code completion for `#!python session.create_client("quicksight").list_iam_policy_assignments` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.list_iam_policy_assignments)

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

kwargs: ListIAMPolicyAssignmentsRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "Namespace": ...,
}

parent.list_iam_policy_assignments(**kwargs)
```

1. See [:material-code-braces: ListIAMPolicyAssignmentsRequestRequestTypeDef](./type_defs.md#listiampolicyassignmentsrequestrequesttypedef) 

### list\_iam\_policy\_assignments\_for\_user

Lists all of the IAM policy assignments, including the Amazon Resource Names
(ARNs), for the IAM policies assigned to the specified user and group, or groups
that the user belongs to.

Type annotations and code completion for `#!python session.create_client("quicksight").list_iam_policy_assignments_for_user` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.list_iam_policy_assignments_for_user)

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

kwargs: ListIAMPolicyAssignmentsForUserRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "UserName": ...,
    "Namespace": ...,
}

parent.list_iam_policy_assignments_for_user(**kwargs)
```

1. See [:material-code-braces: ListIAMPolicyAssignmentsForUserRequestRequestTypeDef](./type_defs.md#listiampolicyassignmentsforuserrequestrequesttypedef) 

### list\_ingestions

Lists the history of SPICE ingestions for a dataset.

Type annotations and code completion for `#!python session.create_client("quicksight").list_ingestions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.list_ingestions)

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

kwargs: ListIngestionsRequestRequestTypeDef = {  # (1)
    "DataSetId": ...,
    "AwsAccountId": ...,
}

parent.list_ingestions(**kwargs)
```

1. See [:material-code-braces: ListIngestionsRequestRequestTypeDef](./type_defs.md#listingestionsrequestrequesttypedef) 

### list\_namespaces

Lists the namespaces for the specified Amazon Web Services account.

Type annotations and code completion for `#!python session.create_client("quicksight").list_namespaces` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.list_namespaces)

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

kwargs: ListNamespacesRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
}

parent.list_namespaces(**kwargs)
```

1. See [:material-code-braces: ListNamespacesRequestRequestTypeDef](./type_defs.md#listnamespacesrequestrequesttypedef) 

### list\_refresh\_schedules

Lists the refresh schedules of a dataset.

Type annotations and code completion for `#!python session.create_client("quicksight").list_refresh_schedules` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.list_refresh_schedules)

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

kwargs: ListRefreshSchedulesRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "DataSetId": ...,
}

parent.list_refresh_schedules(**kwargs)
```

1. See [:material-code-braces: ListRefreshSchedulesRequestRequestTypeDef](./type_defs.md#listrefreshschedulesrequestrequesttypedef) 

### list\_tags\_for\_resource

Lists the tags assigned to a resource.

Type annotations and code completion for `#!python session.create_client("quicksight").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.list_tags_for_resource)

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

kwargs: ListTagsForResourceRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef) 

### list\_template\_aliases

Lists all the aliases of a template.

Type annotations and code completion for `#!python session.create_client("quicksight").list_template_aliases` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.list_template_aliases)

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

kwargs: ListTemplateAliasesRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "TemplateId": ...,
}

parent.list_template_aliases(**kwargs)
```

1. See [:material-code-braces: ListTemplateAliasesRequestRequestTypeDef](./type_defs.md#listtemplatealiasesrequestrequesttypedef) 

### list\_template\_versions

Lists all the versions of the templates in the current Amazon QuickSight
account.

Type annotations and code completion for `#!python session.create_client("quicksight").list_template_versions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.list_template_versions)

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

kwargs: ListTemplateVersionsRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "TemplateId": ...,
}

parent.list_template_versions(**kwargs)
```

1. See [:material-code-braces: ListTemplateVersionsRequestRequestTypeDef](./type_defs.md#listtemplateversionsrequestrequesttypedef) 

### list\_templates

Lists all the templates in the current Amazon QuickSight account.

Type annotations and code completion for `#!python session.create_client("quicksight").list_templates` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.list_templates)

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

kwargs: ListTemplatesRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
}

parent.list_templates(**kwargs)
```

1. See [:material-code-braces: ListTemplatesRequestRequestTypeDef](./type_defs.md#listtemplatesrequestrequesttypedef) 

### list\_theme\_aliases

Lists all the aliases of a theme.

Type annotations and code completion for `#!python session.create_client("quicksight").list_theme_aliases` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.list_theme_aliases)

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

kwargs: ListThemeAliasesRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "ThemeId": ...,
}

parent.list_theme_aliases(**kwargs)
```

1. See [:material-code-braces: ListThemeAliasesRequestRequestTypeDef](./type_defs.md#listthemealiasesrequestrequesttypedef) 

### list\_theme\_versions

Lists all the versions of the themes in the current Amazon Web Services account.

Type annotations and code completion for `#!python session.create_client("quicksight").list_theme_versions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.list_theme_versions)

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

kwargs: ListThemeVersionsRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "ThemeId": ...,
}

parent.list_theme_versions(**kwargs)
```

1. See [:material-code-braces: ListThemeVersionsRequestRequestTypeDef](./type_defs.md#listthemeversionsrequestrequesttypedef) 

### list\_themes

Lists all the themes in the current Amazon Web Services account.

Type annotations and code completion for `#!python session.create_client("quicksight").list_themes` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.list_themes)

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

kwargs: ListThemesRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
}

parent.list_themes(**kwargs)
```

1. See [:material-code-braces: ListThemesRequestRequestTypeDef](./type_defs.md#listthemesrequestrequesttypedef) 

### list\_topic\_refresh\_schedules

Lists all of the refresh schedules for a topic.

Type annotations and code completion for `#!python session.create_client("quicksight").list_topic_refresh_schedules` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.list_topic_refresh_schedules)

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

kwargs: ListTopicRefreshSchedulesRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "TopicId": ...,
}

parent.list_topic_refresh_schedules(**kwargs)
```

1. See [:material-code-braces: ListTopicRefreshSchedulesRequestRequestTypeDef](./type_defs.md#listtopicrefreshschedulesrequestrequesttypedef) 

### list\_topics

Lists all of the topics within an account.

Type annotations and code completion for `#!python session.create_client("quicksight").list_topics` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.list_topics)

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

kwargs: ListTopicsRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
}

parent.list_topics(**kwargs)
```

1. See [:material-code-braces: ListTopicsRequestRequestTypeDef](./type_defs.md#listtopicsrequestrequesttypedef) 

### list\_user\_groups

Lists the Amazon QuickSight groups that an Amazon QuickSight user is a member
of.

Type annotations and code completion for `#!python session.create_client("quicksight").list_user_groups` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.list_user_groups)

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

kwargs: ListUserGroupsRequestRequestTypeDef = {  # (1)
    "UserName": ...,
    "AwsAccountId": ...,
    "Namespace": ...,
}

parent.list_user_groups(**kwargs)
```

1. See [:material-code-braces: ListUserGroupsRequestRequestTypeDef](./type_defs.md#listusergroupsrequestrequesttypedef) 

### list\_users

Returns a list of all of the Amazon QuickSight users belonging to this account.

Type annotations and code completion for `#!python session.create_client("quicksight").list_users` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.list_users)

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

kwargs: ListUsersRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "Namespace": ...,
}

parent.list_users(**kwargs)
```

1. See [:material-code-braces: ListUsersRequestRequestTypeDef](./type_defs.md#listusersrequestrequesttypedef) 

### list\_vpc\_connections

Lists all of the VPC connections in the current set Amazon Web Services Region
of an Amazon Web Services account.

Type annotations and code completion for `#!python session.create_client("quicksight").list_vpc_connections` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.list_vpc_connections)

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

kwargs: ListVPCConnectionsRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
}

parent.list_vpc_connections(**kwargs)
```

1. See [:material-code-braces: ListVPCConnectionsRequestRequestTypeDef](./type_defs.md#listvpcconnectionsrequestrequesttypedef) 

### put\_data\_set\_refresh\_properties

Creates or updates the dataset refresh properties for the dataset.

Type annotations and code completion for `#!python session.create_client("quicksight").put_data_set_refresh_properties` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.put_data_set_refresh_properties)

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

kwargs: PutDataSetRefreshPropertiesRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "DataSetId": ...,
    "DataSetRefreshProperties": ...,
}

parent.put_data_set_refresh_properties(**kwargs)
```

1. See [:material-code-braces: PutDataSetRefreshPropertiesRequestRequestTypeDef](./type_defs.md#putdatasetrefreshpropertiesrequestrequesttypedef) 

### register\_user

Creates an Amazon QuickSight user whose identity is associated with the Identity
and Access Management (IAM) identity or role specified in the request.

Type annotations and code completion for `#!python session.create_client("quicksight").register_user` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.register_user)

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
) -> RegisterUserResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: IdentityTypeType](./literals.md#identitytypetype) 
2. See [:material-code-brackets: UserRoleType](./literals.md#userroletype) 
3. See [:material-code-braces: RegisterUserResponseTypeDef](./type_defs.md#registeruserresponsetypedef) 


```python
# register_user method usage example with argument unpacking

kwargs: RegisterUserRequestRequestTypeDef = {  # (1)
    "IdentityType": ...,
    "Email": ...,
    "UserRole": ...,
    "AwsAccountId": ...,
    "Namespace": ...,
}

parent.register_user(**kwargs)
```

1. See [:material-code-braces: RegisterUserRequestRequestTypeDef](./type_defs.md#registeruserrequestrequesttypedef) 

### restore\_analysis

Restores an analysis.

Type annotations and code completion for `#!python session.create_client("quicksight").restore_analysis` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.restore_analysis)

```python
# restore_analysis method definition

await def restore_analysis(
    self,
    *,
    AwsAccountId: str,
    AnalysisId: str,
) -> RestoreAnalysisResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: RestoreAnalysisResponseTypeDef](./type_defs.md#restoreanalysisresponsetypedef) 


```python
# restore_analysis method usage example with argument unpacking

kwargs: RestoreAnalysisRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "AnalysisId": ...,
}

parent.restore_analysis(**kwargs)
```

1. See [:material-code-braces: RestoreAnalysisRequestRequestTypeDef](./type_defs.md#restoreanalysisrequestrequesttypedef) 

### search\_analyses

Searches for analyses that belong to the user specified in the filter.

Type annotations and code completion for `#!python session.create_client("quicksight").search_analyses` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.search_analyses)

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

kwargs: SearchAnalysesRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "Filters": ...,
}

parent.search_analyses(**kwargs)
```

1. See [:material-code-braces: SearchAnalysesRequestRequestTypeDef](./type_defs.md#searchanalysesrequestrequesttypedef) 

### search\_dashboards

Searches for dashboards that belong to a user.

Type annotations and code completion for `#!python session.create_client("quicksight").search_dashboards` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.search_dashboards)

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

kwargs: SearchDashboardsRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "Filters": ...,
}

parent.search_dashboards(**kwargs)
```

1. See [:material-code-braces: SearchDashboardsRequestRequestTypeDef](./type_defs.md#searchdashboardsrequestrequesttypedef) 

### search\_data\_sets

Use the `SearchDataSets` operation to search for datasets that belong to an
account.

Type annotations and code completion for `#!python session.create_client("quicksight").search_data_sets` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.search_data_sets)

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

kwargs: SearchDataSetsRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "Filters": ...,
}

parent.search_data_sets(**kwargs)
```

1. See [:material-code-braces: SearchDataSetsRequestRequestTypeDef](./type_defs.md#searchdatasetsrequestrequesttypedef) 

### search\_data\_sources

Use the `SearchDataSources` operation to search for data sources that belong to
an account.

Type annotations and code completion for `#!python session.create_client("quicksight").search_data_sources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.search_data_sources)

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

kwargs: SearchDataSourcesRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "Filters": ...,
}

parent.search_data_sources(**kwargs)
```

1. See [:material-code-braces: SearchDataSourcesRequestRequestTypeDef](./type_defs.md#searchdatasourcesrequestrequesttypedef) 

### search\_folders

Searches the subfolders in a folder.

Type annotations and code completion for `#!python session.create_client("quicksight").search_folders` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.search_folders)

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

kwargs: SearchFoldersRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "Filters": ...,
}

parent.search_folders(**kwargs)
```

1. See [:material-code-braces: SearchFoldersRequestRequestTypeDef](./type_defs.md#searchfoldersrequestrequesttypedef) 

### search\_groups

Use the `SearchGroups` operation to search groups in a specified Amazon
QuickSight namespace using the supplied filters.

Type annotations and code completion for `#!python session.create_client("quicksight").search_groups` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.search_groups)

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

kwargs: SearchGroupsRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "Namespace": ...,
    "Filters": ...,
}

parent.search_groups(**kwargs)
```

1. See [:material-code-braces: SearchGroupsRequestRequestTypeDef](./type_defs.md#searchgroupsrequestrequesttypedef) 

### start\_asset\_bundle\_export\_job

Starts an Asset Bundle export job.

Type annotations and code completion for `#!python session.create_client("quicksight").start_asset_bundle_export_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.start_asset_bundle_export_job)

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
    CloudFormationOverridePropertyConfiguration: AssetBundleCloudFormationOverridePropertyConfigurationTypeDef = ...,  # (2)
) -> StartAssetBundleExportJobResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: AssetBundleExportFormatType](./literals.md#assetbundleexportformattype) 
2. See [:material-code-braces: AssetBundleCloudFormationOverridePropertyConfigurationTypeDef](./type_defs.md#assetbundlecloudformationoverridepropertyconfigurationtypedef) 
3. See [:material-code-braces: StartAssetBundleExportJobResponseTypeDef](./type_defs.md#startassetbundleexportjobresponsetypedef) 


```python
# start_asset_bundle_export_job method usage example with argument unpacking

kwargs: StartAssetBundleExportJobRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "AssetBundleExportJobId": ...,
    "ResourceArns": ...,
    "ExportFormat": ...,
}

parent.start_asset_bundle_export_job(**kwargs)
```

1. See [:material-code-braces: StartAssetBundleExportJobRequestRequestTypeDef](./type_defs.md#startassetbundleexportjobrequestrequesttypedef) 

### start\_asset\_bundle\_import\_job

Starts an Asset Bundle import job.

Type annotations and code completion for `#!python session.create_client("quicksight").start_asset_bundle_import_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.start_asset_bundle_import_job)

```python
# start_asset_bundle_import_job method definition

await def start_asset_bundle_import_job(
    self,
    *,
    AwsAccountId: str,
    AssetBundleImportJobId: str,
    AssetBundleImportSource: AssetBundleImportSourceTypeDef,  # (1)
    OverrideParameters: AssetBundleImportJobOverrideParametersTypeDef = ...,  # (2)
    FailureAction: AssetBundleImportFailureActionType = ...,  # (3)
) -> StartAssetBundleImportJobResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: AssetBundleImportSourceTypeDef](./type_defs.md#assetbundleimportsourcetypedef) 
2. See [:material-code-braces: AssetBundleImportJobOverrideParametersTypeDef](./type_defs.md#assetbundleimportjoboverrideparameterstypedef) 
3. See [:material-code-brackets: AssetBundleImportFailureActionType](./literals.md#assetbundleimportfailureactiontype) 
4. See [:material-code-braces: StartAssetBundleImportJobResponseTypeDef](./type_defs.md#startassetbundleimportjobresponsetypedef) 


```python
# start_asset_bundle_import_job method usage example with argument unpacking

kwargs: StartAssetBundleImportJobRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "AssetBundleImportJobId": ...,
    "AssetBundleImportSource": ...,
}

parent.start_asset_bundle_import_job(**kwargs)
```

1. See [:material-code-braces: StartAssetBundleImportJobRequestRequestTypeDef](./type_defs.md#startassetbundleimportjobrequestrequesttypedef) 

### start\_dashboard\_snapshot\_job

Starts an asynchronous job that generates a dashboard snapshot.

Type annotations and code completion for `#!python session.create_client("quicksight").start_dashboard_snapshot_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.start_dashboard_snapshot_job)

```python
# start_dashboard_snapshot_job method definition

await def start_dashboard_snapshot_job(
    self,
    *,
    AwsAccountId: str,
    DashboardId: str,
    SnapshotJobId: str,
    UserConfiguration: SnapshotUserConfigurationTypeDef,  # (1)
    SnapshotConfiguration: SnapshotConfigurationTypeDef,  # (2)
) -> StartDashboardSnapshotJobResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: SnapshotUserConfigurationTypeDef](./type_defs.md#snapshotuserconfigurationtypedef) 
2. See [:material-code-braces: SnapshotConfigurationTypeDef](./type_defs.md#snapshotconfigurationtypedef) 
3. See [:material-code-braces: StartDashboardSnapshotJobResponseTypeDef](./type_defs.md#startdashboardsnapshotjobresponsetypedef) 


```python
# start_dashboard_snapshot_job method usage example with argument unpacking

kwargs: StartDashboardSnapshotJobRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "DashboardId": ...,
    "SnapshotJobId": ...,
    "UserConfiguration": ...,
    "SnapshotConfiguration": ...,
}

parent.start_dashboard_snapshot_job(**kwargs)
```

1. See [:material-code-braces: StartDashboardSnapshotJobRequestRequestTypeDef](./type_defs.md#startdashboardsnapshotjobrequestrequesttypedef) 

### tag\_resource

Assigns one or more tags (key-value pairs) to the specified Amazon QuickSight
resource.

Type annotations and code completion for `#!python session.create_client("quicksight").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.tag_resource)

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

kwargs: TagResourceRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
    "Tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef) 

### untag\_resource

Removes a tag or tags from a resource.

Type annotations and code completion for `#!python session.create_client("quicksight").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.untag_resource)

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

kwargs: UntagResourceRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
    "TagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef) 

### update\_account\_customization

Updates Amazon QuickSight customizations for the current Amazon Web Services
Region.

Type annotations and code completion for `#!python session.create_client("quicksight").update_account_customization` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_account_customization)

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

kwargs: UpdateAccountCustomizationRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "AccountCustomization": ...,
}

parent.update_account_customization(**kwargs)
```

1. See [:material-code-braces: UpdateAccountCustomizationRequestRequestTypeDef](./type_defs.md#updateaccountcustomizationrequestrequesttypedef) 

### update\_account\_settings

Updates the Amazon QuickSight settings in your Amazon Web Services account.

Type annotations and code completion for `#!python session.create_client("quicksight").update_account_settings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_account_settings)

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

kwargs: UpdateAccountSettingsRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "DefaultNamespace": ...,
}

parent.update_account_settings(**kwargs)
```

1. See [:material-code-braces: UpdateAccountSettingsRequestRequestTypeDef](./type_defs.md#updateaccountsettingsrequestrequesttypedef) 

### update\_analysis

Updates an analysis in Amazon QuickSight See also: [AWS API
Documentation](https://docs.aws.amazon.com/goto/WebAPI/quicksight-2018-04-01/UpdateAnalysis).

Type annotations and code completion for `#!python session.create_client("quicksight").update_analysis` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_analysis)

```python
# update_analysis method definition

await def update_analysis(
    self,
    *,
    AwsAccountId: str,
    AnalysisId: str,
    Name: str,
    Parameters: ParametersTypeDef = ...,  # (1)
    SourceEntity: AnalysisSourceEntityTypeDef = ...,  # (2)
    ThemeArn: str = ...,
    Definition: AnalysisDefinitionTypeDef = ...,  # (3)
) -> UpdateAnalysisResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: ParametersTypeDef](./type_defs.md#parameterstypedef) 
2. See [:material-code-braces: AnalysisSourceEntityTypeDef](./type_defs.md#analysissourceentitytypedef) 
3. See [:material-code-braces: AnalysisDefinitionTypeDef](./type_defs.md#analysisdefinitiontypedef) 
4. See [:material-code-braces: UpdateAnalysisResponseTypeDef](./type_defs.md#updateanalysisresponsetypedef) 


```python
# update_analysis method usage example with argument unpacking

kwargs: UpdateAnalysisRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "AnalysisId": ...,
    "Name": ...,
}

parent.update_analysis(**kwargs)
```

1. See [:material-code-braces: UpdateAnalysisRequestRequestTypeDef](./type_defs.md#updateanalysisrequestrequesttypedef) 

### update\_analysis\_permissions

Updates the read and write permissions for an analysis.

Type annotations and code completion for `#!python session.create_client("quicksight").update_analysis_permissions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_analysis_permissions)

```python
# update_analysis_permissions method definition

await def update_analysis_permissions(
    self,
    *,
    AwsAccountId: str,
    AnalysisId: str,
    GrantPermissions: Sequence[ResourcePermissionTypeDef] = ...,  # (1)
    RevokePermissions: Sequence[ResourcePermissionTypeDef] = ...,  # (1)
) -> UpdateAnalysisPermissionsResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: ResourcePermissionTypeDef](./type_defs.md#resourcepermissiontypedef) 
2. See [:material-code-braces: ResourcePermissionTypeDef](./type_defs.md#resourcepermissiontypedef) 
3. See [:material-code-braces: UpdateAnalysisPermissionsResponseTypeDef](./type_defs.md#updateanalysispermissionsresponsetypedef) 


```python
# update_analysis_permissions method usage example with argument unpacking

kwargs: UpdateAnalysisPermissionsRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "AnalysisId": ...,
}

parent.update_analysis_permissions(**kwargs)
```

1. See [:material-code-braces: UpdateAnalysisPermissionsRequestRequestTypeDef](./type_defs.md#updateanalysispermissionsrequestrequesttypedef) 

### update\_dashboard

Updates a dashboard in an Amazon Web Services account.

Type annotations and code completion for `#!python session.create_client("quicksight").update_dashboard` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_dashboard)

```python
# update_dashboard method definition

await def update_dashboard(
    self,
    *,
    AwsAccountId: str,
    DashboardId: str,
    Name: str,
    SourceEntity: DashboardSourceEntityTypeDef = ...,  # (1)
    Parameters: ParametersTypeDef = ...,  # (2)
    VersionDescription: str = ...,
    DashboardPublishOptions: DashboardPublishOptionsTypeDef = ...,  # (3)
    ThemeArn: str = ...,
    Definition: DashboardVersionDefinitionTypeDef = ...,  # (4)
) -> UpdateDashboardResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-braces: DashboardSourceEntityTypeDef](./type_defs.md#dashboardsourceentitytypedef) 
2. See [:material-code-braces: ParametersTypeDef](./type_defs.md#parameterstypedef) 
3. See [:material-code-braces: DashboardPublishOptionsTypeDef](./type_defs.md#dashboardpublishoptionstypedef) 
4. See [:material-code-braces: DashboardVersionDefinitionTypeDef](./type_defs.md#dashboardversiondefinitiontypedef) 
5. See [:material-code-braces: UpdateDashboardResponseTypeDef](./type_defs.md#updatedashboardresponsetypedef) 


```python
# update_dashboard method usage example with argument unpacking

kwargs: UpdateDashboardRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "DashboardId": ...,
    "Name": ...,
}

parent.update_dashboard(**kwargs)
```

1. See [:material-code-braces: UpdateDashboardRequestRequestTypeDef](./type_defs.md#updatedashboardrequestrequesttypedef) 

### update\_dashboard\_permissions

Updates read and write permissions on a dashboard.

Type annotations and code completion for `#!python session.create_client("quicksight").update_dashboard_permissions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_dashboard_permissions)

```python
# update_dashboard_permissions method definition

await def update_dashboard_permissions(
    self,
    *,
    AwsAccountId: str,
    DashboardId: str,
    GrantPermissions: Sequence[ResourcePermissionTypeDef] = ...,  # (1)
    RevokePermissions: Sequence[ResourcePermissionTypeDef] = ...,  # (1)
    GrantLinkPermissions: Sequence[ResourcePermissionTypeDef] = ...,  # (1)
    RevokeLinkPermissions: Sequence[ResourcePermissionTypeDef] = ...,  # (1)
) -> UpdateDashboardPermissionsResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-braces: ResourcePermissionTypeDef](./type_defs.md#resourcepermissiontypedef) 
2. See [:material-code-braces: ResourcePermissionTypeDef](./type_defs.md#resourcepermissiontypedef) 
3. See [:material-code-braces: ResourcePermissionTypeDef](./type_defs.md#resourcepermissiontypedef) 
4. See [:material-code-braces: ResourcePermissionTypeDef](./type_defs.md#resourcepermissiontypedef) 
5. See [:material-code-braces: UpdateDashboardPermissionsResponseTypeDef](./type_defs.md#updatedashboardpermissionsresponsetypedef) 


```python
# update_dashboard_permissions method usage example with argument unpacking

kwargs: UpdateDashboardPermissionsRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "DashboardId": ...,
}

parent.update_dashboard_permissions(**kwargs)
```

1. See [:material-code-braces: UpdateDashboardPermissionsRequestRequestTypeDef](./type_defs.md#updatedashboardpermissionsrequestrequesttypedef) 

### update\_dashboard\_published\_version

Updates the published version of a dashboard.

Type annotations and code completion for `#!python session.create_client("quicksight").update_dashboard_published_version` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_dashboard_published_version)

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

kwargs: UpdateDashboardPublishedVersionRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "DashboardId": ...,
    "VersionNumber": ...,
}

parent.update_dashboard_published_version(**kwargs)
```

1. See [:material-code-braces: UpdateDashboardPublishedVersionRequestRequestTypeDef](./type_defs.md#updatedashboardpublishedversionrequestrequesttypedef) 

### update\_data\_set

Updates a dataset.

Type annotations and code completion for `#!python session.create_client("quicksight").update_data_set` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_data_set)

```python
# update_data_set method definition

await def update_data_set(
    self,
    *,
    AwsAccountId: str,
    DataSetId: str,
    Name: str,
    PhysicalTableMap: Mapping[str, PhysicalTableTypeDef],  # (1)
    ImportMode: DataSetImportModeType,  # (2)
    LogicalTableMap: Mapping[str, LogicalTableTypeDef] = ...,  # (3)
    ColumnGroups: Sequence[ColumnGroupTypeDef] = ...,  # (4)
    FieldFolders: Mapping[str, FieldFolderTypeDef] = ...,  # (5)
    RowLevelPermissionDataSet: RowLevelPermissionDataSetTypeDef = ...,  # (6)
    RowLevelPermissionTagConfiguration: RowLevelPermissionTagConfigurationTypeDef = ...,  # (7)
    ColumnLevelPermissionRules: Sequence[ColumnLevelPermissionRuleTypeDef] = ...,  # (8)
    DataSetUsageConfiguration: DataSetUsageConfigurationTypeDef = ...,  # (9)
    DatasetParameters: Sequence[DatasetParameterTypeDef] = ...,  # (10)
) -> UpdateDataSetResponseTypeDef:  # (11)
    ...
```

1. See [:material-code-braces: PhysicalTableTypeDef](./type_defs.md#physicaltabletypedef) 
2. See [:material-code-brackets: DataSetImportModeType](./literals.md#datasetimportmodetype) 
3. See [:material-code-braces: LogicalTableTypeDef](./type_defs.md#logicaltabletypedef) 
4. See [:material-code-braces: ColumnGroupTypeDef](./type_defs.md#columngrouptypedef) 
5. See [:material-code-braces: FieldFolderTypeDef](./type_defs.md#fieldfoldertypedef) 
6. See [:material-code-braces: RowLevelPermissionDataSetTypeDef](./type_defs.md#rowlevelpermissiondatasettypedef) 
7. See [:material-code-braces: RowLevelPermissionTagConfigurationTypeDef](./type_defs.md#rowlevelpermissiontagconfigurationtypedef) 
8. See [:material-code-braces: ColumnLevelPermissionRuleTypeDef](./type_defs.md#columnlevelpermissionruletypedef) 
9. See [:material-code-braces: DataSetUsageConfigurationTypeDef](./type_defs.md#datasetusageconfigurationtypedef) 
10. See [:material-code-braces: DatasetParameterTypeDef](./type_defs.md#datasetparametertypedef) 
11. See [:material-code-braces: UpdateDataSetResponseTypeDef](./type_defs.md#updatedatasetresponsetypedef) 


```python
# update_data_set method usage example with argument unpacking

kwargs: UpdateDataSetRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "DataSetId": ...,
    "Name": ...,
    "PhysicalTableMap": ...,
    "ImportMode": ...,
}

parent.update_data_set(**kwargs)
```

1. See [:material-code-braces: UpdateDataSetRequestRequestTypeDef](./type_defs.md#updatedatasetrequestrequesttypedef) 

### update\_data\_set\_permissions

Updates the permissions on a dataset.

Type annotations and code completion for `#!python session.create_client("quicksight").update_data_set_permissions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_data_set_permissions)

```python
# update_data_set_permissions method definition

await def update_data_set_permissions(
    self,
    *,
    AwsAccountId: str,
    DataSetId: str,
    GrantPermissions: Sequence[ResourcePermissionTypeDef] = ...,  # (1)
    RevokePermissions: Sequence[ResourcePermissionTypeDef] = ...,  # (1)
) -> UpdateDataSetPermissionsResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: ResourcePermissionTypeDef](./type_defs.md#resourcepermissiontypedef) 
2. See [:material-code-braces: ResourcePermissionTypeDef](./type_defs.md#resourcepermissiontypedef) 
3. See [:material-code-braces: UpdateDataSetPermissionsResponseTypeDef](./type_defs.md#updatedatasetpermissionsresponsetypedef) 


```python
# update_data_set_permissions method usage example with argument unpacking

kwargs: UpdateDataSetPermissionsRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "DataSetId": ...,
}

parent.update_data_set_permissions(**kwargs)
```

1. See [:material-code-braces: UpdateDataSetPermissionsRequestRequestTypeDef](./type_defs.md#updatedatasetpermissionsrequestrequesttypedef) 

### update\_data\_source

Updates a data source.

Type annotations and code completion for `#!python session.create_client("quicksight").update_data_source` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_data_source)

```python
# update_data_source method definition

await def update_data_source(
    self,
    *,
    AwsAccountId: str,
    DataSourceId: str,
    Name: str,
    DataSourceParameters: DataSourceParametersTypeDef = ...,  # (1)
    Credentials: DataSourceCredentialsTypeDef = ...,  # (2)
    VpcConnectionProperties: VpcConnectionPropertiesTypeDef = ...,  # (3)
    SslProperties: SslPropertiesTypeDef = ...,  # (4)
) -> UpdateDataSourceResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-braces: DataSourceParametersTypeDef](./type_defs.md#datasourceparameterstypedef) 
2. See [:material-code-braces: DataSourceCredentialsTypeDef](./type_defs.md#datasourcecredentialstypedef) 
3. See [:material-code-braces: VpcConnectionPropertiesTypeDef](./type_defs.md#vpcconnectionpropertiestypedef) 
4. See [:material-code-braces: SslPropertiesTypeDef](./type_defs.md#sslpropertiestypedef) 
5. See [:material-code-braces: UpdateDataSourceResponseTypeDef](./type_defs.md#updatedatasourceresponsetypedef) 


```python
# update_data_source method usage example with argument unpacking

kwargs: UpdateDataSourceRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "DataSourceId": ...,
    "Name": ...,
}

parent.update_data_source(**kwargs)
```

1. See [:material-code-braces: UpdateDataSourceRequestRequestTypeDef](./type_defs.md#updatedatasourcerequestrequesttypedef) 

### update\_data\_source\_permissions

Updates the permissions to a data source.

Type annotations and code completion for `#!python session.create_client("quicksight").update_data_source_permissions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_data_source_permissions)

```python
# update_data_source_permissions method definition

await def update_data_source_permissions(
    self,
    *,
    AwsAccountId: str,
    DataSourceId: str,
    GrantPermissions: Sequence[ResourcePermissionTypeDef] = ...,  # (1)
    RevokePermissions: Sequence[ResourcePermissionTypeDef] = ...,  # (1)
) -> UpdateDataSourcePermissionsResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: ResourcePermissionTypeDef](./type_defs.md#resourcepermissiontypedef) 
2. See [:material-code-braces: ResourcePermissionTypeDef](./type_defs.md#resourcepermissiontypedef) 
3. See [:material-code-braces: UpdateDataSourcePermissionsResponseTypeDef](./type_defs.md#updatedatasourcepermissionsresponsetypedef) 


```python
# update_data_source_permissions method usage example with argument unpacking

kwargs: UpdateDataSourcePermissionsRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "DataSourceId": ...,
}

parent.update_data_source_permissions(**kwargs)
```

1. See [:material-code-braces: UpdateDataSourcePermissionsRequestRequestTypeDef](./type_defs.md#updatedatasourcepermissionsrequestrequesttypedef) 

### update\_folder

Updates the name of a folder.

Type annotations and code completion for `#!python session.create_client("quicksight").update_folder` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_folder)

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

kwargs: UpdateFolderRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "FolderId": ...,
    "Name": ...,
}

parent.update_folder(**kwargs)
```

1. See [:material-code-braces: UpdateFolderRequestRequestTypeDef](./type_defs.md#updatefolderrequestrequesttypedef) 

### update\_folder\_permissions

Updates permissions of a folder.

Type annotations and code completion for `#!python session.create_client("quicksight").update_folder_permissions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_folder_permissions)

```python
# update_folder_permissions method definition

await def update_folder_permissions(
    self,
    *,
    AwsAccountId: str,
    FolderId: str,
    GrantPermissions: Sequence[ResourcePermissionTypeDef] = ...,  # (1)
    RevokePermissions: Sequence[ResourcePermissionTypeDef] = ...,  # (1)
) -> UpdateFolderPermissionsResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: ResourcePermissionTypeDef](./type_defs.md#resourcepermissiontypedef) 
2. See [:material-code-braces: ResourcePermissionTypeDef](./type_defs.md#resourcepermissiontypedef) 
3. See [:material-code-braces: UpdateFolderPermissionsResponseTypeDef](./type_defs.md#updatefolderpermissionsresponsetypedef) 


```python
# update_folder_permissions method usage example with argument unpacking

kwargs: UpdateFolderPermissionsRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "FolderId": ...,
}

parent.update_folder_permissions(**kwargs)
```

1. See [:material-code-braces: UpdateFolderPermissionsRequestRequestTypeDef](./type_defs.md#updatefolderpermissionsrequestrequesttypedef) 

### update\_group

Changes a group description.

Type annotations and code completion for `#!python session.create_client("quicksight").update_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_group)

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

kwargs: UpdateGroupRequestRequestTypeDef = {  # (1)
    "GroupName": ...,
    "AwsAccountId": ...,
    "Namespace": ...,
}

parent.update_group(**kwargs)
```

1. See [:material-code-braces: UpdateGroupRequestRequestTypeDef](./type_defs.md#updategrouprequestrequesttypedef) 

### update\_iam\_policy\_assignment

Updates an existing IAM policy assignment.

Type annotations and code completion for `#!python session.create_client("quicksight").update_iam_policy_assignment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_iam_policy_assignment)

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

kwargs: UpdateIAMPolicyAssignmentRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "AssignmentName": ...,
    "Namespace": ...,
}

parent.update_iam_policy_assignment(**kwargs)
```

1. See [:material-code-braces: UpdateIAMPolicyAssignmentRequestRequestTypeDef](./type_defs.md#updateiampolicyassignmentrequestrequesttypedef) 

### update\_ip\_restriction

Updates the content and status of IP rules.

Type annotations and code completion for `#!python session.create_client("quicksight").update_ip_restriction` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_ip_restriction)

```python
# update_ip_restriction method definition

await def update_ip_restriction(
    self,
    *,
    AwsAccountId: str,
    IpRestrictionRuleMap: Mapping[str, str] = ...,
    Enabled: bool = ...,
) -> UpdateIpRestrictionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateIpRestrictionResponseTypeDef](./type_defs.md#updateiprestrictionresponsetypedef) 


```python
# update_ip_restriction method usage example with argument unpacking

kwargs: UpdateIpRestrictionRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
}

parent.update_ip_restriction(**kwargs)
```

1. See [:material-code-braces: UpdateIpRestrictionRequestRequestTypeDef](./type_defs.md#updateiprestrictionrequestrequesttypedef) 

### update\_public\_sharing\_settings

Use the `UpdatePublicSharingSettings` operation to turn on or turn off the
public sharing settings of an Amazon QuickSight dashboard.

Type annotations and code completion for `#!python session.create_client("quicksight").update_public_sharing_settings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_public_sharing_settings)

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

kwargs: UpdatePublicSharingSettingsRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
}

parent.update_public_sharing_settings(**kwargs)
```

1. See [:material-code-braces: UpdatePublicSharingSettingsRequestRequestTypeDef](./type_defs.md#updatepublicsharingsettingsrequestrequesttypedef) 

### update\_refresh\_schedule

Updates a refresh schedule for a dataset.

Type annotations and code completion for `#!python session.create_client("quicksight").update_refresh_schedule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_refresh_schedule)

```python
# update_refresh_schedule method definition

await def update_refresh_schedule(
    self,
    *,
    DataSetId: str,
    AwsAccountId: str,
    Schedule: RefreshScheduleTypeDef,  # (1)
) -> UpdateRefreshScheduleResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: RefreshScheduleTypeDef](./type_defs.md#refreshscheduletypedef) 
2. See [:material-code-braces: UpdateRefreshScheduleResponseTypeDef](./type_defs.md#updaterefreshscheduleresponsetypedef) 


```python
# update_refresh_schedule method usage example with argument unpacking

kwargs: UpdateRefreshScheduleRequestRequestTypeDef = {  # (1)
    "DataSetId": ...,
    "AwsAccountId": ...,
    "Schedule": ...,
}

parent.update_refresh_schedule(**kwargs)
```

1. See [:material-code-braces: UpdateRefreshScheduleRequestRequestTypeDef](./type_defs.md#updaterefreshschedulerequestrequesttypedef) 

### update\_template

Updates a template from an existing Amazon QuickSight analysis or another
template.

Type annotations and code completion for `#!python session.create_client("quicksight").update_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_template)

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
    Definition: TemplateVersionDefinitionTypeDef = ...,  # (2)
) -> UpdateTemplateResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: TemplateSourceEntityTypeDef](./type_defs.md#templatesourceentitytypedef) 
2. See [:material-code-braces: TemplateVersionDefinitionTypeDef](./type_defs.md#templateversiondefinitiontypedef) 
3. See [:material-code-braces: UpdateTemplateResponseTypeDef](./type_defs.md#updatetemplateresponsetypedef) 


```python
# update_template method usage example with argument unpacking

kwargs: UpdateTemplateRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "TemplateId": ...,
}

parent.update_template(**kwargs)
```

1. See [:material-code-braces: UpdateTemplateRequestRequestTypeDef](./type_defs.md#updatetemplaterequestrequesttypedef) 

### update\_template\_alias

Updates the template alias of a template.

Type annotations and code completion for `#!python session.create_client("quicksight").update_template_alias` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_template_alias)

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

kwargs: UpdateTemplateAliasRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "TemplateId": ...,
    "AliasName": ...,
    "TemplateVersionNumber": ...,
}

parent.update_template_alias(**kwargs)
```

1. See [:material-code-braces: UpdateTemplateAliasRequestRequestTypeDef](./type_defs.md#updatetemplatealiasrequestrequesttypedef) 

### update\_template\_permissions

Updates the resource permissions for a template.

Type annotations and code completion for `#!python session.create_client("quicksight").update_template_permissions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_template_permissions)

```python
# update_template_permissions method definition

await def update_template_permissions(
    self,
    *,
    AwsAccountId: str,
    TemplateId: str,
    GrantPermissions: Sequence[ResourcePermissionTypeDef] = ...,  # (1)
    RevokePermissions: Sequence[ResourcePermissionTypeDef] = ...,  # (1)
) -> UpdateTemplatePermissionsResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: ResourcePermissionTypeDef](./type_defs.md#resourcepermissiontypedef) 
2. See [:material-code-braces: ResourcePermissionTypeDef](./type_defs.md#resourcepermissiontypedef) 
3. See [:material-code-braces: UpdateTemplatePermissionsResponseTypeDef](./type_defs.md#updatetemplatepermissionsresponsetypedef) 


```python
# update_template_permissions method usage example with argument unpacking

kwargs: UpdateTemplatePermissionsRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "TemplateId": ...,
}

parent.update_template_permissions(**kwargs)
```

1. See [:material-code-braces: UpdateTemplatePermissionsRequestRequestTypeDef](./type_defs.md#updatetemplatepermissionsrequestrequesttypedef) 

### update\_theme

Updates a theme.

Type annotations and code completion for `#!python session.create_client("quicksight").update_theme` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_theme)

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
    Configuration: ThemeConfigurationTypeDef = ...,  # (1)
) -> UpdateThemeResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ThemeConfigurationTypeDef](./type_defs.md#themeconfigurationtypedef) 
2. See [:material-code-braces: UpdateThemeResponseTypeDef](./type_defs.md#updatethemeresponsetypedef) 


```python
# update_theme method usage example with argument unpacking

kwargs: UpdateThemeRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "ThemeId": ...,
    "BaseThemeId": ...,
}

parent.update_theme(**kwargs)
```

1. See [:material-code-braces: UpdateThemeRequestRequestTypeDef](./type_defs.md#updatethemerequestrequesttypedef) 

### update\_theme\_alias

Updates an alias of a theme.

Type annotations and code completion for `#!python session.create_client("quicksight").update_theme_alias` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_theme_alias)

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

kwargs: UpdateThemeAliasRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "ThemeId": ...,
    "AliasName": ...,
    "ThemeVersionNumber": ...,
}

parent.update_theme_alias(**kwargs)
```

1. See [:material-code-braces: UpdateThemeAliasRequestRequestTypeDef](./type_defs.md#updatethemealiasrequestrequesttypedef) 

### update\_theme\_permissions

Updates the resource permissions for a theme.

Type annotations and code completion for `#!python session.create_client("quicksight").update_theme_permissions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_theme_permissions)

```python
# update_theme_permissions method definition

await def update_theme_permissions(
    self,
    *,
    AwsAccountId: str,
    ThemeId: str,
    GrantPermissions: Sequence[ResourcePermissionTypeDef] = ...,  # (1)
    RevokePermissions: Sequence[ResourcePermissionTypeDef] = ...,  # (1)
) -> UpdateThemePermissionsResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: ResourcePermissionTypeDef](./type_defs.md#resourcepermissiontypedef) 
2. See [:material-code-braces: ResourcePermissionTypeDef](./type_defs.md#resourcepermissiontypedef) 
3. See [:material-code-braces: UpdateThemePermissionsResponseTypeDef](./type_defs.md#updatethemepermissionsresponsetypedef) 


```python
# update_theme_permissions method usage example with argument unpacking

kwargs: UpdateThemePermissionsRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "ThemeId": ...,
}

parent.update_theme_permissions(**kwargs)
```

1. See [:material-code-braces: UpdateThemePermissionsRequestRequestTypeDef](./type_defs.md#updatethemepermissionsrequestrequesttypedef) 

### update\_topic

Updates a topic.

Type annotations and code completion for `#!python session.create_client("quicksight").update_topic` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_topic)

```python
# update_topic method definition

await def update_topic(
    self,
    *,
    AwsAccountId: str,
    TopicId: str,
    Topic: TopicDetailsTypeDef,  # (1)
) -> UpdateTopicResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TopicDetailsTypeDef](./type_defs.md#topicdetailstypedef) 
2. See [:material-code-braces: UpdateTopicResponseTypeDef](./type_defs.md#updatetopicresponsetypedef) 


```python
# update_topic method usage example with argument unpacking

kwargs: UpdateTopicRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "TopicId": ...,
    "Topic": ...,
}

parent.update_topic(**kwargs)
```

1. See [:material-code-braces: UpdateTopicRequestRequestTypeDef](./type_defs.md#updatetopicrequestrequesttypedef) 

### update\_topic\_permissions

Updates the permissions of a topic.

Type annotations and code completion for `#!python session.create_client("quicksight").update_topic_permissions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_topic_permissions)

```python
# update_topic_permissions method definition

await def update_topic_permissions(
    self,
    *,
    AwsAccountId: str,
    TopicId: str,
    GrantPermissions: Sequence[ResourcePermissionTypeDef] = ...,  # (1)
    RevokePermissions: Sequence[ResourcePermissionTypeDef] = ...,  # (1)
) -> UpdateTopicPermissionsResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: ResourcePermissionTypeDef](./type_defs.md#resourcepermissiontypedef) 
2. See [:material-code-braces: ResourcePermissionTypeDef](./type_defs.md#resourcepermissiontypedef) 
3. See [:material-code-braces: UpdateTopicPermissionsResponseTypeDef](./type_defs.md#updatetopicpermissionsresponsetypedef) 


```python
# update_topic_permissions method usage example with argument unpacking

kwargs: UpdateTopicPermissionsRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "TopicId": ...,
}

parent.update_topic_permissions(**kwargs)
```

1. See [:material-code-braces: UpdateTopicPermissionsRequestRequestTypeDef](./type_defs.md#updatetopicpermissionsrequestrequesttypedef) 

### update\_topic\_refresh\_schedule

Updates a topic refresh schedule.

Type annotations and code completion for `#!python session.create_client("quicksight").update_topic_refresh_schedule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_topic_refresh_schedule)

```python
# update_topic_refresh_schedule method definition

await def update_topic_refresh_schedule(
    self,
    *,
    AwsAccountId: str,
    TopicId: str,
    DatasetId: str,
    RefreshSchedule: TopicRefreshScheduleTypeDef,  # (1)
) -> UpdateTopicRefreshScheduleResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TopicRefreshScheduleTypeDef](./type_defs.md#topicrefreshscheduletypedef) 
2. See [:material-code-braces: UpdateTopicRefreshScheduleResponseTypeDef](./type_defs.md#updatetopicrefreshscheduleresponsetypedef) 


```python
# update_topic_refresh_schedule method usage example with argument unpacking

kwargs: UpdateTopicRefreshScheduleRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "TopicId": ...,
    "DatasetId": ...,
    "RefreshSchedule": ...,
}

parent.update_topic_refresh_schedule(**kwargs)
```

1. See [:material-code-braces: UpdateTopicRefreshScheduleRequestRequestTypeDef](./type_defs.md#updatetopicrefreshschedulerequestrequesttypedef) 

### update\_user

Updates an Amazon QuickSight user.

Type annotations and code completion for `#!python session.create_client("quicksight").update_user` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_user)

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

kwargs: UpdateUserRequestRequestTypeDef = {  # (1)
    "UserName": ...,
    "AwsAccountId": ...,
    "Namespace": ...,
    "Email": ...,
    "Role": ...,
}

parent.update_user(**kwargs)
```

1. See [:material-code-braces: UpdateUserRequestRequestTypeDef](./type_defs.md#updateuserrequestrequesttypedef) 

### update\_vpc\_connection

Updates a VPC connection.

Type annotations and code completion for `#!python session.create_client("quicksight").update_vpc_connection` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_vpc_connection)

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

kwargs: UpdateVPCConnectionRequestRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "VPCConnectionId": ...,
    "Name": ...,
    "SubnetIds": ...,
    "SecurityGroupIds": ...,
    "RoleArn": ...,
}

parent.update_vpc_connection(**kwargs)
```

1. See [:material-code-braces: UpdateVPCConnectionRequestRequestTypeDef](./type_defs.md#updatevpcconnectionrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("quicksight").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.__aenter__)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> QuickSightClient:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("quicksight").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.__aexit__)

```python
# __aexit__ method definition

await def __aexit__(
    self,
    exc_type: Any,
    exc_val: Any,
    exc_tb: Any,
) -> Any:
    ...
```




### get_paginator

Type annotations and code completion for `#!python session.create_client("quicksight").get_paginator` method with overloads.

- `client.get_paginator("list_analyses")` -> [ListAnalysesPaginator](./paginators.md#listanalysespaginator)
- `client.get_paginator("list_asset_bundle_export_jobs")` -> [ListAssetBundleExportJobsPaginator](./paginators.md#listassetbundleexportjobspaginator)
- `client.get_paginator("list_asset_bundle_import_jobs")` -> [ListAssetBundleImportJobsPaginator](./paginators.md#listassetbundleimportjobspaginator)
- `client.get_paginator("list_dashboard_versions")` -> [ListDashboardVersionsPaginator](./paginators.md#listdashboardversionspaginator)
- `client.get_paginator("list_dashboards")` -> [ListDashboardsPaginator](./paginators.md#listdashboardspaginator)
- `client.get_paginator("list_data_sets")` -> [ListDataSetsPaginator](./paginators.md#listdatasetspaginator)
- `client.get_paginator("list_data_sources")` -> [ListDataSourcesPaginator](./paginators.md#listdatasourcespaginator)
- `client.get_paginator("list_group_memberships")` -> [ListGroupMembershipsPaginator](./paginators.md#listgroupmembershipspaginator)
- `client.get_paginator("list_groups")` -> [ListGroupsPaginator](./paginators.md#listgroupspaginator)
- `client.get_paginator("list_iam_policy_assignments")` -> [ListIAMPolicyAssignmentsPaginator](./paginators.md#listiampolicyassignmentspaginator)
- `client.get_paginator("list_iam_policy_assignments_for_user")` -> [ListIAMPolicyAssignmentsForUserPaginator](./paginators.md#listiampolicyassignmentsforuserpaginator)
- `client.get_paginator("list_ingestions")` -> [ListIngestionsPaginator](./paginators.md#listingestionspaginator)
- `client.get_paginator("list_namespaces")` -> [ListNamespacesPaginator](./paginators.md#listnamespacespaginator)
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
- `client.get_paginator("search_groups")` -> [SearchGroupsPaginator](./paginators.md#searchgroupspaginator)



