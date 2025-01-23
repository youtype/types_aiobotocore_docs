# Type definitions

> [Index](../README.md) > [CloudWatchNetworkMonitor](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [CloudWatchNetworkMonitor](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmonitor.html#cloudwatchnetworkmonitor)
    type annotations stubs module [types-aiobotocore-networkmonitor](https://pypi.org/project/types-aiobotocore-networkmonitor/).



## CreateMonitorProbeInputTypeDef

```python
# CreateMonitorProbeInputTypeDef definition

class CreateMonitorProbeInputTypeDef(TypedDict):
    sourceArn: str,
    destination: str,
    protocol: ProtocolType,  # (1)
    destinationPort: NotRequired[int],
    packetSize: NotRequired[int],
    probeTags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: ProtocolType](./literals.md#protocoltype) 
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

## ProbeInputTypeDef

```python
# ProbeInputTypeDef definition

class ProbeInputTypeDef(TypedDict):
    sourceArn: str,
    destination: str,
    protocol: ProtocolType,  # (1)
    destinationPort: NotRequired[int],
    packetSize: NotRequired[int],
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: ProtocolType](./literals.md#protocoltype) 
## DeleteMonitorInputRequestTypeDef

```python
# DeleteMonitorInputRequestTypeDef definition

class DeleteMonitorInputRequestTypeDef(TypedDict):
    monitorName: str,
```

## DeleteProbeInputRequestTypeDef

```python
# DeleteProbeInputRequestTypeDef definition

class DeleteProbeInputRequestTypeDef(TypedDict):
    monitorName: str,
    probeId: str,
```

## GetMonitorInputRequestTypeDef

```python
# GetMonitorInputRequestTypeDef definition

class GetMonitorInputRequestTypeDef(TypedDict):
    monitorName: str,
```

## ProbeTypeDef

```python
# ProbeTypeDef definition

class ProbeTypeDef(TypedDict):
    sourceArn: str,
    destination: str,
    protocol: ProtocolType,  # (1)
    probeId: NotRequired[str],
    probeArn: NotRequired[str],
    destinationPort: NotRequired[int],
    packetSize: NotRequired[int],
    addressFamily: NotRequired[AddressFamilyType],  # (2)
    vpcId: NotRequired[str],
    state: NotRequired[ProbeStateType],  # (3)
    createdAt: NotRequired[datetime],
    modifiedAt: NotRequired[datetime],
    tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-brackets: ProtocolType](./literals.md#protocoltype) 
2. See [:material-code-brackets: AddressFamilyType](./literals.md#addressfamilytype) 
3. See [:material-code-brackets: ProbeStateType](./literals.md#probestatetype) 
## GetProbeInputRequestTypeDef

```python
# GetProbeInputRequestTypeDef definition

class GetProbeInputRequestTypeDef(TypedDict):
    monitorName: str,
    probeId: str,
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListMonitorsInputRequestTypeDef

```python
# ListMonitorsInputRequestTypeDef definition

class ListMonitorsInputRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
    state: NotRequired[str],
```

## MonitorSummaryTypeDef

```python
# MonitorSummaryTypeDef definition

class MonitorSummaryTypeDef(TypedDict):
    monitorArn: str,
    monitorName: str,
    state: MonitorStateType,  # (1)
    aggregationPeriod: NotRequired[int],
    tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-brackets: MonitorStateType](./literals.md#monitorstatetype) 
## ListTagsForResourceInputRequestTypeDef

```python
# ListTagsForResourceInputRequestTypeDef definition

class ListTagsForResourceInputRequestTypeDef(TypedDict):
    resourceArn: str,
```

## TagResourceInputRequestTypeDef

```python
# TagResourceInputRequestTypeDef definition

class TagResourceInputRequestTypeDef(TypedDict):
    resourceArn: str,
    tags: Mapping[str, str],
```

## UntagResourceInputRequestTypeDef

```python
# UntagResourceInputRequestTypeDef definition

class UntagResourceInputRequestTypeDef(TypedDict):
    resourceArn: str,
    tagKeys: Sequence[str],
```

## UpdateMonitorInputRequestTypeDef

```python
# UpdateMonitorInputRequestTypeDef definition

class UpdateMonitorInputRequestTypeDef(TypedDict):
    monitorName: str,
    aggregationPeriod: int,
```

## UpdateProbeInputRequestTypeDef

```python
# UpdateProbeInputRequestTypeDef definition

class UpdateProbeInputRequestTypeDef(TypedDict):
    monitorName: str,
    probeId: str,
    state: NotRequired[ProbeStateType],  # (1)
    destination: NotRequired[str],
    destinationPort: NotRequired[int],
    protocol: NotRequired[ProtocolType],  # (2)
    packetSize: NotRequired[int],
```

1. See [:material-code-brackets: ProbeStateType](./literals.md#probestatetype) 
2. See [:material-code-brackets: ProtocolType](./literals.md#protocoltype) 
## CreateMonitorInputRequestTypeDef

```python
# CreateMonitorInputRequestTypeDef definition

class CreateMonitorInputRequestTypeDef(TypedDict):
    monitorName: str,
    probes: NotRequired[Sequence[CreateMonitorProbeInputTypeDef]],  # (1)
    aggregationPeriod: NotRequired[int],
    clientToken: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: CreateMonitorProbeInputTypeDef](./type_defs.md#createmonitorprobeinputtypedef) 
## CreateMonitorOutputTypeDef

```python
# CreateMonitorOutputTypeDef definition

class CreateMonitorOutputTypeDef(TypedDict):
    monitorArn: str,
    monitorName: str,
    state: MonitorStateType,  # (1)
    aggregationPeriod: int,
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: MonitorStateType](./literals.md#monitorstatetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateProbeOutputTypeDef

```python
# CreateProbeOutputTypeDef definition

class CreateProbeOutputTypeDef(TypedDict):
    probeId: str,
    probeArn: str,
    sourceArn: str,
    destination: str,
    destinationPort: int,
    protocol: ProtocolType,  # (1)
    packetSize: int,
    addressFamily: AddressFamilyType,  # (2)
    vpcId: str,
    state: ProbeStateType,  # (3)
    createdAt: datetime,
    modifiedAt: datetime,
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: ProtocolType](./literals.md#protocoltype) 
2. See [:material-code-brackets: AddressFamilyType](./literals.md#addressfamilytype) 
3. See [:material-code-brackets: ProbeStateType](./literals.md#probestatetype) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetProbeOutputTypeDef

```python
# GetProbeOutputTypeDef definition

class GetProbeOutputTypeDef(TypedDict):
    probeId: str,
    probeArn: str,
    sourceArn: str,
    destination: str,
    destinationPort: int,
    protocol: ProtocolType,  # (1)
    packetSize: int,
    addressFamily: AddressFamilyType,  # (2)
    vpcId: str,
    state: ProbeStateType,  # (3)
    createdAt: datetime,
    modifiedAt: datetime,
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: ProtocolType](./literals.md#protocoltype) 
2. See [:material-code-brackets: AddressFamilyType](./literals.md#addressfamilytype) 
3. See [:material-code-brackets: ProbeStateType](./literals.md#probestatetype) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceOutputTypeDef

```python
# ListTagsForResourceOutputTypeDef definition

class ListTagsForResourceOutputTypeDef(TypedDict):
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateMonitorOutputTypeDef

```python
# UpdateMonitorOutputTypeDef definition

class UpdateMonitorOutputTypeDef(TypedDict):
    monitorArn: str,
    monitorName: str,
    state: MonitorStateType,  # (1)
    aggregationPeriod: int,
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: MonitorStateType](./literals.md#monitorstatetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateProbeOutputTypeDef

```python
# UpdateProbeOutputTypeDef definition

class UpdateProbeOutputTypeDef(TypedDict):
    probeId: str,
    probeArn: str,
    sourceArn: str,
    destination: str,
    destinationPort: int,
    protocol: ProtocolType,  # (1)
    packetSize: int,
    addressFamily: AddressFamilyType,  # (2)
    vpcId: str,
    state: ProbeStateType,  # (3)
    createdAt: datetime,
    modifiedAt: datetime,
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: ProtocolType](./literals.md#protocoltype) 
2. See [:material-code-brackets: AddressFamilyType](./literals.md#addressfamilytype) 
3. See [:material-code-brackets: ProbeStateType](./literals.md#probestatetype) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateProbeInputRequestTypeDef

```python
# CreateProbeInputRequestTypeDef definition

class CreateProbeInputRequestTypeDef(TypedDict):
    monitorName: str,
    probe: ProbeInputTypeDef,  # (1)
    clientToken: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: ProbeInputTypeDef](./type_defs.md#probeinputtypedef) 
## GetMonitorOutputTypeDef

```python
# GetMonitorOutputTypeDef definition

class GetMonitorOutputTypeDef(TypedDict):
    monitorArn: str,
    monitorName: str,
    state: MonitorStateType,  # (1)
    aggregationPeriod: int,
    tags: Dict[str, str],
    probes: List[ProbeTypeDef],  # (2)
    createdAt: datetime,
    modifiedAt: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: MonitorStateType](./literals.md#monitorstatetype) 
2. See [:material-code-braces: ProbeTypeDef](./type_defs.md#probetypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListMonitorsInputPaginateTypeDef

```python
# ListMonitorsInputPaginateTypeDef definition

class ListMonitorsInputPaginateTypeDef(TypedDict):
    state: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListMonitorsOutputTypeDef

```python
# ListMonitorsOutputTypeDef definition

class ListMonitorsOutputTypeDef(TypedDict):
    monitors: List[MonitorSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: MonitorSummaryTypeDef](./type_defs.md#monitorsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
