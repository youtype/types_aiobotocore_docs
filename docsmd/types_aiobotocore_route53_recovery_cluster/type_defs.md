# Type definitions

> [Index](../README.md) > [Route53RecoveryCluster](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [Route53RecoveryCluster](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-cluster.html#route53recoverycluster)
    type annotations stubs module [types-aiobotocore-route53-recovery-cluster](https://pypi.org/project/types-aiobotocore-route53-recovery-cluster/).



## GetRoutingControlStateRequestRequestTypeDef

```python
# GetRoutingControlStateRequestRequestTypeDef definition

class GetRoutingControlStateRequestRequestTypeDef(TypedDict):
    RoutingControlArn: str,
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

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListRoutingControlsRequestRequestTypeDef

```python
# ListRoutingControlsRequestRequestTypeDef definition

class ListRoutingControlsRequestRequestTypeDef(TypedDict):
    ControlPanelArn: NotRequired[str],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## RoutingControlTypeDef

```python
# RoutingControlTypeDef definition

class RoutingControlTypeDef(TypedDict):
    ControlPanelArn: NotRequired[str],
    ControlPanelName: NotRequired[str],
    RoutingControlArn: NotRequired[str],
    RoutingControlName: NotRequired[str],
    RoutingControlState: NotRequired[RoutingControlStateType],  # (1)
    Owner: NotRequired[str],
```

1. See [:material-code-brackets: RoutingControlStateType](./literals.md#routingcontrolstatetype) 
## UpdateRoutingControlStateEntryTypeDef

```python
# UpdateRoutingControlStateEntryTypeDef definition

class UpdateRoutingControlStateEntryTypeDef(TypedDict):
    RoutingControlArn: str,
    RoutingControlState: RoutingControlStateType,  # (1)
```

1. See [:material-code-brackets: RoutingControlStateType](./literals.md#routingcontrolstatetype) 
## UpdateRoutingControlStateRequestRequestTypeDef

```python
# UpdateRoutingControlStateRequestRequestTypeDef definition

class UpdateRoutingControlStateRequestRequestTypeDef(TypedDict):
    RoutingControlArn: str,
    RoutingControlState: RoutingControlStateType,  # (1)
    SafetyRulesToOverride: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: RoutingControlStateType](./literals.md#routingcontrolstatetype) 
## GetRoutingControlStateResponseTypeDef

```python
# GetRoutingControlStateResponseTypeDef definition

class GetRoutingControlStateResponseTypeDef(TypedDict):
    RoutingControlArn: str,
    RoutingControlState: RoutingControlStateType,  # (1)
    RoutingControlName: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: RoutingControlStateType](./literals.md#routingcontrolstatetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListRoutingControlsRequestPaginateTypeDef

```python
# ListRoutingControlsRequestPaginateTypeDef definition

class ListRoutingControlsRequestPaginateTypeDef(TypedDict):
    ControlPanelArn: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListRoutingControlsResponseTypeDef

```python
# ListRoutingControlsResponseTypeDef definition

class ListRoutingControlsResponseTypeDef(TypedDict):
    RoutingControls: List[RoutingControlTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: RoutingControlTypeDef](./type_defs.md#routingcontroltypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateRoutingControlStatesRequestRequestTypeDef

```python
# UpdateRoutingControlStatesRequestRequestTypeDef definition

class UpdateRoutingControlStatesRequestRequestTypeDef(TypedDict):
    UpdateRoutingControlStateEntries: Sequence[UpdateRoutingControlStateEntryTypeDef],  # (1)
    SafetyRulesToOverride: NotRequired[Sequence[str]],
```

1. See [:material-code-braces: UpdateRoutingControlStateEntryTypeDef](./type_defs.md#updateroutingcontrolstateentrytypedef) 
