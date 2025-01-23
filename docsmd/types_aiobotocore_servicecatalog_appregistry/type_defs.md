# Type definitions

> [Index](../README.md) > [AppRegistry](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [AppRegistry](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry.html#appregistry)
    type annotations stubs module [types-aiobotocore-servicecatalog-appregistry](https://pypi.org/project/types-aiobotocore-servicecatalog-appregistry/).



## TagQueryConfigurationTypeDef

```python
# TagQueryConfigurationTypeDef definition

class TagQueryConfigurationTypeDef(TypedDict):
    tagKey: NotRequired[str],
```

## ApplicationSummaryTypeDef

```python
# ApplicationSummaryTypeDef definition

class ApplicationSummaryTypeDef(TypedDict):
    id: NotRequired[str],
    arn: NotRequired[str],
    name: NotRequired[str],
    description: NotRequired[str],
    creationTime: NotRequired[datetime],
    lastUpdateTime: NotRequired[datetime],
```

## ResourcesListItemTypeDef

```python
# ResourcesListItemTypeDef definition

class ResourcesListItemTypeDef(TypedDict):
    resourceArn: NotRequired[str],
    errorMessage: NotRequired[str],
    status: NotRequired[str],
    resourceType: NotRequired[str],
```

## ApplicationTypeDef

```python
# ApplicationTypeDef definition

class ApplicationTypeDef(TypedDict):
    id: NotRequired[str],
    arn: NotRequired[str],
    name: NotRequired[str],
    description: NotRequired[str],
    creationTime: NotRequired[datetime],
    lastUpdateTime: NotRequired[datetime],
    tags: NotRequired[Dict[str, str]],
    applicationTag: NotRequired[Dict[str, str]],
```

## AssociateAttributeGroupRequestRequestTypeDef

```python
# AssociateAttributeGroupRequestRequestTypeDef definition

class AssociateAttributeGroupRequestRequestTypeDef(TypedDict):
    application: str,
    attributeGroup: str,
```

## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef definition

class ResponseMetadataTypeDef(TypedDict):
    RequestId: str,
    HTTPStatusCode: int,
    HTTPHeaders: Dict[str, str],
    RetryAttempts: int,
    HostId: NotRequired[str],
```

## AssociateResourceRequestRequestTypeDef

```python
# AssociateResourceRequestRequestTypeDef definition

class AssociateResourceRequestRequestTypeDef(TypedDict):
    application: str,
    resourceType: ResourceTypeType,  # (1)
    resource: str,
    options: NotRequired[Sequence[AssociationOptionType]],  # (2)
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
2. See [:material-code-brackets: AssociationOptionType](./literals.md#associationoptiontype) 
## AttributeGroupDetailsTypeDef

```python
# AttributeGroupDetailsTypeDef definition

class AttributeGroupDetailsTypeDef(TypedDict):
    id: NotRequired[str],
    arn: NotRequired[str],
    name: NotRequired[str],
    createdBy: NotRequired[str],
```

## AttributeGroupSummaryTypeDef

```python
# AttributeGroupSummaryTypeDef definition

class AttributeGroupSummaryTypeDef(TypedDict):
    id: NotRequired[str],
    arn: NotRequired[str],
    name: NotRequired[str],
    description: NotRequired[str],
    creationTime: NotRequired[datetime],
    lastUpdateTime: NotRequired[datetime],
    createdBy: NotRequired[str],
```

## AttributeGroupTypeDef

```python
# AttributeGroupTypeDef definition

class AttributeGroupTypeDef(TypedDict):
    id: NotRequired[str],
    arn: NotRequired[str],
    name: NotRequired[str],
    description: NotRequired[str],
    creationTime: NotRequired[datetime],
    lastUpdateTime: NotRequired[datetime],
    tags: NotRequired[Dict[str, str]],
```

## CreateApplicationRequestRequestTypeDef

```python
# CreateApplicationRequestRequestTypeDef definition

class CreateApplicationRequestRequestTypeDef(TypedDict):
    name: str,
    clientToken: str,
    description: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

## CreateAttributeGroupRequestRequestTypeDef

```python
# CreateAttributeGroupRequestRequestTypeDef definition

class CreateAttributeGroupRequestRequestTypeDef(TypedDict):
    name: str,
    attributes: str,
    clientToken: str,
    description: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

## DeleteApplicationRequestRequestTypeDef

```python
# DeleteApplicationRequestRequestTypeDef definition

class DeleteApplicationRequestRequestTypeDef(TypedDict):
    application: str,
```

## DeleteAttributeGroupRequestRequestTypeDef

```python
# DeleteAttributeGroupRequestRequestTypeDef definition

class DeleteAttributeGroupRequestRequestTypeDef(TypedDict):
    attributeGroup: str,
```

## DisassociateAttributeGroupRequestRequestTypeDef

```python
# DisassociateAttributeGroupRequestRequestTypeDef definition

class DisassociateAttributeGroupRequestRequestTypeDef(TypedDict):
    application: str,
    attributeGroup: str,
```

## DisassociateResourceRequestRequestTypeDef

```python
# DisassociateResourceRequestRequestTypeDef definition

class DisassociateResourceRequestRequestTypeDef(TypedDict):
    application: str,
    resourceType: ResourceTypeType,  # (1)
    resource: str,
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
## GetApplicationRequestRequestTypeDef

```python
# GetApplicationRequestRequestTypeDef definition

class GetApplicationRequestRequestTypeDef(TypedDict):
    application: str,
```

## GetAssociatedResourceRequestRequestTypeDef

```python
# GetAssociatedResourceRequestRequestTypeDef definition

class GetAssociatedResourceRequestRequestTypeDef(TypedDict):
    application: str,
    resourceType: ResourceTypeType,  # (1)
    resource: str,
    nextToken: NotRequired[str],
    resourceTagStatus: NotRequired[Sequence[ResourceItemStatusType]],  # (2)
    maxResults: NotRequired[int],
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
2. See [:material-code-brackets: ResourceItemStatusType](./literals.md#resourceitemstatustype) 
## GetAttributeGroupRequestRequestTypeDef

```python
# GetAttributeGroupRequestRequestTypeDef definition

class GetAttributeGroupRequestRequestTypeDef(TypedDict):
    attributeGroup: str,
```

## ResourceGroupTypeDef

```python
# ResourceGroupTypeDef definition

class ResourceGroupTypeDef(TypedDict):
    state: NotRequired[ResourceGroupStateType],  # (1)
    arn: NotRequired[str],
    errorMessage: NotRequired[str],
```

1. See [:material-code-brackets: ResourceGroupStateType](./literals.md#resourcegroupstatetype) 
## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListApplicationsRequestRequestTypeDef

```python
# ListApplicationsRequestRequestTypeDef definition

class ListApplicationsRequestRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListAssociatedAttributeGroupsRequestRequestTypeDef

```python
# ListAssociatedAttributeGroupsRequestRequestTypeDef definition

class ListAssociatedAttributeGroupsRequestRequestTypeDef(TypedDict):
    application: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListAssociatedResourcesRequestRequestTypeDef

```python
# ListAssociatedResourcesRequestRequestTypeDef definition

class ListAssociatedResourcesRequestRequestTypeDef(TypedDict):
    application: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListAttributeGroupsForApplicationRequestRequestTypeDef

```python
# ListAttributeGroupsForApplicationRequestRequestTypeDef definition

class ListAttributeGroupsForApplicationRequestRequestTypeDef(TypedDict):
    application: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListAttributeGroupsRequestRequestTypeDef

```python
# ListAttributeGroupsRequestRequestTypeDef definition

class ListAttributeGroupsRequestRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
```

## ResourceDetailsTypeDef

```python
# ResourceDetailsTypeDef definition

class ResourceDetailsTypeDef(TypedDict):
    tagValue: NotRequired[str],
```

## SyncResourceRequestRequestTypeDef

```python
# SyncResourceRequestRequestTypeDef definition

class SyncResourceRequestRequestTypeDef(TypedDict):
    resourceType: ResourceTypeType,  # (1)
    resource: str,
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    tags: Mapping[str, str],
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    tagKeys: Sequence[str],
```

## UpdateApplicationRequestRequestTypeDef

```python
# UpdateApplicationRequestRequestTypeDef definition

class UpdateApplicationRequestRequestTypeDef(TypedDict):
    application: str,
    name: NotRequired[str],
    description: NotRequired[str],
```

## UpdateAttributeGroupRequestRequestTypeDef

```python
# UpdateAttributeGroupRequestRequestTypeDef definition

class UpdateAttributeGroupRequestRequestTypeDef(TypedDict):
    attributeGroup: str,
    name: NotRequired[str],
    description: NotRequired[str],
    attributes: NotRequired[str],
```

## AppRegistryConfigurationTypeDef

```python
# AppRegistryConfigurationTypeDef definition

class AppRegistryConfigurationTypeDef(TypedDict):
    tagQueryConfiguration: NotRequired[TagQueryConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: TagQueryConfigurationTypeDef](./type_defs.md#tagqueryconfigurationtypedef) 
## ApplicationTagResultTypeDef

```python
# ApplicationTagResultTypeDef definition

class ApplicationTagResultTypeDef(TypedDict):
    applicationTagStatus: NotRequired[ApplicationTagStatusType],  # (1)
    errorMessage: NotRequired[str],
    resources: NotRequired[List[ResourcesListItemTypeDef]],  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-brackets: ApplicationTagStatusType](./literals.md#applicationtagstatustype) 
2. See [:material-code-braces: ResourcesListItemTypeDef](./type_defs.md#resourceslistitemtypedef) 
## AssociateAttributeGroupResponseTypeDef

```python
# AssociateAttributeGroupResponseTypeDef definition

class AssociateAttributeGroupResponseTypeDef(TypedDict):
    applicationArn: str,
    attributeGroupArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AssociateResourceResponseTypeDef

```python
# AssociateResourceResponseTypeDef definition

class AssociateResourceResponseTypeDef(TypedDict):
    applicationArn: str,
    resourceArn: str,
    options: List[AssociationOptionType],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: AssociationOptionType](./literals.md#associationoptiontype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateApplicationResponseTypeDef

```python
# CreateApplicationResponseTypeDef definition

class CreateApplicationResponseTypeDef(TypedDict):
    application: ApplicationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ApplicationTypeDef](./type_defs.md#applicationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteApplicationResponseTypeDef

```python
# DeleteApplicationResponseTypeDef definition

class DeleteApplicationResponseTypeDef(TypedDict):
    application: ApplicationSummaryTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ApplicationSummaryTypeDef](./type_defs.md#applicationsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DisassociateAttributeGroupResponseTypeDef

```python
# DisassociateAttributeGroupResponseTypeDef definition

class DisassociateAttributeGroupResponseTypeDef(TypedDict):
    applicationArn: str,
    attributeGroupArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DisassociateResourceResponseTypeDef

```python
# DisassociateResourceResponseTypeDef definition

class DisassociateResourceResponseTypeDef(TypedDict):
    applicationArn: str,
    resourceArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EmptyResponseMetadataTypeDef

```python
# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetAttributeGroupResponseTypeDef

```python
# GetAttributeGroupResponseTypeDef definition

class GetAttributeGroupResponseTypeDef(TypedDict):
    id: str,
    arn: str,
    name: str,
    description: str,
    attributes: str,
    creationTime: datetime,
    lastUpdateTime: datetime,
    tags: Dict[str, str],
    createdBy: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListApplicationsResponseTypeDef

```python
# ListApplicationsResponseTypeDef definition

class ListApplicationsResponseTypeDef(TypedDict):
    applications: List[ApplicationSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ApplicationSummaryTypeDef](./type_defs.md#applicationsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAssociatedAttributeGroupsResponseTypeDef

```python
# ListAssociatedAttributeGroupsResponseTypeDef definition

class ListAssociatedAttributeGroupsResponseTypeDef(TypedDict):
    attributeGroups: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SyncResourceResponseTypeDef

```python
# SyncResourceResponseTypeDef definition

class SyncResourceResponseTypeDef(TypedDict):
    applicationArn: str,
    resourceArn: str,
    actionTaken: SyncActionType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: SyncActionType](./literals.md#syncactiontype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateApplicationResponseTypeDef

```python
# UpdateApplicationResponseTypeDef definition

class UpdateApplicationResponseTypeDef(TypedDict):
    application: ApplicationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ApplicationTypeDef](./type_defs.md#applicationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAttributeGroupsForApplicationResponseTypeDef

```python
# ListAttributeGroupsForApplicationResponseTypeDef definition

class ListAttributeGroupsForApplicationResponseTypeDef(TypedDict):
    attributeGroupsDetails: List[AttributeGroupDetailsTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: AttributeGroupDetailsTypeDef](./type_defs.md#attributegroupdetailstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteAttributeGroupResponseTypeDef

```python
# DeleteAttributeGroupResponseTypeDef definition

class DeleteAttributeGroupResponseTypeDef(TypedDict):
    attributeGroup: AttributeGroupSummaryTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AttributeGroupSummaryTypeDef](./type_defs.md#attributegroupsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAttributeGroupsResponseTypeDef

```python
# ListAttributeGroupsResponseTypeDef definition

class ListAttributeGroupsResponseTypeDef(TypedDict):
    attributeGroups: List[AttributeGroupSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: AttributeGroupSummaryTypeDef](./type_defs.md#attributegroupsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateAttributeGroupResponseTypeDef

```python
# CreateAttributeGroupResponseTypeDef definition

class CreateAttributeGroupResponseTypeDef(TypedDict):
    attributeGroup: AttributeGroupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AttributeGroupTypeDef](./type_defs.md#attributegrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateAttributeGroupResponseTypeDef

```python
# UpdateAttributeGroupResponseTypeDef definition

class UpdateAttributeGroupResponseTypeDef(TypedDict):
    attributeGroup: AttributeGroupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AttributeGroupTypeDef](./type_defs.md#attributegrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## IntegrationsTypeDef

```python
# IntegrationsTypeDef definition

class IntegrationsTypeDef(TypedDict):
    resourceGroup: NotRequired[ResourceGroupTypeDef],  # (1)
    applicationTagResourceGroup: NotRequired[ResourceGroupTypeDef],  # (1)
```

1. See [:material-code-braces: ResourceGroupTypeDef](./type_defs.md#resourcegrouptypedef) 
2. See [:material-code-braces: ResourceGroupTypeDef](./type_defs.md#resourcegrouptypedef) 
## ResourceIntegrationsTypeDef

```python
# ResourceIntegrationsTypeDef definition

class ResourceIntegrationsTypeDef(TypedDict):
    resourceGroup: NotRequired[ResourceGroupTypeDef],  # (1)
```

1. See [:material-code-braces: ResourceGroupTypeDef](./type_defs.md#resourcegrouptypedef) 
## ListApplicationsRequestPaginateTypeDef

```python
# ListApplicationsRequestPaginateTypeDef definition

class ListApplicationsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAssociatedAttributeGroupsRequestPaginateTypeDef

```python
# ListAssociatedAttributeGroupsRequestPaginateTypeDef definition

class ListAssociatedAttributeGroupsRequestPaginateTypeDef(TypedDict):
    application: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAssociatedResourcesRequestPaginateTypeDef

```python
# ListAssociatedResourcesRequestPaginateTypeDef definition

class ListAssociatedResourcesRequestPaginateTypeDef(TypedDict):
    application: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAttributeGroupsForApplicationRequestPaginateTypeDef

```python
# ListAttributeGroupsForApplicationRequestPaginateTypeDef definition

class ListAttributeGroupsForApplicationRequestPaginateTypeDef(TypedDict):
    application: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAttributeGroupsRequestPaginateTypeDef

```python
# ListAttributeGroupsRequestPaginateTypeDef definition

class ListAttributeGroupsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ResourceInfoTypeDef

```python
# ResourceInfoTypeDef definition

class ResourceInfoTypeDef(TypedDict):
    name: NotRequired[str],
    arn: NotRequired[str],
    resourceType: NotRequired[ResourceTypeType],  # (1)
    resourceDetails: NotRequired[ResourceDetailsTypeDef],  # (2)
    options: NotRequired[List[AssociationOptionType]],  # (3)
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
2. See [:material-code-braces: ResourceDetailsTypeDef](./type_defs.md#resourcedetailstypedef) 
3. See [:material-code-brackets: AssociationOptionType](./literals.md#associationoptiontype) 
## GetConfigurationResponseTypeDef

```python
# GetConfigurationResponseTypeDef definition

class GetConfigurationResponseTypeDef(TypedDict):
    configuration: AppRegistryConfigurationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AppRegistryConfigurationTypeDef](./type_defs.md#appregistryconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutConfigurationRequestRequestTypeDef

```python
# PutConfigurationRequestRequestTypeDef definition

class PutConfigurationRequestRequestTypeDef(TypedDict):
    configuration: AppRegistryConfigurationTypeDef,  # (1)
```

1. See [:material-code-braces: AppRegistryConfigurationTypeDef](./type_defs.md#appregistryconfigurationtypedef) 
## GetApplicationResponseTypeDef

```python
# GetApplicationResponseTypeDef definition

class GetApplicationResponseTypeDef(TypedDict):
    id: str,
    arn: str,
    name: str,
    description: str,
    creationTime: datetime,
    lastUpdateTime: datetime,
    associatedResourceCount: int,
    tags: Dict[str, str],
    integrations: IntegrationsTypeDef,  # (1)
    applicationTag: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: IntegrationsTypeDef](./type_defs.md#integrationstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ResourceTypeDef

```python
# ResourceTypeDef definition

class ResourceTypeDef(TypedDict):
    name: NotRequired[str],
    arn: NotRequired[str],
    associationTime: NotRequired[datetime],
    integrations: NotRequired[ResourceIntegrationsTypeDef],  # (1)
```

1. See [:material-code-braces: ResourceIntegrationsTypeDef](./type_defs.md#resourceintegrationstypedef) 
## ListAssociatedResourcesResponseTypeDef

```python
# ListAssociatedResourcesResponseTypeDef definition

class ListAssociatedResourcesResponseTypeDef(TypedDict):
    resources: List[ResourceInfoTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ResourceInfoTypeDef](./type_defs.md#resourceinfotypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetAssociatedResourceResponseTypeDef

```python
# GetAssociatedResourceResponseTypeDef definition

class GetAssociatedResourceResponseTypeDef(TypedDict):
    resource: ResourceTypeDef,  # (1)
    options: List[AssociationOptionType],  # (2)
    applicationTagResult: ApplicationTagResultTypeDef,  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: ResourceTypeDef](./type_defs.md#resourcetypedef) 
2. See [:material-code-brackets: AssociationOptionType](./literals.md#associationoptiontype) 
3. See [:material-code-braces: ApplicationTagResultTypeDef](./type_defs.md#applicationtagresulttypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
