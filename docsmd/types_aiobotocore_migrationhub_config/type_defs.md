# Type definitions

> [Index](../README.md) > [MigrationHubConfig](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [MigrationHubConfig](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhub-config.html#migrationhubconfig)
    type annotations stubs module [types-aiobotocore-migrationhub-config](https://pypi.org/project/types-aiobotocore-migrationhub-config/).



## TargetTypeDef

```python
# TargetTypeDef definition

class TargetTypeDef(TypedDict):
    Type: TargetTypeType,  # (1)
    Id: NotRequired[str],
```

1. See [:material-code-brackets: TargetTypeType](./literals.md#targettypetype) 
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

## DeleteHomeRegionControlRequestRequestTypeDef

```python
# DeleteHomeRegionControlRequestRequestTypeDef definition

class DeleteHomeRegionControlRequestRequestTypeDef(TypedDict):
    ControlId: str,
```

## CreateHomeRegionControlRequestRequestTypeDef

```python
# CreateHomeRegionControlRequestRequestTypeDef definition

class CreateHomeRegionControlRequestRequestTypeDef(TypedDict):
    HomeRegion: str,
    Target: TargetTypeDef,  # (1)
    DryRun: NotRequired[bool],
```

1. See [:material-code-braces: TargetTypeDef](./type_defs.md#targettypedef) 
## DescribeHomeRegionControlsRequestRequestTypeDef

```python
# DescribeHomeRegionControlsRequestRequestTypeDef definition

class DescribeHomeRegionControlsRequestRequestTypeDef(TypedDict):
    ControlId: NotRequired[str],
    HomeRegion: NotRequired[str],
    Target: NotRequired[TargetTypeDef],  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: TargetTypeDef](./type_defs.md#targettypedef) 
## HomeRegionControlTypeDef

```python
# HomeRegionControlTypeDef definition

class HomeRegionControlTypeDef(TypedDict):
    ControlId: NotRequired[str],
    HomeRegion: NotRequired[str],
    Target: NotRequired[TargetTypeDef],  # (1)
    RequestedTime: NotRequired[datetime],
```

1. See [:material-code-braces: TargetTypeDef](./type_defs.md#targettypedef) 
## GetHomeRegionResultTypeDef

```python
# GetHomeRegionResultTypeDef definition

class GetHomeRegionResultTypeDef(TypedDict):
    HomeRegion: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateHomeRegionControlResultTypeDef

```python
# CreateHomeRegionControlResultTypeDef definition

class CreateHomeRegionControlResultTypeDef(TypedDict):
    HomeRegionControl: HomeRegionControlTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: HomeRegionControlTypeDef](./type_defs.md#homeregioncontroltypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeHomeRegionControlsResultTypeDef

```python
# DescribeHomeRegionControlsResultTypeDef definition

class DescribeHomeRegionControlsResultTypeDef(TypedDict):
    HomeRegionControls: List[HomeRegionControlTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: HomeRegionControlTypeDef](./type_defs.md#homeregioncontroltypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
