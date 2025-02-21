# Type definitions

> [Index](../README.md) > [ControlCatalog](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [ControlCatalog](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controlcatalog.html#controlcatalog)
    type annotations stubs module [types-aiobotocore-controlcatalog](https://pypi.org/project/types-aiobotocore-controlcatalog/).



## AssociatedDomainSummaryTypeDef

```python
# AssociatedDomainSummaryTypeDef TypedDict usage example

from types_aiobotocore_controlcatalog.type_defs import AssociatedDomainSummaryTypeDef


def get_value() -> AssociatedDomainSummaryTypeDef:
    return {
        "Arn": ...,
    }


# AssociatedDomainSummaryTypeDef definition

class AssociatedDomainSummaryTypeDef(TypedDict):
    Arn: NotRequired[str],
    Name: NotRequired[str],
```

## AssociatedObjectiveSummaryTypeDef

```python
# AssociatedObjectiveSummaryTypeDef TypedDict usage example

from types_aiobotocore_controlcatalog.type_defs import AssociatedObjectiveSummaryTypeDef


def get_value() -> AssociatedObjectiveSummaryTypeDef:
    return {
        "Arn": ...,
    }


# AssociatedObjectiveSummaryTypeDef definition

class AssociatedObjectiveSummaryTypeDef(TypedDict):
    Arn: NotRequired[str],
    Name: NotRequired[str],
```

## ObjectiveResourceFilterTypeDef

```python
# ObjectiveResourceFilterTypeDef TypedDict usage example

from types_aiobotocore_controlcatalog.type_defs import ObjectiveResourceFilterTypeDef


def get_value() -> ObjectiveResourceFilterTypeDef:
    return {
        "Arn": ...,
    }


# ObjectiveResourceFilterTypeDef definition

class ObjectiveResourceFilterTypeDef(TypedDict):
    Arn: NotRequired[str],
```

## ControlParameterTypeDef

```python
# ControlParameterTypeDef TypedDict usage example

from types_aiobotocore_controlcatalog.type_defs import ControlParameterTypeDef


def get_value() -> ControlParameterTypeDef:
    return {
        "Name": ...,
    }


# ControlParameterTypeDef definition

class ControlParameterTypeDef(TypedDict):
    Name: str,
```

## ControlSummaryTypeDef

```python
# ControlSummaryTypeDef TypedDict usage example

from types_aiobotocore_controlcatalog.type_defs import ControlSummaryTypeDef


def get_value() -> ControlSummaryTypeDef:
    return {
        "Arn": ...,
    }


# ControlSummaryTypeDef definition

class ControlSummaryTypeDef(TypedDict):
    Arn: str,
    Name: str,
    Description: str,
```

## DomainResourceFilterTypeDef

```python
# DomainResourceFilterTypeDef TypedDict usage example

from types_aiobotocore_controlcatalog.type_defs import DomainResourceFilterTypeDef


def get_value() -> DomainResourceFilterTypeDef:
    return {
        "Arn": ...,
    }


# DomainResourceFilterTypeDef definition

class DomainResourceFilterTypeDef(TypedDict):
    Arn: NotRequired[str],
```

## DomainSummaryTypeDef

```python
# DomainSummaryTypeDef TypedDict usage example

from types_aiobotocore_controlcatalog.type_defs import DomainSummaryTypeDef


def get_value() -> DomainSummaryTypeDef:
    return {
        "Arn": ...,
    }


# DomainSummaryTypeDef definition

class DomainSummaryTypeDef(TypedDict):
    Arn: str,
    Name: str,
    Description: str,
    CreateTime: datetime,
    LastUpdateTime: datetime,
```

## GetControlRequestTypeDef

```python
# GetControlRequestTypeDef TypedDict usage example

from types_aiobotocore_controlcatalog.type_defs import GetControlRequestTypeDef


def get_value() -> GetControlRequestTypeDef:
    return {
        "ControlArn": ...,
    }


# GetControlRequestTypeDef definition

class GetControlRequestTypeDef(TypedDict):
    ControlArn: str,
```

## ImplementationDetailsTypeDef

```python
# ImplementationDetailsTypeDef TypedDict usage example

from types_aiobotocore_controlcatalog.type_defs import ImplementationDetailsTypeDef


def get_value() -> ImplementationDetailsTypeDef:
    return {
        "Type": ...,
    }


# ImplementationDetailsTypeDef definition

class ImplementationDetailsTypeDef(TypedDict):
    Type: str,
```

## RegionConfigurationTypeDef

```python
# RegionConfigurationTypeDef TypedDict usage example

from types_aiobotocore_controlcatalog.type_defs import RegionConfigurationTypeDef


def get_value() -> RegionConfigurationTypeDef:
    return {
        "Scope": ...,
    }


# RegionConfigurationTypeDef definition

class RegionConfigurationTypeDef(TypedDict):
    Scope: ControlScopeType,  # (1)
    DeployableRegions: NotRequired[List[str]],
```

1. See [:material-code-brackets: ControlScopeType](./literals.md#controlscopetype) 
## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_controlcatalog.type_defs import ResponseMetadataTypeDef


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

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef TypedDict usage example

from types_aiobotocore_controlcatalog.type_defs import PaginatorConfigTypeDef


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

## ListControlsRequestTypeDef

```python
# ListControlsRequestTypeDef TypedDict usage example

from types_aiobotocore_controlcatalog.type_defs import ListControlsRequestTypeDef


def get_value() -> ListControlsRequestTypeDef:
    return {
        "NextToken": ...,
    }


# ListControlsRequestTypeDef definition

class ListControlsRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListDomainsRequestTypeDef

```python
# ListDomainsRequestTypeDef TypedDict usage example

from types_aiobotocore_controlcatalog.type_defs import ListDomainsRequestTypeDef


def get_value() -> ListDomainsRequestTypeDef:
    return {
        "MaxResults": ...,
    }


# ListDomainsRequestTypeDef definition

class ListDomainsRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ObjectiveSummaryTypeDef

```python
# ObjectiveSummaryTypeDef TypedDict usage example

from types_aiobotocore_controlcatalog.type_defs import ObjectiveSummaryTypeDef


def get_value() -> ObjectiveSummaryTypeDef:
    return {
        "Arn": ...,
    }


# ObjectiveSummaryTypeDef definition

class ObjectiveSummaryTypeDef(TypedDict):
    Arn: str,
    Name: str,
    Description: str,
    Domain: AssociatedDomainSummaryTypeDef,  # (1)
    CreateTime: datetime,
    LastUpdateTime: datetime,
```

1. See [:material-code-braces: AssociatedDomainSummaryTypeDef](./type_defs.md#associateddomainsummarytypedef) 
## CommonControlSummaryTypeDef

```python
# CommonControlSummaryTypeDef TypedDict usage example

from types_aiobotocore_controlcatalog.type_defs import CommonControlSummaryTypeDef


def get_value() -> CommonControlSummaryTypeDef:
    return {
        "Arn": ...,
    }


# CommonControlSummaryTypeDef definition

class CommonControlSummaryTypeDef(TypedDict):
    Arn: str,
    Name: str,
    Description: str,
    Domain: AssociatedDomainSummaryTypeDef,  # (1)
    Objective: AssociatedObjectiveSummaryTypeDef,  # (2)
    CreateTime: datetime,
    LastUpdateTime: datetime,
```

1. See [:material-code-braces: AssociatedDomainSummaryTypeDef](./type_defs.md#associateddomainsummarytypedef) 
2. See [:material-code-braces: AssociatedObjectiveSummaryTypeDef](./type_defs.md#associatedobjectivesummarytypedef) 
## CommonControlFilterTypeDef

```python
# CommonControlFilterTypeDef TypedDict usage example

from types_aiobotocore_controlcatalog.type_defs import CommonControlFilterTypeDef


def get_value() -> CommonControlFilterTypeDef:
    return {
        "Objectives": ...,
    }


# CommonControlFilterTypeDef definition

class CommonControlFilterTypeDef(TypedDict):
    Objectives: NotRequired[Sequence[ObjectiveResourceFilterTypeDef]],  # (1)
```

1. See [:material-code-braces: ObjectiveResourceFilterTypeDef](./type_defs.md#objectiveresourcefiltertypedef) 
## ObjectiveFilterTypeDef

```python
# ObjectiveFilterTypeDef TypedDict usage example

from types_aiobotocore_controlcatalog.type_defs import ObjectiveFilterTypeDef


def get_value() -> ObjectiveFilterTypeDef:
    return {
        "Domains": ...,
    }


# ObjectiveFilterTypeDef definition

class ObjectiveFilterTypeDef(TypedDict):
    Domains: NotRequired[Sequence[DomainResourceFilterTypeDef]],  # (1)
```

1. See [:material-code-braces: DomainResourceFilterTypeDef](./type_defs.md#domainresourcefiltertypedef) 
## GetControlResponseTypeDef

```python
# GetControlResponseTypeDef TypedDict usage example

from types_aiobotocore_controlcatalog.type_defs import GetControlResponseTypeDef


def get_value() -> GetControlResponseTypeDef:
    return {
        "Arn": ...,
    }


# GetControlResponseTypeDef definition

class GetControlResponseTypeDef(TypedDict):
    Arn: str,
    Name: str,
    Description: str,
    Behavior: ControlBehaviorType,  # (1)
    RegionConfiguration: RegionConfigurationTypeDef,  # (2)
    Implementation: ImplementationDetailsTypeDef,  # (3)
    Parameters: List[ControlParameterTypeDef],  # (4)
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-brackets: ControlBehaviorType](./literals.md#controlbehaviortype) 
2. See [:material-code-braces: RegionConfigurationTypeDef](./type_defs.md#regionconfigurationtypedef) 
3. See [:material-code-braces: ImplementationDetailsTypeDef](./type_defs.md#implementationdetailstypedef) 
4. See [:material-code-braces: ControlParameterTypeDef](./type_defs.md#controlparametertypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListControlsResponseTypeDef

```python
# ListControlsResponseTypeDef TypedDict usage example

from types_aiobotocore_controlcatalog.type_defs import ListControlsResponseTypeDef


def get_value() -> ListControlsResponseTypeDef:
    return {
        "Controls": ...,
    }


# ListControlsResponseTypeDef definition

class ListControlsResponseTypeDef(TypedDict):
    Controls: List[ControlSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ControlSummaryTypeDef](./type_defs.md#controlsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDomainsResponseTypeDef

```python
# ListDomainsResponseTypeDef TypedDict usage example

from types_aiobotocore_controlcatalog.type_defs import ListDomainsResponseTypeDef


def get_value() -> ListDomainsResponseTypeDef:
    return {
        "Domains": ...,
    }


# ListDomainsResponseTypeDef definition

class ListDomainsResponseTypeDef(TypedDict):
    Domains: List[DomainSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: DomainSummaryTypeDef](./type_defs.md#domainsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListControlsRequestPaginateTypeDef

```python
# ListControlsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_controlcatalog.type_defs import ListControlsRequestPaginateTypeDef


def get_value() -> ListControlsRequestPaginateTypeDef:
    return {
        "PaginationConfig": ...,
    }


# ListControlsRequestPaginateTypeDef definition

class ListControlsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDomainsRequestPaginateTypeDef

```python
# ListDomainsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_controlcatalog.type_defs import ListDomainsRequestPaginateTypeDef


def get_value() -> ListDomainsRequestPaginateTypeDef:
    return {
        "PaginationConfig": ...,
    }


# ListDomainsRequestPaginateTypeDef definition

class ListDomainsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListObjectivesResponseTypeDef

```python
# ListObjectivesResponseTypeDef TypedDict usage example

from types_aiobotocore_controlcatalog.type_defs import ListObjectivesResponseTypeDef


def get_value() -> ListObjectivesResponseTypeDef:
    return {
        "Objectives": ...,
    }


# ListObjectivesResponseTypeDef definition

class ListObjectivesResponseTypeDef(TypedDict):
    Objectives: List[ObjectiveSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ObjectiveSummaryTypeDef](./type_defs.md#objectivesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListCommonControlsResponseTypeDef

```python
# ListCommonControlsResponseTypeDef TypedDict usage example

from types_aiobotocore_controlcatalog.type_defs import ListCommonControlsResponseTypeDef


def get_value() -> ListCommonControlsResponseTypeDef:
    return {
        "CommonControls": ...,
    }


# ListCommonControlsResponseTypeDef definition

class ListCommonControlsResponseTypeDef(TypedDict):
    CommonControls: List[CommonControlSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: CommonControlSummaryTypeDef](./type_defs.md#commoncontrolsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListCommonControlsRequestPaginateTypeDef

```python
# ListCommonControlsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_controlcatalog.type_defs import ListCommonControlsRequestPaginateTypeDef


def get_value() -> ListCommonControlsRequestPaginateTypeDef:
    return {
        "CommonControlFilter": ...,
    }


# ListCommonControlsRequestPaginateTypeDef definition

class ListCommonControlsRequestPaginateTypeDef(TypedDict):
    CommonControlFilter: NotRequired[CommonControlFilterTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: CommonControlFilterTypeDef](./type_defs.md#commoncontrolfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListCommonControlsRequestTypeDef

```python
# ListCommonControlsRequestTypeDef TypedDict usage example

from types_aiobotocore_controlcatalog.type_defs import ListCommonControlsRequestTypeDef


def get_value() -> ListCommonControlsRequestTypeDef:
    return {
        "MaxResults": ...,
    }


# ListCommonControlsRequestTypeDef definition

class ListCommonControlsRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    CommonControlFilter: NotRequired[CommonControlFilterTypeDef],  # (1)
```

1. See [:material-code-braces: CommonControlFilterTypeDef](./type_defs.md#commoncontrolfiltertypedef) 
## ListObjectivesRequestPaginateTypeDef

```python
# ListObjectivesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_controlcatalog.type_defs import ListObjectivesRequestPaginateTypeDef


def get_value() -> ListObjectivesRequestPaginateTypeDef:
    return {
        "ObjectiveFilter": ...,
    }


# ListObjectivesRequestPaginateTypeDef definition

class ListObjectivesRequestPaginateTypeDef(TypedDict):
    ObjectiveFilter: NotRequired[ObjectiveFilterTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: ObjectiveFilterTypeDef](./type_defs.md#objectivefiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListObjectivesRequestTypeDef

```python
# ListObjectivesRequestTypeDef TypedDict usage example

from types_aiobotocore_controlcatalog.type_defs import ListObjectivesRequestTypeDef


def get_value() -> ListObjectivesRequestTypeDef:
    return {
        "MaxResults": ...,
    }


# ListObjectivesRequestTypeDef definition

class ListObjectivesRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    ObjectiveFilter: NotRequired[ObjectiveFilterTypeDef],  # (1)
```

1. See [:material-code-braces: ObjectiveFilterTypeDef](./type_defs.md#objectivefiltertypedef) 
