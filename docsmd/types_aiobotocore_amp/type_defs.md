# Type definitions

> [Index](../README.md) > [PrometheusService](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [PrometheusService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#prometheusservice)
    type annotations stubs module [types-aiobotocore-amp](https://pypi.org/project/types-aiobotocore-amp/).

## BlobTypeDef

```python
# BlobTypeDef Union usage example

from types_aiobotocore_amp.type_defs import BlobTypeDef


def get_value() -> BlobTypeDef:
    return ...


# BlobTypeDef definition

BlobTypeDef = Union[
    str,
    bytes,
    IO[Any],
    StreamingBody,
]
```


## ScrapeConfigurationUnionTypeDef

```python
# ScrapeConfigurationUnionTypeDef Union usage example

from types_aiobotocore_amp.type_defs import ScrapeConfigurationUnionTypeDef


def get_value() -> ScrapeConfigurationUnionTypeDef:
    return ...


# ScrapeConfigurationUnionTypeDef definition

ScrapeConfigurationUnionTypeDef = Union[
    ScrapeConfigurationTypeDef,  # (1)
    ScrapeConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ScrapeConfigurationTypeDef](./type_defs.md#scrapeconfigurationtypedef) 
2. See [:material-code-braces: ScrapeConfigurationOutputTypeDef](./type_defs.md#scrapeconfigurationoutputtypedef) 

## SourceUnionTypeDef

```python
# SourceUnionTypeDef Union usage example

from types_aiobotocore_amp.type_defs import SourceUnionTypeDef


def get_value() -> SourceUnionTypeDef:
    return ...


# SourceUnionTypeDef definition

SourceUnionTypeDef = Union[
    SourceTypeDef,  # (1)
    SourceOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: SourceTypeDef](./type_defs.md#sourcetypedef) 
2. See [:material-code-braces: SourceOutputTypeDef](./type_defs.md#sourceoutputtypedef) 



## AlertManagerDefinitionStatusTypeDef

```python
# AlertManagerDefinitionStatusTypeDef TypedDict usage example

from types_aiobotocore_amp.type_defs import AlertManagerDefinitionStatusTypeDef


def get_value() -> AlertManagerDefinitionStatusTypeDef:
    return {
        "statusCode": ...,
    }


# AlertManagerDefinitionStatusTypeDef definition

class AlertManagerDefinitionStatusTypeDef(TypedDict):
    statusCode: AlertManagerDefinitionStatusCodeType,  # (1)
    statusReason: NotRequired[str],
```

1. See [:material-code-brackets: AlertManagerDefinitionStatusCodeType](./literals.md#alertmanagerdefinitionstatuscodetype) 
## AmpConfigurationTypeDef

```python
# AmpConfigurationTypeDef TypedDict usage example

from types_aiobotocore_amp.type_defs import AmpConfigurationTypeDef


def get_value() -> AmpConfigurationTypeDef:
    return {
        "workspaceArn": ...,
    }


# AmpConfigurationTypeDef definition

class AmpConfigurationTypeDef(TypedDict):
    workspaceArn: str,
```

## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_amp.type_defs import ResponseMetadataTypeDef


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

## CreateLoggingConfigurationRequestTypeDef

```python
# CreateLoggingConfigurationRequestTypeDef TypedDict usage example

from types_aiobotocore_amp.type_defs import CreateLoggingConfigurationRequestTypeDef


def get_value() -> CreateLoggingConfigurationRequestTypeDef:
    return {
        "logGroupArn": ...,
    }


# CreateLoggingConfigurationRequestTypeDef definition

class CreateLoggingConfigurationRequestTypeDef(TypedDict):
    logGroupArn: str,
    workspaceId: str,
    clientToken: NotRequired[str],
```

## LoggingConfigurationStatusTypeDef

```python
# LoggingConfigurationStatusTypeDef TypedDict usage example

from types_aiobotocore_amp.type_defs import LoggingConfigurationStatusTypeDef


def get_value() -> LoggingConfigurationStatusTypeDef:
    return {
        "statusCode": ...,
    }


# LoggingConfigurationStatusTypeDef definition

class LoggingConfigurationStatusTypeDef(TypedDict):
    statusCode: LoggingConfigurationStatusCodeType,  # (1)
    statusReason: NotRequired[str],
```

1. See [:material-code-brackets: LoggingConfigurationStatusCodeType](./literals.md#loggingconfigurationstatuscodetype) 
## RuleGroupsNamespaceStatusTypeDef

```python
# RuleGroupsNamespaceStatusTypeDef TypedDict usage example

from types_aiobotocore_amp.type_defs import RuleGroupsNamespaceStatusTypeDef


def get_value() -> RuleGroupsNamespaceStatusTypeDef:
    return {
        "statusCode": ...,
    }


# RuleGroupsNamespaceStatusTypeDef definition

class RuleGroupsNamespaceStatusTypeDef(TypedDict):
    statusCode: RuleGroupsNamespaceStatusCodeType,  # (1)
    statusReason: NotRequired[str],
```

1. See [:material-code-brackets: RuleGroupsNamespaceStatusCodeType](./literals.md#rulegroupsnamespacestatuscodetype) 
## RoleConfigurationTypeDef

```python
# RoleConfigurationTypeDef TypedDict usage example

from types_aiobotocore_amp.type_defs import RoleConfigurationTypeDef


def get_value() -> RoleConfigurationTypeDef:
    return {
        "sourceRoleArn": ...,
    }


# RoleConfigurationTypeDef definition

class RoleConfigurationTypeDef(TypedDict):
    sourceRoleArn: NotRequired[str],
    targetRoleArn: NotRequired[str],
```

## ScraperStatusTypeDef

```python
# ScraperStatusTypeDef TypedDict usage example

from types_aiobotocore_amp.type_defs import ScraperStatusTypeDef


def get_value() -> ScraperStatusTypeDef:
    return {
        "statusCode": ...,
    }


# ScraperStatusTypeDef definition

class ScraperStatusTypeDef(TypedDict):
    statusCode: ScraperStatusCodeType,  # (1)
```

1. See [:material-code-brackets: ScraperStatusCodeType](./literals.md#scraperstatuscodetype) 
## CreateWorkspaceRequestTypeDef

```python
# CreateWorkspaceRequestTypeDef TypedDict usage example

from types_aiobotocore_amp.type_defs import CreateWorkspaceRequestTypeDef


def get_value() -> CreateWorkspaceRequestTypeDef:
    return {
        "alias": ...,
    }


# CreateWorkspaceRequestTypeDef definition

class CreateWorkspaceRequestTypeDef(TypedDict):
    alias: NotRequired[str],
    clientToken: NotRequired[str],
    kmsKeyArn: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

## WorkspaceStatusTypeDef

```python
# WorkspaceStatusTypeDef TypedDict usage example

from types_aiobotocore_amp.type_defs import WorkspaceStatusTypeDef


def get_value() -> WorkspaceStatusTypeDef:
    return {
        "statusCode": ...,
    }


# WorkspaceStatusTypeDef definition

class WorkspaceStatusTypeDef(TypedDict):
    statusCode: WorkspaceStatusCodeType,  # (1)
```

1. See [:material-code-brackets: WorkspaceStatusCodeType](./literals.md#workspacestatuscodetype) 
## DeleteAlertManagerDefinitionRequestTypeDef

```python
# DeleteAlertManagerDefinitionRequestTypeDef TypedDict usage example

from types_aiobotocore_amp.type_defs import DeleteAlertManagerDefinitionRequestTypeDef


def get_value() -> DeleteAlertManagerDefinitionRequestTypeDef:
    return {
        "workspaceId": ...,
    }


# DeleteAlertManagerDefinitionRequestTypeDef definition

class DeleteAlertManagerDefinitionRequestTypeDef(TypedDict):
    workspaceId: str,
    clientToken: NotRequired[str],
```

## DeleteLoggingConfigurationRequestTypeDef

```python
# DeleteLoggingConfigurationRequestTypeDef TypedDict usage example

from types_aiobotocore_amp.type_defs import DeleteLoggingConfigurationRequestTypeDef


def get_value() -> DeleteLoggingConfigurationRequestTypeDef:
    return {
        "workspaceId": ...,
    }


# DeleteLoggingConfigurationRequestTypeDef definition

class DeleteLoggingConfigurationRequestTypeDef(TypedDict):
    workspaceId: str,
    clientToken: NotRequired[str],
```

## DeleteRuleGroupsNamespaceRequestTypeDef

```python
# DeleteRuleGroupsNamespaceRequestTypeDef TypedDict usage example

from types_aiobotocore_amp.type_defs import DeleteRuleGroupsNamespaceRequestTypeDef


def get_value() -> DeleteRuleGroupsNamespaceRequestTypeDef:
    return {
        "name": ...,
    }


# DeleteRuleGroupsNamespaceRequestTypeDef definition

class DeleteRuleGroupsNamespaceRequestTypeDef(TypedDict):
    name: str,
    workspaceId: str,
    clientToken: NotRequired[str],
```

## DeleteScraperRequestTypeDef

```python
# DeleteScraperRequestTypeDef TypedDict usage example

from types_aiobotocore_amp.type_defs import DeleteScraperRequestTypeDef


def get_value() -> DeleteScraperRequestTypeDef:
    return {
        "scraperId": ...,
    }


# DeleteScraperRequestTypeDef definition

class DeleteScraperRequestTypeDef(TypedDict):
    scraperId: str,
    clientToken: NotRequired[str],
```

## DeleteWorkspaceRequestTypeDef

```python
# DeleteWorkspaceRequestTypeDef TypedDict usage example

from types_aiobotocore_amp.type_defs import DeleteWorkspaceRequestTypeDef


def get_value() -> DeleteWorkspaceRequestTypeDef:
    return {
        "workspaceId": ...,
    }


# DeleteWorkspaceRequestTypeDef definition

class DeleteWorkspaceRequestTypeDef(TypedDict):
    workspaceId: str,
    clientToken: NotRequired[str],
```

## DescribeAlertManagerDefinitionRequestTypeDef

```python
# DescribeAlertManagerDefinitionRequestTypeDef TypedDict usage example

from types_aiobotocore_amp.type_defs import DescribeAlertManagerDefinitionRequestTypeDef


def get_value() -> DescribeAlertManagerDefinitionRequestTypeDef:
    return {
        "workspaceId": ...,
    }


# DescribeAlertManagerDefinitionRequestTypeDef definition

class DescribeAlertManagerDefinitionRequestTypeDef(TypedDict):
    workspaceId: str,
```

## DescribeLoggingConfigurationRequestTypeDef

```python
# DescribeLoggingConfigurationRequestTypeDef TypedDict usage example

from types_aiobotocore_amp.type_defs import DescribeLoggingConfigurationRequestTypeDef


def get_value() -> DescribeLoggingConfigurationRequestTypeDef:
    return {
        "workspaceId": ...,
    }


# DescribeLoggingConfigurationRequestTypeDef definition

class DescribeLoggingConfigurationRequestTypeDef(TypedDict):
    workspaceId: str,
```

## DescribeRuleGroupsNamespaceRequestTypeDef

```python
# DescribeRuleGroupsNamespaceRequestTypeDef TypedDict usage example

from types_aiobotocore_amp.type_defs import DescribeRuleGroupsNamespaceRequestTypeDef


def get_value() -> DescribeRuleGroupsNamespaceRequestTypeDef:
    return {
        "name": ...,
    }


# DescribeRuleGroupsNamespaceRequestTypeDef definition

class DescribeRuleGroupsNamespaceRequestTypeDef(TypedDict):
    name: str,
    workspaceId: str,
```

## DescribeScraperRequestTypeDef

```python
# DescribeScraperRequestTypeDef TypedDict usage example

from types_aiobotocore_amp.type_defs import DescribeScraperRequestTypeDef


def get_value() -> DescribeScraperRequestTypeDef:
    return {
        "scraperId": ...,
    }


# DescribeScraperRequestTypeDef definition

class DescribeScraperRequestTypeDef(TypedDict):
    scraperId: str,
```

## WaiterConfigTypeDef

```python
# WaiterConfigTypeDef TypedDict usage example

from types_aiobotocore_amp.type_defs import WaiterConfigTypeDef


def get_value() -> WaiterConfigTypeDef:
    return {
        "Delay": ...,
    }


# WaiterConfigTypeDef definition

class WaiterConfigTypeDef(TypedDict):
    Delay: NotRequired[int],
    MaxAttempts: NotRequired[int],
```

## DescribeWorkspaceRequestTypeDef

```python
# DescribeWorkspaceRequestTypeDef TypedDict usage example

from types_aiobotocore_amp.type_defs import DescribeWorkspaceRequestTypeDef


def get_value() -> DescribeWorkspaceRequestTypeDef:
    return {
        "workspaceId": ...,
    }


# DescribeWorkspaceRequestTypeDef definition

class DescribeWorkspaceRequestTypeDef(TypedDict):
    workspaceId: str,
```

## EksConfigurationOutputTypeDef

```python
# EksConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_amp.type_defs import EksConfigurationOutputTypeDef


def get_value() -> EksConfigurationOutputTypeDef:
    return {
        "clusterArn": ...,
    }


# EksConfigurationOutputTypeDef definition

class EksConfigurationOutputTypeDef(TypedDict):
    clusterArn: str,
    subnetIds: List[str],
    securityGroupIds: NotRequired[List[str]],
```

## EksConfigurationTypeDef

```python
# EksConfigurationTypeDef TypedDict usage example

from types_aiobotocore_amp.type_defs import EksConfigurationTypeDef


def get_value() -> EksConfigurationTypeDef:
    return {
        "clusterArn": ...,
    }


# EksConfigurationTypeDef definition

class EksConfigurationTypeDef(TypedDict):
    clusterArn: str,
    subnetIds: Sequence[str],
    securityGroupIds: NotRequired[Sequence[str]],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef TypedDict usage example

from types_aiobotocore_amp.type_defs import PaginatorConfigTypeDef


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

## ListRuleGroupsNamespacesRequestTypeDef

```python
# ListRuleGroupsNamespacesRequestTypeDef TypedDict usage example

from types_aiobotocore_amp.type_defs import ListRuleGroupsNamespacesRequestTypeDef


def get_value() -> ListRuleGroupsNamespacesRequestTypeDef:
    return {
        "workspaceId": ...,
    }


# ListRuleGroupsNamespacesRequestTypeDef definition

class ListRuleGroupsNamespacesRequestTypeDef(TypedDict):
    workspaceId: str,
    maxResults: NotRequired[int],
    name: NotRequired[str],
    nextToken: NotRequired[str],
```

## ListScrapersRequestTypeDef

```python
# ListScrapersRequestTypeDef TypedDict usage example

from types_aiobotocore_amp.type_defs import ListScrapersRequestTypeDef


def get_value() -> ListScrapersRequestTypeDef:
    return {
        "filters": ...,
    }


# ListScrapersRequestTypeDef definition

class ListScrapersRequestTypeDef(TypedDict):
    filters: NotRequired[Mapping[str, Sequence[str]]],
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListTagsForResourceRequestTypeDef

```python
# ListTagsForResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_amp.type_defs import ListTagsForResourceRequestTypeDef


def get_value() -> ListTagsForResourceRequestTypeDef:
    return {
        "resourceArn": ...,
    }


# ListTagsForResourceRequestTypeDef definition

class ListTagsForResourceRequestTypeDef(TypedDict):
    resourceArn: str,
```

## ListWorkspacesRequestTypeDef

```python
# ListWorkspacesRequestTypeDef TypedDict usage example

from types_aiobotocore_amp.type_defs import ListWorkspacesRequestTypeDef


def get_value() -> ListWorkspacesRequestTypeDef:
    return {
        "alias": ...,
    }


# ListWorkspacesRequestTypeDef definition

class ListWorkspacesRequestTypeDef(TypedDict):
    alias: NotRequired[str],
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ScrapeConfigurationOutputTypeDef

```python
# ScrapeConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_amp.type_defs import ScrapeConfigurationOutputTypeDef


def get_value() -> ScrapeConfigurationOutputTypeDef:
    return {
        "configurationBlob": ...,
    }


# ScrapeConfigurationOutputTypeDef definition

class ScrapeConfigurationOutputTypeDef(TypedDict):
    configurationBlob: NotRequired[bytes],
```

## TagResourceRequestTypeDef

```python
# TagResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_amp.type_defs import TagResourceRequestTypeDef


def get_value() -> TagResourceRequestTypeDef:
    return {
        "resourceArn": ...,
    }


# TagResourceRequestTypeDef definition

class TagResourceRequestTypeDef(TypedDict):
    resourceArn: str,
    tags: Mapping[str, str],
```

## UntagResourceRequestTypeDef

```python
# UntagResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_amp.type_defs import UntagResourceRequestTypeDef


def get_value() -> UntagResourceRequestTypeDef:
    return {
        "resourceArn": ...,
    }


# UntagResourceRequestTypeDef definition

class UntagResourceRequestTypeDef(TypedDict):
    resourceArn: str,
    tagKeys: Sequence[str],
```

## UpdateLoggingConfigurationRequestTypeDef

```python
# UpdateLoggingConfigurationRequestTypeDef TypedDict usage example

from types_aiobotocore_amp.type_defs import UpdateLoggingConfigurationRequestTypeDef


def get_value() -> UpdateLoggingConfigurationRequestTypeDef:
    return {
        "logGroupArn": ...,
    }


# UpdateLoggingConfigurationRequestTypeDef definition

class UpdateLoggingConfigurationRequestTypeDef(TypedDict):
    logGroupArn: str,
    workspaceId: str,
    clientToken: NotRequired[str],
```

## UpdateWorkspaceAliasRequestTypeDef

```python
# UpdateWorkspaceAliasRequestTypeDef TypedDict usage example

from types_aiobotocore_amp.type_defs import UpdateWorkspaceAliasRequestTypeDef


def get_value() -> UpdateWorkspaceAliasRequestTypeDef:
    return {
        "workspaceId": ...,
    }


# UpdateWorkspaceAliasRequestTypeDef definition

class UpdateWorkspaceAliasRequestTypeDef(TypedDict):
    workspaceId: str,
    alias: NotRequired[str],
    clientToken: NotRequired[str],
```

## AlertManagerDefinitionDescriptionTypeDef

```python
# AlertManagerDefinitionDescriptionTypeDef TypedDict usage example

from types_aiobotocore_amp.type_defs import AlertManagerDefinitionDescriptionTypeDef


def get_value() -> AlertManagerDefinitionDescriptionTypeDef:
    return {
        "createdAt": ...,
    }


# AlertManagerDefinitionDescriptionTypeDef definition

class AlertManagerDefinitionDescriptionTypeDef(TypedDict):
    createdAt: datetime,
    data: bytes,
    modifiedAt: datetime,
    status: AlertManagerDefinitionStatusTypeDef,  # (1)
```

1. See [:material-code-braces: AlertManagerDefinitionStatusTypeDef](./type_defs.md#alertmanagerdefinitionstatustypedef) 
## DestinationTypeDef

```python
# DestinationTypeDef TypedDict usage example

from types_aiobotocore_amp.type_defs import DestinationTypeDef


def get_value() -> DestinationTypeDef:
    return {
        "ampConfiguration": ...,
    }


# DestinationTypeDef definition

class DestinationTypeDef(TypedDict):
    ampConfiguration: NotRequired[AmpConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: AmpConfigurationTypeDef](./type_defs.md#ampconfigurationtypedef) 
## CreateAlertManagerDefinitionRequestTypeDef

```python
# CreateAlertManagerDefinitionRequestTypeDef TypedDict usage example

from types_aiobotocore_amp.type_defs import CreateAlertManagerDefinitionRequestTypeDef


def get_value() -> CreateAlertManagerDefinitionRequestTypeDef:
    return {
        "data": ...,
    }


# CreateAlertManagerDefinitionRequestTypeDef definition

class CreateAlertManagerDefinitionRequestTypeDef(TypedDict):
    data: BlobTypeDef,
    workspaceId: str,
    clientToken: NotRequired[str],
```

## CreateRuleGroupsNamespaceRequestTypeDef

```python
# CreateRuleGroupsNamespaceRequestTypeDef TypedDict usage example

from types_aiobotocore_amp.type_defs import CreateRuleGroupsNamespaceRequestTypeDef


def get_value() -> CreateRuleGroupsNamespaceRequestTypeDef:
    return {
        "data": ...,
    }


# CreateRuleGroupsNamespaceRequestTypeDef definition

class CreateRuleGroupsNamespaceRequestTypeDef(TypedDict):
    data: BlobTypeDef,
    name: str,
    workspaceId: str,
    clientToken: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

## PutAlertManagerDefinitionRequestTypeDef

```python
# PutAlertManagerDefinitionRequestTypeDef TypedDict usage example

from types_aiobotocore_amp.type_defs import PutAlertManagerDefinitionRequestTypeDef


def get_value() -> PutAlertManagerDefinitionRequestTypeDef:
    return {
        "data": ...,
    }


# PutAlertManagerDefinitionRequestTypeDef definition

class PutAlertManagerDefinitionRequestTypeDef(TypedDict):
    data: BlobTypeDef,
    workspaceId: str,
    clientToken: NotRequired[str],
```

## PutRuleGroupsNamespaceRequestTypeDef

```python
# PutRuleGroupsNamespaceRequestTypeDef TypedDict usage example

from types_aiobotocore_amp.type_defs import PutRuleGroupsNamespaceRequestTypeDef


def get_value() -> PutRuleGroupsNamespaceRequestTypeDef:
    return {
        "data": ...,
    }


# PutRuleGroupsNamespaceRequestTypeDef definition

class PutRuleGroupsNamespaceRequestTypeDef(TypedDict):
    data: BlobTypeDef,
    name: str,
    workspaceId: str,
    clientToken: NotRequired[str],
```

## ScrapeConfigurationTypeDef

```python
# ScrapeConfigurationTypeDef TypedDict usage example

from types_aiobotocore_amp.type_defs import ScrapeConfigurationTypeDef


def get_value() -> ScrapeConfigurationTypeDef:
    return {
        "configurationBlob": ...,
    }


# ScrapeConfigurationTypeDef definition

class ScrapeConfigurationTypeDef(TypedDict):
    configurationBlob: NotRequired[BlobTypeDef],
```

## CreateAlertManagerDefinitionResponseTypeDef

```python
# CreateAlertManagerDefinitionResponseTypeDef TypedDict usage example

from types_aiobotocore_amp.type_defs import CreateAlertManagerDefinitionResponseTypeDef


def get_value() -> CreateAlertManagerDefinitionResponseTypeDef:
    return {
        "status": ...,
    }


# CreateAlertManagerDefinitionResponseTypeDef definition

class CreateAlertManagerDefinitionResponseTypeDef(TypedDict):
    status: AlertManagerDefinitionStatusTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AlertManagerDefinitionStatusTypeDef](./type_defs.md#alertmanagerdefinitionstatustypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EmptyResponseMetadataTypeDef

```python
# EmptyResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_amp.type_defs import EmptyResponseMetadataTypeDef


def get_value() -> EmptyResponseMetadataTypeDef:
    return {
        "ResponseMetadata": ...,
    }


# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetDefaultScraperConfigurationResponseTypeDef

```python
# GetDefaultScraperConfigurationResponseTypeDef TypedDict usage example

from types_aiobotocore_amp.type_defs import GetDefaultScraperConfigurationResponseTypeDef


def get_value() -> GetDefaultScraperConfigurationResponseTypeDef:
    return {
        "configuration": ...,
    }


# GetDefaultScraperConfigurationResponseTypeDef definition

class GetDefaultScraperConfigurationResponseTypeDef(TypedDict):
    configuration: bytes,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef TypedDict usage example

from types_aiobotocore_amp.type_defs import ListTagsForResourceResponseTypeDef


def get_value() -> ListTagsForResourceResponseTypeDef:
    return {
        "tags": ...,
    }


# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutAlertManagerDefinitionResponseTypeDef

```python
# PutAlertManagerDefinitionResponseTypeDef TypedDict usage example

from types_aiobotocore_amp.type_defs import PutAlertManagerDefinitionResponseTypeDef


def get_value() -> PutAlertManagerDefinitionResponseTypeDef:
    return {
        "status": ...,
    }


# PutAlertManagerDefinitionResponseTypeDef definition

class PutAlertManagerDefinitionResponseTypeDef(TypedDict):
    status: AlertManagerDefinitionStatusTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AlertManagerDefinitionStatusTypeDef](./type_defs.md#alertmanagerdefinitionstatustypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateLoggingConfigurationResponseTypeDef

```python
# CreateLoggingConfigurationResponseTypeDef TypedDict usage example

from types_aiobotocore_amp.type_defs import CreateLoggingConfigurationResponseTypeDef


def get_value() -> CreateLoggingConfigurationResponseTypeDef:
    return {
        "status": ...,
    }


# CreateLoggingConfigurationResponseTypeDef definition

class CreateLoggingConfigurationResponseTypeDef(TypedDict):
    status: LoggingConfigurationStatusTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LoggingConfigurationStatusTypeDef](./type_defs.md#loggingconfigurationstatustypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## LoggingConfigurationMetadataTypeDef

```python
# LoggingConfigurationMetadataTypeDef TypedDict usage example

from types_aiobotocore_amp.type_defs import LoggingConfigurationMetadataTypeDef


def get_value() -> LoggingConfigurationMetadataTypeDef:
    return {
        "createdAt": ...,
    }


# LoggingConfigurationMetadataTypeDef definition

class LoggingConfigurationMetadataTypeDef(TypedDict):
    createdAt: datetime,
    logGroupArn: str,
    modifiedAt: datetime,
    status: LoggingConfigurationStatusTypeDef,  # (1)
    workspace: str,
```

1. See [:material-code-braces: LoggingConfigurationStatusTypeDef](./type_defs.md#loggingconfigurationstatustypedef) 
## UpdateLoggingConfigurationResponseTypeDef

```python
# UpdateLoggingConfigurationResponseTypeDef TypedDict usage example

from types_aiobotocore_amp.type_defs import UpdateLoggingConfigurationResponseTypeDef


def get_value() -> UpdateLoggingConfigurationResponseTypeDef:
    return {
        "status": ...,
    }


# UpdateLoggingConfigurationResponseTypeDef definition

class UpdateLoggingConfigurationResponseTypeDef(TypedDict):
    status: LoggingConfigurationStatusTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LoggingConfigurationStatusTypeDef](./type_defs.md#loggingconfigurationstatustypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateRuleGroupsNamespaceResponseTypeDef

```python
# CreateRuleGroupsNamespaceResponseTypeDef TypedDict usage example

from types_aiobotocore_amp.type_defs import CreateRuleGroupsNamespaceResponseTypeDef


def get_value() -> CreateRuleGroupsNamespaceResponseTypeDef:
    return {
        "arn": ...,
    }


# CreateRuleGroupsNamespaceResponseTypeDef definition

class CreateRuleGroupsNamespaceResponseTypeDef(TypedDict):
    arn: str,
    name: str,
    status: RuleGroupsNamespaceStatusTypeDef,  # (1)
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RuleGroupsNamespaceStatusTypeDef](./type_defs.md#rulegroupsnamespacestatustypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutRuleGroupsNamespaceResponseTypeDef

```python
# PutRuleGroupsNamespaceResponseTypeDef TypedDict usage example

from types_aiobotocore_amp.type_defs import PutRuleGroupsNamespaceResponseTypeDef


def get_value() -> PutRuleGroupsNamespaceResponseTypeDef:
    return {
        "arn": ...,
    }


# PutRuleGroupsNamespaceResponseTypeDef definition

class PutRuleGroupsNamespaceResponseTypeDef(TypedDict):
    arn: str,
    name: str,
    status: RuleGroupsNamespaceStatusTypeDef,  # (1)
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RuleGroupsNamespaceStatusTypeDef](./type_defs.md#rulegroupsnamespacestatustypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RuleGroupsNamespaceDescriptionTypeDef

```python
# RuleGroupsNamespaceDescriptionTypeDef TypedDict usage example

from types_aiobotocore_amp.type_defs import RuleGroupsNamespaceDescriptionTypeDef


def get_value() -> RuleGroupsNamespaceDescriptionTypeDef:
    return {
        "arn": ...,
    }


# RuleGroupsNamespaceDescriptionTypeDef definition

class RuleGroupsNamespaceDescriptionTypeDef(TypedDict):
    arn: str,
    createdAt: datetime,
    data: bytes,
    modifiedAt: datetime,
    name: str,
    status: RuleGroupsNamespaceStatusTypeDef,  # (1)
    tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-braces: RuleGroupsNamespaceStatusTypeDef](./type_defs.md#rulegroupsnamespacestatustypedef) 
## RuleGroupsNamespaceSummaryTypeDef

```python
# RuleGroupsNamespaceSummaryTypeDef TypedDict usage example

from types_aiobotocore_amp.type_defs import RuleGroupsNamespaceSummaryTypeDef


def get_value() -> RuleGroupsNamespaceSummaryTypeDef:
    return {
        "arn": ...,
    }


# RuleGroupsNamespaceSummaryTypeDef definition

class RuleGroupsNamespaceSummaryTypeDef(TypedDict):
    arn: str,
    createdAt: datetime,
    modifiedAt: datetime,
    name: str,
    status: RuleGroupsNamespaceStatusTypeDef,  # (1)
    tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-braces: RuleGroupsNamespaceStatusTypeDef](./type_defs.md#rulegroupsnamespacestatustypedef) 
## CreateScraperResponseTypeDef

```python
# CreateScraperResponseTypeDef TypedDict usage example

from types_aiobotocore_amp.type_defs import CreateScraperResponseTypeDef


def get_value() -> CreateScraperResponseTypeDef:
    return {
        "arn": ...,
    }


# CreateScraperResponseTypeDef definition

class CreateScraperResponseTypeDef(TypedDict):
    arn: str,
    scraperId: str,
    status: ScraperStatusTypeDef,  # (1)
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ScraperStatusTypeDef](./type_defs.md#scraperstatustypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteScraperResponseTypeDef

```python
# DeleteScraperResponseTypeDef TypedDict usage example

from types_aiobotocore_amp.type_defs import DeleteScraperResponseTypeDef


def get_value() -> DeleteScraperResponseTypeDef:
    return {
        "scraperId": ...,
    }


# DeleteScraperResponseTypeDef definition

class DeleteScraperResponseTypeDef(TypedDict):
    scraperId: str,
    status: ScraperStatusTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ScraperStatusTypeDef](./type_defs.md#scraperstatustypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateScraperResponseTypeDef

```python
# UpdateScraperResponseTypeDef TypedDict usage example

from types_aiobotocore_amp.type_defs import UpdateScraperResponseTypeDef


def get_value() -> UpdateScraperResponseTypeDef:
    return {
        "arn": ...,
    }


# UpdateScraperResponseTypeDef definition

class UpdateScraperResponseTypeDef(TypedDict):
    arn: str,
    scraperId: str,
    status: ScraperStatusTypeDef,  # (1)
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ScraperStatusTypeDef](./type_defs.md#scraperstatustypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateWorkspaceResponseTypeDef

```python
# CreateWorkspaceResponseTypeDef TypedDict usage example

from types_aiobotocore_amp.type_defs import CreateWorkspaceResponseTypeDef


def get_value() -> CreateWorkspaceResponseTypeDef:
    return {
        "arn": ...,
    }


# CreateWorkspaceResponseTypeDef definition

class CreateWorkspaceResponseTypeDef(TypedDict):
    arn: str,
    kmsKeyArn: str,
    status: WorkspaceStatusTypeDef,  # (1)
    tags: Dict[str, str],
    workspaceId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: WorkspaceStatusTypeDef](./type_defs.md#workspacestatustypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## WorkspaceDescriptionTypeDef

```python
# WorkspaceDescriptionTypeDef TypedDict usage example

from types_aiobotocore_amp.type_defs import WorkspaceDescriptionTypeDef


def get_value() -> WorkspaceDescriptionTypeDef:
    return {
        "alias": ...,
    }


# WorkspaceDescriptionTypeDef definition

class WorkspaceDescriptionTypeDef(TypedDict):
    arn: str,
    createdAt: datetime,
    status: WorkspaceStatusTypeDef,  # (1)
    workspaceId: str,
    alias: NotRequired[str],
    kmsKeyArn: NotRequired[str],
    prometheusEndpoint: NotRequired[str],
    tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-braces: WorkspaceStatusTypeDef](./type_defs.md#workspacestatustypedef) 
## WorkspaceSummaryTypeDef

```python
# WorkspaceSummaryTypeDef TypedDict usage example

from types_aiobotocore_amp.type_defs import WorkspaceSummaryTypeDef


def get_value() -> WorkspaceSummaryTypeDef:
    return {
        "alias": ...,
    }


# WorkspaceSummaryTypeDef definition

class WorkspaceSummaryTypeDef(TypedDict):
    arn: str,
    createdAt: datetime,
    status: WorkspaceStatusTypeDef,  # (1)
    workspaceId: str,
    alias: NotRequired[str],
    kmsKeyArn: NotRequired[str],
    tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-braces: WorkspaceStatusTypeDef](./type_defs.md#workspacestatustypedef) 
## DescribeScraperRequestWaitExtraTypeDef

```python
# DescribeScraperRequestWaitExtraTypeDef TypedDict usage example

from types_aiobotocore_amp.type_defs import DescribeScraperRequestWaitExtraTypeDef


def get_value() -> DescribeScraperRequestWaitExtraTypeDef:
    return {
        "scraperId": ...,
    }


# DescribeScraperRequestWaitExtraTypeDef definition

class DescribeScraperRequestWaitExtraTypeDef(TypedDict):
    scraperId: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeScraperRequestWaitTypeDef

```python
# DescribeScraperRequestWaitTypeDef TypedDict usage example

from types_aiobotocore_amp.type_defs import DescribeScraperRequestWaitTypeDef


def get_value() -> DescribeScraperRequestWaitTypeDef:
    return {
        "scraperId": ...,
    }


# DescribeScraperRequestWaitTypeDef definition

class DescribeScraperRequestWaitTypeDef(TypedDict):
    scraperId: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeWorkspaceRequestWaitExtraTypeDef

```python
# DescribeWorkspaceRequestWaitExtraTypeDef TypedDict usage example

from types_aiobotocore_amp.type_defs import DescribeWorkspaceRequestWaitExtraTypeDef


def get_value() -> DescribeWorkspaceRequestWaitExtraTypeDef:
    return {
        "workspaceId": ...,
    }


# DescribeWorkspaceRequestWaitExtraTypeDef definition

class DescribeWorkspaceRequestWaitExtraTypeDef(TypedDict):
    workspaceId: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeWorkspaceRequestWaitTypeDef

```python
# DescribeWorkspaceRequestWaitTypeDef TypedDict usage example

from types_aiobotocore_amp.type_defs import DescribeWorkspaceRequestWaitTypeDef


def get_value() -> DescribeWorkspaceRequestWaitTypeDef:
    return {
        "workspaceId": ...,
    }


# DescribeWorkspaceRequestWaitTypeDef definition

class DescribeWorkspaceRequestWaitTypeDef(TypedDict):
    workspaceId: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## SourceOutputTypeDef

```python
# SourceOutputTypeDef TypedDict usage example

from types_aiobotocore_amp.type_defs import SourceOutputTypeDef


def get_value() -> SourceOutputTypeDef:
    return {
        "eksConfiguration": ...,
    }


# SourceOutputTypeDef definition

class SourceOutputTypeDef(TypedDict):
    eksConfiguration: NotRequired[EksConfigurationOutputTypeDef],  # (1)
```

1. See [:material-code-braces: EksConfigurationOutputTypeDef](./type_defs.md#eksconfigurationoutputtypedef) 
## SourceTypeDef

```python
# SourceTypeDef TypedDict usage example

from types_aiobotocore_amp.type_defs import SourceTypeDef


def get_value() -> SourceTypeDef:
    return {
        "eksConfiguration": ...,
    }


# SourceTypeDef definition

class SourceTypeDef(TypedDict):
    eksConfiguration: NotRequired[EksConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: EksConfigurationTypeDef](./type_defs.md#eksconfigurationtypedef) 
## ListRuleGroupsNamespacesRequestPaginateTypeDef

```python
# ListRuleGroupsNamespacesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_amp.type_defs import ListRuleGroupsNamespacesRequestPaginateTypeDef


def get_value() -> ListRuleGroupsNamespacesRequestPaginateTypeDef:
    return {
        "workspaceId": ...,
    }


# ListRuleGroupsNamespacesRequestPaginateTypeDef definition

class ListRuleGroupsNamespacesRequestPaginateTypeDef(TypedDict):
    workspaceId: str,
    name: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListScrapersRequestPaginateTypeDef

```python
# ListScrapersRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_amp.type_defs import ListScrapersRequestPaginateTypeDef


def get_value() -> ListScrapersRequestPaginateTypeDef:
    return {
        "filters": ...,
    }


# ListScrapersRequestPaginateTypeDef definition

class ListScrapersRequestPaginateTypeDef(TypedDict):
    filters: NotRequired[Mapping[str, Sequence[str]]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListWorkspacesRequestPaginateTypeDef

```python
# ListWorkspacesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_amp.type_defs import ListWorkspacesRequestPaginateTypeDef


def get_value() -> ListWorkspacesRequestPaginateTypeDef:
    return {
        "alias": ...,
    }


# ListWorkspacesRequestPaginateTypeDef definition

class ListWorkspacesRequestPaginateTypeDef(TypedDict):
    alias: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeAlertManagerDefinitionResponseTypeDef

```python
# DescribeAlertManagerDefinitionResponseTypeDef TypedDict usage example

from types_aiobotocore_amp.type_defs import DescribeAlertManagerDefinitionResponseTypeDef


def get_value() -> DescribeAlertManagerDefinitionResponseTypeDef:
    return {
        "alertManagerDefinition": ...,
    }


# DescribeAlertManagerDefinitionResponseTypeDef definition

class DescribeAlertManagerDefinitionResponseTypeDef(TypedDict):
    alertManagerDefinition: AlertManagerDefinitionDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AlertManagerDefinitionDescriptionTypeDef](./type_defs.md#alertmanagerdefinitiondescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeLoggingConfigurationResponseTypeDef

```python
# DescribeLoggingConfigurationResponseTypeDef TypedDict usage example

from types_aiobotocore_amp.type_defs import DescribeLoggingConfigurationResponseTypeDef


def get_value() -> DescribeLoggingConfigurationResponseTypeDef:
    return {
        "loggingConfiguration": ...,
    }


# DescribeLoggingConfigurationResponseTypeDef definition

class DescribeLoggingConfigurationResponseTypeDef(TypedDict):
    loggingConfiguration: LoggingConfigurationMetadataTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LoggingConfigurationMetadataTypeDef](./type_defs.md#loggingconfigurationmetadatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeRuleGroupsNamespaceResponseTypeDef

```python
# DescribeRuleGroupsNamespaceResponseTypeDef TypedDict usage example

from types_aiobotocore_amp.type_defs import DescribeRuleGroupsNamespaceResponseTypeDef


def get_value() -> DescribeRuleGroupsNamespaceResponseTypeDef:
    return {
        "ruleGroupsNamespace": ...,
    }


# DescribeRuleGroupsNamespaceResponseTypeDef definition

class DescribeRuleGroupsNamespaceResponseTypeDef(TypedDict):
    ruleGroupsNamespace: RuleGroupsNamespaceDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RuleGroupsNamespaceDescriptionTypeDef](./type_defs.md#rulegroupsnamespacedescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListRuleGroupsNamespacesResponseTypeDef

```python
# ListRuleGroupsNamespacesResponseTypeDef TypedDict usage example

from types_aiobotocore_amp.type_defs import ListRuleGroupsNamespacesResponseTypeDef


def get_value() -> ListRuleGroupsNamespacesResponseTypeDef:
    return {
        "nextToken": ...,
    }


# ListRuleGroupsNamespacesResponseTypeDef definition

class ListRuleGroupsNamespacesResponseTypeDef(TypedDict):
    ruleGroupsNamespaces: List[RuleGroupsNamespaceSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: RuleGroupsNamespaceSummaryTypeDef](./type_defs.md#rulegroupsnamespacesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeWorkspaceResponseTypeDef

```python
# DescribeWorkspaceResponseTypeDef TypedDict usage example

from types_aiobotocore_amp.type_defs import DescribeWorkspaceResponseTypeDef


def get_value() -> DescribeWorkspaceResponseTypeDef:
    return {
        "workspace": ...,
    }


# DescribeWorkspaceResponseTypeDef definition

class DescribeWorkspaceResponseTypeDef(TypedDict):
    workspace: WorkspaceDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: WorkspaceDescriptionTypeDef](./type_defs.md#workspacedescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListWorkspacesResponseTypeDef

```python
# ListWorkspacesResponseTypeDef TypedDict usage example

from types_aiobotocore_amp.type_defs import ListWorkspacesResponseTypeDef


def get_value() -> ListWorkspacesResponseTypeDef:
    return {
        "nextToken": ...,
    }


# ListWorkspacesResponseTypeDef definition

class ListWorkspacesResponseTypeDef(TypedDict):
    workspaces: List[WorkspaceSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: WorkspaceSummaryTypeDef](./type_defs.md#workspacesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ScraperDescriptionTypeDef

```python
# ScraperDescriptionTypeDef TypedDict usage example

from types_aiobotocore_amp.type_defs import ScraperDescriptionTypeDef


def get_value() -> ScraperDescriptionTypeDef:
    return {
        "alias": ...,
    }


# ScraperDescriptionTypeDef definition

class ScraperDescriptionTypeDef(TypedDict):
    arn: str,
    createdAt: datetime,
    destination: DestinationTypeDef,  # (1)
    lastModifiedAt: datetime,
    roleArn: str,
    scrapeConfiguration: ScrapeConfigurationOutputTypeDef,  # (3)
    scraperId: str,
    source: SourceOutputTypeDef,  # (4)
    status: ScraperStatusTypeDef,  # (5)
    alias: NotRequired[str],
    roleConfiguration: NotRequired[RoleConfigurationTypeDef],  # (2)
    statusReason: NotRequired[str],
    tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-braces: DestinationTypeDef](./type_defs.md#destinationtypedef) 
2. See [:material-code-braces: RoleConfigurationTypeDef](./type_defs.md#roleconfigurationtypedef) 
3. See [:material-code-braces: ScrapeConfigurationOutputTypeDef](./type_defs.md#scrapeconfigurationoutputtypedef) 
4. See [:material-code-braces: SourceOutputTypeDef](./type_defs.md#sourceoutputtypedef) 
5. See [:material-code-braces: ScraperStatusTypeDef](./type_defs.md#scraperstatustypedef) 
## ScraperSummaryTypeDef

```python
# ScraperSummaryTypeDef TypedDict usage example

from types_aiobotocore_amp.type_defs import ScraperSummaryTypeDef


def get_value() -> ScraperSummaryTypeDef:
    return {
        "alias": ...,
    }


# ScraperSummaryTypeDef definition

class ScraperSummaryTypeDef(TypedDict):
    arn: str,
    createdAt: datetime,
    destination: DestinationTypeDef,  # (1)
    lastModifiedAt: datetime,
    roleArn: str,
    scraperId: str,
    source: SourceOutputTypeDef,  # (3)
    status: ScraperStatusTypeDef,  # (4)
    alias: NotRequired[str],
    roleConfiguration: NotRequired[RoleConfigurationTypeDef],  # (2)
    statusReason: NotRequired[str],
    tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-braces: DestinationTypeDef](./type_defs.md#destinationtypedef) 
2. See [:material-code-braces: RoleConfigurationTypeDef](./type_defs.md#roleconfigurationtypedef) 
3. See [:material-code-braces: SourceOutputTypeDef](./type_defs.md#sourceoutputtypedef) 
4. See [:material-code-braces: ScraperStatusTypeDef](./type_defs.md#scraperstatustypedef) 
## UpdateScraperRequestTypeDef

```python
# UpdateScraperRequestTypeDef TypedDict usage example

from types_aiobotocore_amp.type_defs import UpdateScraperRequestTypeDef


def get_value() -> UpdateScraperRequestTypeDef:
    return {
        "scraperId": ...,
    }


# UpdateScraperRequestTypeDef definition

class UpdateScraperRequestTypeDef(TypedDict):
    scraperId: str,
    alias: NotRequired[str],
    clientToken: NotRequired[str],
    destination: NotRequired[DestinationTypeDef],  # (1)
    roleConfiguration: NotRequired[RoleConfigurationTypeDef],  # (2)
    scrapeConfiguration: NotRequired[ScrapeConfigurationUnionTypeDef],  # (3)
```

1. See [:material-code-braces: DestinationTypeDef](./type_defs.md#destinationtypedef) 
2. See [:material-code-braces: RoleConfigurationTypeDef](./type_defs.md#roleconfigurationtypedef) 
3. See [:material-code-braces: ScrapeConfigurationTypeDef](./type_defs.md#scrapeconfigurationtypedef) [:material-code-braces: ScrapeConfigurationOutputTypeDef](./type_defs.md#scrapeconfigurationoutputtypedef) 
## DescribeScraperResponseTypeDef

```python
# DescribeScraperResponseTypeDef TypedDict usage example

from types_aiobotocore_amp.type_defs import DescribeScraperResponseTypeDef


def get_value() -> DescribeScraperResponseTypeDef:
    return {
        "scraper": ...,
    }


# DescribeScraperResponseTypeDef definition

class DescribeScraperResponseTypeDef(TypedDict):
    scraper: ScraperDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ScraperDescriptionTypeDef](./type_defs.md#scraperdescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListScrapersResponseTypeDef

```python
# ListScrapersResponseTypeDef TypedDict usage example

from types_aiobotocore_amp.type_defs import ListScrapersResponseTypeDef


def get_value() -> ListScrapersResponseTypeDef:
    return {
        "nextToken": ...,
    }


# ListScrapersResponseTypeDef definition

class ListScrapersResponseTypeDef(TypedDict):
    scrapers: List[ScraperSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ScraperSummaryTypeDef](./type_defs.md#scrapersummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateScraperRequestTypeDef

```python
# CreateScraperRequestTypeDef TypedDict usage example

from types_aiobotocore_amp.type_defs import CreateScraperRequestTypeDef


def get_value() -> CreateScraperRequestTypeDef:
    return {
        "destination": ...,
    }


# CreateScraperRequestTypeDef definition

class CreateScraperRequestTypeDef(TypedDict):
    destination: DestinationTypeDef,  # (1)
    scrapeConfiguration: ScrapeConfigurationUnionTypeDef,  # (2)
    source: SourceUnionTypeDef,  # (3)
    alias: NotRequired[str],
    clientToken: NotRequired[str],
    roleConfiguration: NotRequired[RoleConfigurationTypeDef],  # (4)
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: DestinationTypeDef](./type_defs.md#destinationtypedef) 
2. See [:material-code-braces: ScrapeConfigurationTypeDef](./type_defs.md#scrapeconfigurationtypedef) [:material-code-braces: ScrapeConfigurationOutputTypeDef](./type_defs.md#scrapeconfigurationoutputtypedef) 
3. See [:material-code-braces: SourceTypeDef](./type_defs.md#sourcetypedef) [:material-code-braces: SourceOutputTypeDef](./type_defs.md#sourceoutputtypedef) 
4. See [:material-code-braces: RoleConfigurationTypeDef](./type_defs.md#roleconfigurationtypedef) 
