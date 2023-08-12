# Type definitions

> [Index](../README.md) > [IoTSecureTunneling](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [IoTSecureTunneling](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsecuretunneling.html#IoTSecureTunneling)
    type annotations stubs module [types-aiobotocore-iotsecuretunneling](https://pypi.org/project/types-aiobotocore-iotsecuretunneling/).



## CloseTunnelRequestRequestTypeDef

```python
# CloseTunnelRequestRequestTypeDef definition

class CloseTunnelRequestRequestTypeDef(TypedDict):
    tunnelId: str,
    delete: NotRequired[bool],
```

## ConnectionStateTypeDef

```python
# ConnectionStateTypeDef definition

class ConnectionStateTypeDef(TypedDict):
    status: NotRequired[ConnectionStatusType],  # (1)
    lastUpdatedAt: NotRequired[datetime],
```

1. See [:material-code-brackets: ConnectionStatusType](./literals.md#connectionstatustype) 
## DescribeTunnelRequestRequestTypeDef

```python
# DescribeTunnelRequestRequestTypeDef definition

class DescribeTunnelRequestRequestTypeDef(TypedDict):
    tunnelId: str,
```

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

## DestinationConfigTypeDef

```python
# DestinationConfigTypeDef definition

class DestinationConfigTypeDef(TypedDict):
    services: List[str],
    thingName: NotRequired[str],
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
```

## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    key: str,
    value: str,
```

## ListTunnelsRequestRequestTypeDef

```python
# ListTunnelsRequestRequestTypeDef definition

class ListTunnelsRequestRequestTypeDef(TypedDict):
    thingName: NotRequired[str],
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## TunnelSummaryTypeDef

```python
# TunnelSummaryTypeDef definition

class TunnelSummaryTypeDef(TypedDict):
    tunnelId: NotRequired[str],
    tunnelArn: NotRequired[str],
    status: NotRequired[TunnelStatusType],  # (1)
    description: NotRequired[str],
    createdAt: NotRequired[datetime],
    lastUpdatedAt: NotRequired[datetime],
```

1. See [:material-code-brackets: TunnelStatusType](./literals.md#tunnelstatustype) 
## TimeoutConfigTypeDef

```python
# TimeoutConfigTypeDef definition

class TimeoutConfigTypeDef(TypedDict):
    maxLifetimeTimeoutMinutes: NotRequired[int],
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    tagKeys: Sequence[str],
```

## OpenTunnelResponseTypeDef

```python
# OpenTunnelResponseTypeDef definition

class OpenTunnelResponseTypeDef(TypedDict):
    tunnelId: str,
    tunnelArn: str,
    sourceAccessToken: str,
    destinationAccessToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RotateTunnelAccessTokenResponseTypeDef

```python
# RotateTunnelAccessTokenResponseTypeDef definition

class RotateTunnelAccessTokenResponseTypeDef(TypedDict):
    tunnelArn: str,
    sourceAccessToken: str,
    destinationAccessToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RotateTunnelAccessTokenRequestRequestTypeDef

```python
# RotateTunnelAccessTokenRequestRequestTypeDef definition

class RotateTunnelAccessTokenRequestRequestTypeDef(TypedDict):
    tunnelId: str,
    clientMode: ClientModeType,  # (1)
    destinationConfig: NotRequired[DestinationConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: ClientModeType](./literals.md#clientmodetype) 
2. See [:material-code-braces: DestinationConfigTypeDef](./type_defs.md#destinationconfigtypedef) 
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
## ListTunnelsResponseTypeDef

```python
# ListTunnelsResponseTypeDef definition

class ListTunnelsResponseTypeDef(TypedDict):
    tunnelSummaries: List[TunnelSummaryTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TunnelSummaryTypeDef](./type_defs.md#tunnelsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## OpenTunnelRequestRequestTypeDef

```python
# OpenTunnelRequestRequestTypeDef definition

class OpenTunnelRequestRequestTypeDef(TypedDict):
    description: NotRequired[str],
    tags: NotRequired[Sequence[TagTypeDef]],  # (1)
    destinationConfig: NotRequired[DestinationConfigTypeDef],  # (2)
    timeoutConfig: NotRequired[TimeoutConfigTypeDef],  # (3)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: DestinationConfigTypeDef](./type_defs.md#destinationconfigtypedef) 
3. See [:material-code-braces: TimeoutConfigTypeDef](./type_defs.md#timeoutconfigtypedef) 
## TunnelTypeDef

```python
# TunnelTypeDef definition

class TunnelTypeDef(TypedDict):
    tunnelId: NotRequired[str],
    tunnelArn: NotRequired[str],
    status: NotRequired[TunnelStatusType],  # (1)
    sourceConnectionState: NotRequired[ConnectionStateTypeDef],  # (2)
    destinationConnectionState: NotRequired[ConnectionStateTypeDef],  # (2)
    description: NotRequired[str],
    destinationConfig: NotRequired[DestinationConfigTypeDef],  # (4)
    timeoutConfig: NotRequired[TimeoutConfigTypeDef],  # (5)
    tags: NotRequired[List[TagTypeDef]],  # (6)
    createdAt: NotRequired[datetime],
    lastUpdatedAt: NotRequired[datetime],
```

1. See [:material-code-brackets: TunnelStatusType](./literals.md#tunnelstatustype) 
2. See [:material-code-braces: ConnectionStateTypeDef](./type_defs.md#connectionstatetypedef) 
3. See [:material-code-braces: ConnectionStateTypeDef](./type_defs.md#connectionstatetypedef) 
4. See [:material-code-braces: DestinationConfigTypeDef](./type_defs.md#destinationconfigtypedef) 
5. See [:material-code-braces: TimeoutConfigTypeDef](./type_defs.md#timeoutconfigtypedef) 
6. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## DescribeTunnelResponseTypeDef

```python
# DescribeTunnelResponseTypeDef definition

class DescribeTunnelResponseTypeDef(TypedDict):
    tunnel: TunnelTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TunnelTypeDef](./type_defs.md#tunneltypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
