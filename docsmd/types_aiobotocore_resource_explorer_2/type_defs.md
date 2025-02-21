# Type definitions

> [Index](../README.md) > [ResourceExplorer](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [ResourceExplorer](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-explorer-2.html#resourceexplorer)
    type annotations stubs module [types-aiobotocore-resource-explorer-2](https://pypi.org/project/types-aiobotocore-resource-explorer-2/).



## AssociateDefaultViewInputTypeDef

```python
# AssociateDefaultViewInputTypeDef TypedDict usage example

from types_aiobotocore_resource_explorer_2.type_defs import AssociateDefaultViewInputTypeDef


def get_value() -> AssociateDefaultViewInputTypeDef:
    return {
        "ViewArn": ...,
    }


# AssociateDefaultViewInputTypeDef definition

class AssociateDefaultViewInputTypeDef(TypedDict):
    ViewArn: str,
```

## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_resource_explorer_2.type_defs import ResponseMetadataTypeDef


def get_value() -> ResponseMetadataTypeDef:
    return {
        "RequestId": ...,
    }


# ResponseMetadataTypeDef definition

class ResponseMetadataTypeDef(TypedDict):
    RequestId: str,
    HTTPStatusCode: int,
    HTTPHeaders: Dict[str, str],
    RetryAttempts: int,
    HostId: NotRequired[str],
```

## BatchGetViewErrorTypeDef

```python
# BatchGetViewErrorTypeDef TypedDict usage example

from types_aiobotocore_resource_explorer_2.type_defs import BatchGetViewErrorTypeDef


def get_value() -> BatchGetViewErrorTypeDef:
    return {
        "ErrorMessage": ...,
    }


# BatchGetViewErrorTypeDef definition

class BatchGetViewErrorTypeDef(TypedDict):
    ErrorMessage: str,
    ViewArn: str,
```

## BatchGetViewInputTypeDef

```python
# BatchGetViewInputTypeDef TypedDict usage example

from types_aiobotocore_resource_explorer_2.type_defs import BatchGetViewInputTypeDef


def get_value() -> BatchGetViewInputTypeDef:
    return {
        "ViewArns": ...,
    }


# BatchGetViewInputTypeDef definition

class BatchGetViewInputTypeDef(TypedDict):
    ViewArns: NotRequired[Sequence[str]],
```

## CreateIndexInputTypeDef

```python
# CreateIndexInputTypeDef TypedDict usage example

from types_aiobotocore_resource_explorer_2.type_defs import CreateIndexInputTypeDef


def get_value() -> CreateIndexInputTypeDef:
    return {
        "ClientToken": ...,
    }


# CreateIndexInputTypeDef definition

class CreateIndexInputTypeDef(TypedDict):
    ClientToken: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
```

## IncludedPropertyTypeDef

```python
# IncludedPropertyTypeDef TypedDict usage example

from types_aiobotocore_resource_explorer_2.type_defs import IncludedPropertyTypeDef


def get_value() -> IncludedPropertyTypeDef:
    return {
        "Name": ...,
    }


# IncludedPropertyTypeDef definition

class IncludedPropertyTypeDef(TypedDict):
    Name: str,
```

## SearchFilterTypeDef

```python
# SearchFilterTypeDef TypedDict usage example

from types_aiobotocore_resource_explorer_2.type_defs import SearchFilterTypeDef


def get_value() -> SearchFilterTypeDef:
    return {
        "FilterString": ...,
    }


# SearchFilterTypeDef definition

class SearchFilterTypeDef(TypedDict):
    FilterString: str,
```

## DeleteIndexInputTypeDef

```python
# DeleteIndexInputTypeDef TypedDict usage example

from types_aiobotocore_resource_explorer_2.type_defs import DeleteIndexInputTypeDef


def get_value() -> DeleteIndexInputTypeDef:
    return {
        "Arn": ...,
    }


# DeleteIndexInputTypeDef definition

class DeleteIndexInputTypeDef(TypedDict):
    Arn: str,
```

## DeleteViewInputTypeDef

```python
# DeleteViewInputTypeDef TypedDict usage example

from types_aiobotocore_resource_explorer_2.type_defs import DeleteViewInputTypeDef


def get_value() -> DeleteViewInputTypeDef:
    return {
        "ViewArn": ...,
    }


# DeleteViewInputTypeDef definition

class DeleteViewInputTypeDef(TypedDict):
    ViewArn: str,
```

## OrgConfigurationTypeDef

```python
# OrgConfigurationTypeDef TypedDict usage example

from types_aiobotocore_resource_explorer_2.type_defs import OrgConfigurationTypeDef


def get_value() -> OrgConfigurationTypeDef:
    return {
        "AWSServiceAccessStatus": ...,
    }


# OrgConfigurationTypeDef definition

class OrgConfigurationTypeDef(TypedDict):
    AWSServiceAccessStatus: AWSServiceAccessStatusType,  # (1)
    ServiceLinkedRole: NotRequired[str],
```

1. See [:material-code-brackets: AWSServiceAccessStatusType](./literals.md#awsserviceaccessstatustype) 
## GetManagedViewInputTypeDef

```python
# GetManagedViewInputTypeDef TypedDict usage example

from types_aiobotocore_resource_explorer_2.type_defs import GetManagedViewInputTypeDef


def get_value() -> GetManagedViewInputTypeDef:
    return {
        "ManagedViewArn": ...,
    }


# GetManagedViewInputTypeDef definition

class GetManagedViewInputTypeDef(TypedDict):
    ManagedViewArn: str,
```

## GetViewInputTypeDef

```python
# GetViewInputTypeDef TypedDict usage example

from types_aiobotocore_resource_explorer_2.type_defs import GetViewInputTypeDef


def get_value() -> GetViewInputTypeDef:
    return {
        "ViewArn": ...,
    }


# GetViewInputTypeDef definition

class GetViewInputTypeDef(TypedDict):
    ViewArn: str,
```

## IndexTypeDef

```python
# IndexTypeDef TypedDict usage example

from types_aiobotocore_resource_explorer_2.type_defs import IndexTypeDef


def get_value() -> IndexTypeDef:
    return {
        "Arn": ...,
    }


# IndexTypeDef definition

class IndexTypeDef(TypedDict):
    Arn: NotRequired[str],
    Region: NotRequired[str],
    Type: NotRequired[IndexTypeType],  # (1)
```

1. See [:material-code-brackets: IndexTypeType](./literals.md#indextypetype) 
## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef TypedDict usage example

from types_aiobotocore_resource_explorer_2.type_defs import PaginatorConfigTypeDef


def get_value() -> PaginatorConfigTypeDef:
    return {
        "MaxItems": ...,
    }


# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListIndexesForMembersInputTypeDef

```python
# ListIndexesForMembersInputTypeDef TypedDict usage example

from types_aiobotocore_resource_explorer_2.type_defs import ListIndexesForMembersInputTypeDef


def get_value() -> ListIndexesForMembersInputTypeDef:
    return {
        "AccountIdList": ...,
    }


# ListIndexesForMembersInputTypeDef definition

class ListIndexesForMembersInputTypeDef(TypedDict):
    AccountIdList: Sequence[str],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## MemberIndexTypeDef

```python
# MemberIndexTypeDef TypedDict usage example

from types_aiobotocore_resource_explorer_2.type_defs import MemberIndexTypeDef


def get_value() -> MemberIndexTypeDef:
    return {
        "AccountId": ...,
    }


# MemberIndexTypeDef definition

class MemberIndexTypeDef(TypedDict):
    AccountId: NotRequired[str],
    Arn: NotRequired[str],
    Region: NotRequired[str],
    Type: NotRequired[IndexTypeType],  # (1)
```

1. See [:material-code-brackets: IndexTypeType](./literals.md#indextypetype) 
## ListIndexesInputTypeDef

```python
# ListIndexesInputTypeDef TypedDict usage example

from types_aiobotocore_resource_explorer_2.type_defs import ListIndexesInputTypeDef


def get_value() -> ListIndexesInputTypeDef:
    return {
        "MaxResults": ...,
    }


# ListIndexesInputTypeDef definition

class ListIndexesInputTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    Regions: NotRequired[Sequence[str]],
    Type: NotRequired[IndexTypeType],  # (1)
```

1. See [:material-code-brackets: IndexTypeType](./literals.md#indextypetype) 
## ListManagedViewsInputTypeDef

```python
# ListManagedViewsInputTypeDef TypedDict usage example

from types_aiobotocore_resource_explorer_2.type_defs import ListManagedViewsInputTypeDef


def get_value() -> ListManagedViewsInputTypeDef:
    return {
        "MaxResults": ...,
    }


# ListManagedViewsInputTypeDef definition

class ListManagedViewsInputTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    ServicePrincipal: NotRequired[str],
```

## ListSupportedResourceTypesInputTypeDef

```python
# ListSupportedResourceTypesInputTypeDef TypedDict usage example

from types_aiobotocore_resource_explorer_2.type_defs import ListSupportedResourceTypesInputTypeDef


def get_value() -> ListSupportedResourceTypesInputTypeDef:
    return {
        "MaxResults": ...,
    }


# ListSupportedResourceTypesInputTypeDef definition

class ListSupportedResourceTypesInputTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## SupportedResourceTypeTypeDef

```python
# SupportedResourceTypeTypeDef TypedDict usage example

from types_aiobotocore_resource_explorer_2.type_defs import SupportedResourceTypeTypeDef


def get_value() -> SupportedResourceTypeTypeDef:
    return {
        "ResourceType": ...,
    }


# SupportedResourceTypeTypeDef definition

class SupportedResourceTypeTypeDef(TypedDict):
    ResourceType: NotRequired[str],
    Service: NotRequired[str],
```

## ListTagsForResourceInputTypeDef

```python
# ListTagsForResourceInputTypeDef TypedDict usage example

from types_aiobotocore_resource_explorer_2.type_defs import ListTagsForResourceInputTypeDef


def get_value() -> ListTagsForResourceInputTypeDef:
    return {
        "resourceArn": ...,
    }


# ListTagsForResourceInputTypeDef definition

class ListTagsForResourceInputTypeDef(TypedDict):
    resourceArn: str,
```

## ListViewsInputTypeDef

```python
# ListViewsInputTypeDef TypedDict usage example

from types_aiobotocore_resource_explorer_2.type_defs import ListViewsInputTypeDef


def get_value() -> ListViewsInputTypeDef:
    return {
        "MaxResults": ...,
    }


# ListViewsInputTypeDef definition

class ListViewsInputTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ResourceCountTypeDef

```python
# ResourceCountTypeDef TypedDict usage example

from types_aiobotocore_resource_explorer_2.type_defs import ResourceCountTypeDef


def get_value() -> ResourceCountTypeDef:
    return {
        "Complete": ...,
    }


# ResourceCountTypeDef definition

class ResourceCountTypeDef(TypedDict):
    Complete: NotRequired[bool],
    TotalResources: NotRequired[int],
```

## ResourcePropertyTypeDef

```python
# ResourcePropertyTypeDef TypedDict usage example

from types_aiobotocore_resource_explorer_2.type_defs import ResourcePropertyTypeDef


def get_value() -> ResourcePropertyTypeDef:
    return {
        "Data": ...,
    }


# ResourcePropertyTypeDef definition

class ResourcePropertyTypeDef(TypedDict):
    Data: NotRequired[Dict[str, Any]],
    LastReportedAt: NotRequired[datetime],
    Name: NotRequired[str],
```

## SearchInputTypeDef

```python
# SearchInputTypeDef TypedDict usage example

from types_aiobotocore_resource_explorer_2.type_defs import SearchInputTypeDef


def get_value() -> SearchInputTypeDef:
    return {
        "QueryString": ...,
    }


# SearchInputTypeDef definition

class SearchInputTypeDef(TypedDict):
    QueryString: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    ViewArn: NotRequired[str],
```

## TagResourceInputTypeDef

```python
# TagResourceInputTypeDef TypedDict usage example

from types_aiobotocore_resource_explorer_2.type_defs import TagResourceInputTypeDef


def get_value() -> TagResourceInputTypeDef:
    return {
        "resourceArn": ...,
    }


# TagResourceInputTypeDef definition

class TagResourceInputTypeDef(TypedDict):
    resourceArn: str,
    Tags: NotRequired[Mapping[str, str]],
```

## UntagResourceInputTypeDef

```python
# UntagResourceInputTypeDef TypedDict usage example

from types_aiobotocore_resource_explorer_2.type_defs import UntagResourceInputTypeDef


def get_value() -> UntagResourceInputTypeDef:
    return {
        "resourceArn": ...,
    }


# UntagResourceInputTypeDef definition

class UntagResourceInputTypeDef(TypedDict):
    resourceArn: str,
    tagKeys: Sequence[str],
```

## UpdateIndexTypeInputTypeDef

```python
# UpdateIndexTypeInputTypeDef TypedDict usage example

from types_aiobotocore_resource_explorer_2.type_defs import UpdateIndexTypeInputTypeDef


def get_value() -> UpdateIndexTypeInputTypeDef:
    return {
        "Arn": ...,
    }


# UpdateIndexTypeInputTypeDef definition

class UpdateIndexTypeInputTypeDef(TypedDict):
    Arn: str,
    Type: IndexTypeType,  # (1)
```

1. See [:material-code-brackets: IndexTypeType](./literals.md#indextypetype) 
## AssociateDefaultViewOutputTypeDef

```python
# AssociateDefaultViewOutputTypeDef TypedDict usage example

from types_aiobotocore_resource_explorer_2.type_defs import AssociateDefaultViewOutputTypeDef


def get_value() -> AssociateDefaultViewOutputTypeDef:
    return {
        "ViewArn": ...,
    }


# AssociateDefaultViewOutputTypeDef definition

class AssociateDefaultViewOutputTypeDef(TypedDict):
    ViewArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateIndexOutputTypeDef

```python
# CreateIndexOutputTypeDef TypedDict usage example

from types_aiobotocore_resource_explorer_2.type_defs import CreateIndexOutputTypeDef


def get_value() -> CreateIndexOutputTypeDef:
    return {
        "Arn": ...,
    }


# CreateIndexOutputTypeDef definition

class CreateIndexOutputTypeDef(TypedDict):
    Arn: str,
    CreatedAt: datetime,
    State: IndexStateType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: IndexStateType](./literals.md#indexstatetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteIndexOutputTypeDef

```python
# DeleteIndexOutputTypeDef TypedDict usage example

from types_aiobotocore_resource_explorer_2.type_defs import DeleteIndexOutputTypeDef


def get_value() -> DeleteIndexOutputTypeDef:
    return {
        "Arn": ...,
    }


# DeleteIndexOutputTypeDef definition

class DeleteIndexOutputTypeDef(TypedDict):
    Arn: str,
    LastUpdatedAt: datetime,
    State: IndexStateType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: IndexStateType](./literals.md#indexstatetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteViewOutputTypeDef

```python
# DeleteViewOutputTypeDef TypedDict usage example

from types_aiobotocore_resource_explorer_2.type_defs import DeleteViewOutputTypeDef


def get_value() -> DeleteViewOutputTypeDef:
    return {
        "ViewArn": ...,
    }


# DeleteViewOutputTypeDef definition

class DeleteViewOutputTypeDef(TypedDict):
    ViewArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EmptyResponseMetadataTypeDef

```python
# EmptyResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_resource_explorer_2.type_defs import EmptyResponseMetadataTypeDef


def get_value() -> EmptyResponseMetadataTypeDef:
    return {
        "ResponseMetadata": ...,
    }


# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetDefaultViewOutputTypeDef

```python
# GetDefaultViewOutputTypeDef TypedDict usage example

from types_aiobotocore_resource_explorer_2.type_defs import GetDefaultViewOutputTypeDef


def get_value() -> GetDefaultViewOutputTypeDef:
    return {
        "ViewArn": ...,
    }


# GetDefaultViewOutputTypeDef definition

class GetDefaultViewOutputTypeDef(TypedDict):
    ViewArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetIndexOutputTypeDef

```python
# GetIndexOutputTypeDef TypedDict usage example

from types_aiobotocore_resource_explorer_2.type_defs import GetIndexOutputTypeDef


def get_value() -> GetIndexOutputTypeDef:
    return {
        "Arn": ...,
    }


# GetIndexOutputTypeDef definition

class GetIndexOutputTypeDef(TypedDict):
    Arn: str,
    CreatedAt: datetime,
    LastUpdatedAt: datetime,
    ReplicatingFrom: List[str],
    ReplicatingTo: List[str],
    State: IndexStateType,  # (1)
    Tags: Dict[str, str],
    Type: IndexTypeType,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: IndexStateType](./literals.md#indexstatetype) 
2. See [:material-code-brackets: IndexTypeType](./literals.md#indextypetype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListManagedViewsOutputTypeDef

```python
# ListManagedViewsOutputTypeDef TypedDict usage example

from types_aiobotocore_resource_explorer_2.type_defs import ListManagedViewsOutputTypeDef


def get_value() -> ListManagedViewsOutputTypeDef:
    return {
        "ManagedViews": ...,
    }


# ListManagedViewsOutputTypeDef definition

class ListManagedViewsOutputTypeDef(TypedDict):
    ManagedViews: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceOutputTypeDef

```python
# ListTagsForResourceOutputTypeDef TypedDict usage example

from types_aiobotocore_resource_explorer_2.type_defs import ListTagsForResourceOutputTypeDef


def get_value() -> ListTagsForResourceOutputTypeDef:
    return {
        "Tags": ...,
    }


# ListTagsForResourceOutputTypeDef definition

class ListTagsForResourceOutputTypeDef(TypedDict):
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListViewsOutputTypeDef

```python
# ListViewsOutputTypeDef TypedDict usage example

from types_aiobotocore_resource_explorer_2.type_defs import ListViewsOutputTypeDef


def get_value() -> ListViewsOutputTypeDef:
    return {
        "NextToken": ...,
    }


# ListViewsOutputTypeDef definition

class ListViewsOutputTypeDef(TypedDict):
    Views: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateIndexTypeOutputTypeDef

```python
# UpdateIndexTypeOutputTypeDef TypedDict usage example

from types_aiobotocore_resource_explorer_2.type_defs import UpdateIndexTypeOutputTypeDef


def get_value() -> UpdateIndexTypeOutputTypeDef:
    return {
        "Arn": ...,
    }


# UpdateIndexTypeOutputTypeDef definition

class UpdateIndexTypeOutputTypeDef(TypedDict):
    Arn: str,
    LastUpdatedAt: datetime,
    State: IndexStateType,  # (1)
    Type: IndexTypeType,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: IndexStateType](./literals.md#indexstatetype) 
2. See [:material-code-brackets: IndexTypeType](./literals.md#indextypetype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateViewInputTypeDef

```python
# CreateViewInputTypeDef TypedDict usage example

from types_aiobotocore_resource_explorer_2.type_defs import CreateViewInputTypeDef


def get_value() -> CreateViewInputTypeDef:
    return {
        "ViewName": ...,
    }


# CreateViewInputTypeDef definition

class CreateViewInputTypeDef(TypedDict):
    ViewName: str,
    ClientToken: NotRequired[str],
    Filters: NotRequired[SearchFilterTypeDef],  # (1)
    IncludedProperties: NotRequired[Sequence[IncludedPropertyTypeDef]],  # (2)
    Scope: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: SearchFilterTypeDef](./type_defs.md#searchfiltertypedef) 
2. See [:material-code-braces: IncludedPropertyTypeDef](./type_defs.md#includedpropertytypedef) 
## ListResourcesInputTypeDef

```python
# ListResourcesInputTypeDef TypedDict usage example

from types_aiobotocore_resource_explorer_2.type_defs import ListResourcesInputTypeDef


def get_value() -> ListResourcesInputTypeDef:
    return {
        "Filters": ...,
    }


# ListResourcesInputTypeDef definition

class ListResourcesInputTypeDef(TypedDict):
    Filters: NotRequired[SearchFilterTypeDef],  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    ViewArn: NotRequired[str],
```

1. See [:material-code-braces: SearchFilterTypeDef](./type_defs.md#searchfiltertypedef) 
## ManagedViewTypeDef

```python
# ManagedViewTypeDef TypedDict usage example

from types_aiobotocore_resource_explorer_2.type_defs import ManagedViewTypeDef


def get_value() -> ManagedViewTypeDef:
    return {
        "Filters": ...,
    }


# ManagedViewTypeDef definition

class ManagedViewTypeDef(TypedDict):
    Filters: NotRequired[SearchFilterTypeDef],  # (1)
    IncludedProperties: NotRequired[List[IncludedPropertyTypeDef]],  # (2)
    LastUpdatedAt: NotRequired[datetime],
    ManagedViewArn: NotRequired[str],
    ManagedViewName: NotRequired[str],
    Owner: NotRequired[str],
    ResourcePolicy: NotRequired[str],
    Scope: NotRequired[str],
    TrustedService: NotRequired[str],
    Version: NotRequired[str],
```

1. See [:material-code-braces: SearchFilterTypeDef](./type_defs.md#searchfiltertypedef) 
2. See [:material-code-braces: IncludedPropertyTypeDef](./type_defs.md#includedpropertytypedef) 
## UpdateViewInputTypeDef

```python
# UpdateViewInputTypeDef TypedDict usage example

from types_aiobotocore_resource_explorer_2.type_defs import UpdateViewInputTypeDef


def get_value() -> UpdateViewInputTypeDef:
    return {
        "ViewArn": ...,
    }


# UpdateViewInputTypeDef definition

class UpdateViewInputTypeDef(TypedDict):
    ViewArn: str,
    Filters: NotRequired[SearchFilterTypeDef],  # (1)
    IncludedProperties: NotRequired[Sequence[IncludedPropertyTypeDef]],  # (2)
```

1. See [:material-code-braces: SearchFilterTypeDef](./type_defs.md#searchfiltertypedef) 
2. See [:material-code-braces: IncludedPropertyTypeDef](./type_defs.md#includedpropertytypedef) 
## ViewTypeDef

```python
# ViewTypeDef TypedDict usage example

from types_aiobotocore_resource_explorer_2.type_defs import ViewTypeDef


def get_value() -> ViewTypeDef:
    return {
        "Filters": ...,
    }


# ViewTypeDef definition

class ViewTypeDef(TypedDict):
    Filters: NotRequired[SearchFilterTypeDef],  # (1)
    IncludedProperties: NotRequired[List[IncludedPropertyTypeDef]],  # (2)
    LastUpdatedAt: NotRequired[datetime],
    Owner: NotRequired[str],
    Scope: NotRequired[str],
    ViewArn: NotRequired[str],
```

1. See [:material-code-braces: SearchFilterTypeDef](./type_defs.md#searchfiltertypedef) 
2. See [:material-code-braces: IncludedPropertyTypeDef](./type_defs.md#includedpropertytypedef) 
## GetAccountLevelServiceConfigurationOutputTypeDef

```python
# GetAccountLevelServiceConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_resource_explorer_2.type_defs import GetAccountLevelServiceConfigurationOutputTypeDef


def get_value() -> GetAccountLevelServiceConfigurationOutputTypeDef:
    return {
        "OrgConfiguration": ...,
    }


# GetAccountLevelServiceConfigurationOutputTypeDef definition

class GetAccountLevelServiceConfigurationOutputTypeDef(TypedDict):
    OrgConfiguration: OrgConfigurationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OrgConfigurationTypeDef](./type_defs.md#orgconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListIndexesOutputTypeDef

```python
# ListIndexesOutputTypeDef TypedDict usage example

from types_aiobotocore_resource_explorer_2.type_defs import ListIndexesOutputTypeDef


def get_value() -> ListIndexesOutputTypeDef:
    return {
        "Indexes": ...,
    }


# ListIndexesOutputTypeDef definition

class ListIndexesOutputTypeDef(TypedDict):
    Indexes: List[IndexTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: IndexTypeDef](./type_defs.md#indextypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListIndexesForMembersInputPaginateTypeDef

```python
# ListIndexesForMembersInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_resource_explorer_2.type_defs import ListIndexesForMembersInputPaginateTypeDef


def get_value() -> ListIndexesForMembersInputPaginateTypeDef:
    return {
        "AccountIdList": ...,
    }


# ListIndexesForMembersInputPaginateTypeDef definition

class ListIndexesForMembersInputPaginateTypeDef(TypedDict):
    AccountIdList: Sequence[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListIndexesInputPaginateTypeDef

```python
# ListIndexesInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_resource_explorer_2.type_defs import ListIndexesInputPaginateTypeDef


def get_value() -> ListIndexesInputPaginateTypeDef:
    return {
        "Regions": ...,
    }


# ListIndexesInputPaginateTypeDef definition

class ListIndexesInputPaginateTypeDef(TypedDict):
    Regions: NotRequired[Sequence[str]],
    Type: NotRequired[IndexTypeType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: IndexTypeType](./literals.md#indextypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListManagedViewsInputPaginateTypeDef

```python
# ListManagedViewsInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_resource_explorer_2.type_defs import ListManagedViewsInputPaginateTypeDef


def get_value() -> ListManagedViewsInputPaginateTypeDef:
    return {
        "ServicePrincipal": ...,
    }


# ListManagedViewsInputPaginateTypeDef definition

class ListManagedViewsInputPaginateTypeDef(TypedDict):
    ServicePrincipal: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListResourcesInputPaginateTypeDef

```python
# ListResourcesInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_resource_explorer_2.type_defs import ListResourcesInputPaginateTypeDef


def get_value() -> ListResourcesInputPaginateTypeDef:
    return {
        "Filters": ...,
    }


# ListResourcesInputPaginateTypeDef definition

class ListResourcesInputPaginateTypeDef(TypedDict):
    Filters: NotRequired[SearchFilterTypeDef],  # (1)
    ViewArn: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: SearchFilterTypeDef](./type_defs.md#searchfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListSupportedResourceTypesInputPaginateTypeDef

```python
# ListSupportedResourceTypesInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_resource_explorer_2.type_defs import ListSupportedResourceTypesInputPaginateTypeDef


def get_value() -> ListSupportedResourceTypesInputPaginateTypeDef:
    return {
        "PaginationConfig": ...,
    }


# ListSupportedResourceTypesInputPaginateTypeDef definition

class ListSupportedResourceTypesInputPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListViewsInputPaginateTypeDef

```python
# ListViewsInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_resource_explorer_2.type_defs import ListViewsInputPaginateTypeDef


def get_value() -> ListViewsInputPaginateTypeDef:
    return {
        "PaginationConfig": ...,
    }


# ListViewsInputPaginateTypeDef definition

class ListViewsInputPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## SearchInputPaginateTypeDef

```python
# SearchInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_resource_explorer_2.type_defs import SearchInputPaginateTypeDef


def get_value() -> SearchInputPaginateTypeDef:
    return {
        "QueryString": ...,
    }


# SearchInputPaginateTypeDef definition

class SearchInputPaginateTypeDef(TypedDict):
    QueryString: str,
    ViewArn: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListIndexesForMembersOutputTypeDef

```python
# ListIndexesForMembersOutputTypeDef TypedDict usage example

from types_aiobotocore_resource_explorer_2.type_defs import ListIndexesForMembersOutputTypeDef


def get_value() -> ListIndexesForMembersOutputTypeDef:
    return {
        "Indexes": ...,
    }


# ListIndexesForMembersOutputTypeDef definition

class ListIndexesForMembersOutputTypeDef(TypedDict):
    Indexes: List[MemberIndexTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: MemberIndexTypeDef](./type_defs.md#memberindextypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListSupportedResourceTypesOutputTypeDef

```python
# ListSupportedResourceTypesOutputTypeDef TypedDict usage example

from types_aiobotocore_resource_explorer_2.type_defs import ListSupportedResourceTypesOutputTypeDef


def get_value() -> ListSupportedResourceTypesOutputTypeDef:
    return {
        "NextToken": ...,
    }


# ListSupportedResourceTypesOutputTypeDef definition

class ListSupportedResourceTypesOutputTypeDef(TypedDict):
    ResourceTypes: List[SupportedResourceTypeTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: SupportedResourceTypeTypeDef](./type_defs.md#supportedresourcetypetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ResourceTypeDef

```python
# ResourceTypeDef TypedDict usage example

from types_aiobotocore_resource_explorer_2.type_defs import ResourceTypeDef


def get_value() -> ResourceTypeDef:
    return {
        "Arn": ...,
    }


# ResourceTypeDef definition

class ResourceTypeDef(TypedDict):
    Arn: NotRequired[str],
    LastReportedAt: NotRequired[datetime],
    OwningAccountId: NotRequired[str],
    Properties: NotRequired[List[ResourcePropertyTypeDef]],  # (1)
    Region: NotRequired[str],
    ResourceType: NotRequired[str],
    Service: NotRequired[str],
```

1. See [:material-code-braces: ResourcePropertyTypeDef](./type_defs.md#resourcepropertytypedef) 
## GetManagedViewOutputTypeDef

```python
# GetManagedViewOutputTypeDef TypedDict usage example

from types_aiobotocore_resource_explorer_2.type_defs import GetManagedViewOutputTypeDef


def get_value() -> GetManagedViewOutputTypeDef:
    return {
        "ManagedView": ...,
    }


# GetManagedViewOutputTypeDef definition

class GetManagedViewOutputTypeDef(TypedDict):
    ManagedView: ManagedViewTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ManagedViewTypeDef](./type_defs.md#managedviewtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchGetViewOutputTypeDef

```python
# BatchGetViewOutputTypeDef TypedDict usage example

from types_aiobotocore_resource_explorer_2.type_defs import BatchGetViewOutputTypeDef


def get_value() -> BatchGetViewOutputTypeDef:
    return {
        "Errors": ...,
    }


# BatchGetViewOutputTypeDef definition

class BatchGetViewOutputTypeDef(TypedDict):
    Errors: List[BatchGetViewErrorTypeDef],  # (1)
    Views: List[ViewTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: BatchGetViewErrorTypeDef](./type_defs.md#batchgetviewerrortypedef) 
2. See [:material-code-braces: ViewTypeDef](./type_defs.md#viewtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateViewOutputTypeDef

```python
# CreateViewOutputTypeDef TypedDict usage example

from types_aiobotocore_resource_explorer_2.type_defs import CreateViewOutputTypeDef


def get_value() -> CreateViewOutputTypeDef:
    return {
        "View": ...,
    }


# CreateViewOutputTypeDef definition

class CreateViewOutputTypeDef(TypedDict):
    View: ViewTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ViewTypeDef](./type_defs.md#viewtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetViewOutputTypeDef

```python
# GetViewOutputTypeDef TypedDict usage example

from types_aiobotocore_resource_explorer_2.type_defs import GetViewOutputTypeDef


def get_value() -> GetViewOutputTypeDef:
    return {
        "Tags": ...,
    }


# GetViewOutputTypeDef definition

class GetViewOutputTypeDef(TypedDict):
    Tags: Dict[str, str],
    View: ViewTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ViewTypeDef](./type_defs.md#viewtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateViewOutputTypeDef

```python
# UpdateViewOutputTypeDef TypedDict usage example

from types_aiobotocore_resource_explorer_2.type_defs import UpdateViewOutputTypeDef


def get_value() -> UpdateViewOutputTypeDef:
    return {
        "View": ...,
    }


# UpdateViewOutputTypeDef definition

class UpdateViewOutputTypeDef(TypedDict):
    View: ViewTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ViewTypeDef](./type_defs.md#viewtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListResourcesOutputTypeDef

```python
# ListResourcesOutputTypeDef TypedDict usage example

from types_aiobotocore_resource_explorer_2.type_defs import ListResourcesOutputTypeDef


def get_value() -> ListResourcesOutputTypeDef:
    return {
        "NextToken": ...,
    }


# ListResourcesOutputTypeDef definition

class ListResourcesOutputTypeDef(TypedDict):
    Resources: List[ResourceTypeDef],  # (1)
    ViewArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ResourceTypeDef](./type_defs.md#resourcetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SearchOutputTypeDef

```python
# SearchOutputTypeDef TypedDict usage example

from types_aiobotocore_resource_explorer_2.type_defs import SearchOutputTypeDef


def get_value() -> SearchOutputTypeDef:
    return {
        "Count": ...,
    }


# SearchOutputTypeDef definition

class SearchOutputTypeDef(TypedDict):
    Count: ResourceCountTypeDef,  # (1)
    Resources: List[ResourceTypeDef],  # (2)
    ViewArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ResourceCountTypeDef](./type_defs.md#resourcecounttypedef) 
2. See [:material-code-braces: ResourceTypeDef](./type_defs.md#resourcetypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
