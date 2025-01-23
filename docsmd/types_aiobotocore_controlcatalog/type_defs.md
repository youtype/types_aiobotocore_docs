# Type definitions

> [Index](../README.md) > [ControlCatalog](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [ControlCatalog](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controlcatalog.html#controlcatalog)
    type annotations stubs module [types-aiobotocore-controlcatalog](https://pypi.org/project/types-aiobotocore-controlcatalog/).



## AssociatedDomainSummaryTypeDef

```python
# AssociatedDomainSummaryTypeDef definition

class AssociatedDomainSummaryTypeDef(TypedDict):
    Arn: NotRequired[str],
    Name: NotRequired[str],
```

## AssociatedObjectiveSummaryTypeDef

```python
# AssociatedObjectiveSummaryTypeDef definition

class AssociatedObjectiveSummaryTypeDef(TypedDict):
    Arn: NotRequired[str],
    Name: NotRequired[str],
```

## ObjectiveResourceFilterTypeDef

```python
# ObjectiveResourceFilterTypeDef definition

class ObjectiveResourceFilterTypeDef(TypedDict):
    Arn: NotRequired[str],
```

## ControlParameterTypeDef

```python
# ControlParameterTypeDef definition

class ControlParameterTypeDef(TypedDict):
    Name: str,
```

## ControlSummaryTypeDef

```python
# ControlSummaryTypeDef definition

class ControlSummaryTypeDef(TypedDict):
    Arn: str,
    Name: str,
    Description: str,
```

## DomainResourceFilterTypeDef

```python
# DomainResourceFilterTypeDef definition

class DomainResourceFilterTypeDef(TypedDict):
    Arn: NotRequired[str],
```

## DomainSummaryTypeDef

```python
# DomainSummaryTypeDef definition

class DomainSummaryTypeDef(TypedDict):
    Arn: str,
    Name: str,
    Description: str,
    CreateTime: datetime,
    LastUpdateTime: datetime,
```

## GetControlRequestRequestTypeDef

```python
# GetControlRequestRequestTypeDef definition

class GetControlRequestRequestTypeDef(TypedDict):
    ControlArn: str,
```

## ImplementationDetailsTypeDef

```python
# ImplementationDetailsTypeDef definition

class ImplementationDetailsTypeDef(TypedDict):
    Type: str,
```

## RegionConfigurationTypeDef

```python
# RegionConfigurationTypeDef definition

class RegionConfigurationTypeDef(TypedDict):
    Scope: ControlScopeType,  # (1)
    DeployableRegions: NotRequired[List[str]],
```

1. See [:material-code-brackets: ControlScopeType](./literals.md#controlscopetype) 
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

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListControlsRequestRequestTypeDef

```python
# ListControlsRequestRequestTypeDef definition

class ListControlsRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListDomainsRequestRequestTypeDef

```python
# ListDomainsRequestRequestTypeDef definition

class ListDomainsRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ObjectiveSummaryTypeDef

```python
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
# CommonControlFilterTypeDef definition

class CommonControlFilterTypeDef(TypedDict):
    Objectives: NotRequired[Sequence[ObjectiveResourceFilterTypeDef]],  # (1)
```

1. See [:material-code-braces: ObjectiveResourceFilterTypeDef](./type_defs.md#objectiveresourcefiltertypedef) 
## ObjectiveFilterTypeDef

```python
# ObjectiveFilterTypeDef definition

class ObjectiveFilterTypeDef(TypedDict):
    Domains: NotRequired[Sequence[DomainResourceFilterTypeDef]],  # (1)
```

1. See [:material-code-braces: DomainResourceFilterTypeDef](./type_defs.md#domainresourcefiltertypedef) 
## GetControlResponseTypeDef

```python
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
# ListControlsRequestPaginateTypeDef definition

class ListControlsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDomainsRequestPaginateTypeDef

```python
# ListDomainsRequestPaginateTypeDef definition

class ListDomainsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListObjectivesResponseTypeDef

```python
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
# ListCommonControlsRequestPaginateTypeDef definition

class ListCommonControlsRequestPaginateTypeDef(TypedDict):
    CommonControlFilter: NotRequired[CommonControlFilterTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: CommonControlFilterTypeDef](./type_defs.md#commoncontrolfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListCommonControlsRequestRequestTypeDef

```python
# ListCommonControlsRequestRequestTypeDef definition

class ListCommonControlsRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    CommonControlFilter: NotRequired[CommonControlFilterTypeDef],  # (1)
```

1. See [:material-code-braces: CommonControlFilterTypeDef](./type_defs.md#commoncontrolfiltertypedef) 
## ListObjectivesRequestPaginateTypeDef

```python
# ListObjectivesRequestPaginateTypeDef definition

class ListObjectivesRequestPaginateTypeDef(TypedDict):
    ObjectiveFilter: NotRequired[ObjectiveFilterTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: ObjectiveFilterTypeDef](./type_defs.md#objectivefiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListObjectivesRequestRequestTypeDef

```python
# ListObjectivesRequestRequestTypeDef definition

class ListObjectivesRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    ObjectiveFilter: NotRequired[ObjectiveFilterTypeDef],  # (1)
```

1. See [:material-code-braces: ObjectiveFilterTypeDef](./type_defs.md#objectivefiltertypedef) 
