# Type definitions

> [Index](../README.md) > [CodeStarconnections](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [CodeStarconnections](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-connections.html#CodeStarconnections)
    type annotations stubs module [types-aiobotocore-codestar-connections](https://pypi.org/project/types-aiobotocore-codestar-connections/).



## ConnectionTypeDef

```python
# ConnectionTypeDef definition

class ConnectionTypeDef(TypedDict):
    ConnectionName: NotRequired[str],
    ConnectionArn: NotRequired[str],
    ProviderType: NotRequired[ProviderTypeType],  # (1)
    OwnerAccountId: NotRequired[str],
    ConnectionStatus: NotRequired[ConnectionStatusType],  # (2)
    HostArn: NotRequired[str],
```

1. See [:material-code-brackets: ProviderTypeType](./literals.md#providertypetype) 
2. See [:material-code-brackets: ConnectionStatusType](./literals.md#connectionstatustype) 
## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    Key: str,
    Value: str,
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

## VpcConfigurationTypeDef

```python
# VpcConfigurationTypeDef definition

class VpcConfigurationTypeDef(TypedDict):
    VpcId: str,
    SubnetIds: Sequence[str],
    SecurityGroupIds: Sequence[str],
    TlsCertificate: NotRequired[str],
```

## DeleteConnectionInputRequestTypeDef

```python
# DeleteConnectionInputRequestTypeDef definition

class DeleteConnectionInputRequestTypeDef(TypedDict):
    ConnectionArn: str,
```

## DeleteHostInputRequestTypeDef

```python
# DeleteHostInputRequestTypeDef definition

class DeleteHostInputRequestTypeDef(TypedDict):
    HostArn: str,
```

## GetConnectionInputRequestTypeDef

```python
# GetConnectionInputRequestTypeDef definition

class GetConnectionInputRequestTypeDef(TypedDict):
    ConnectionArn: str,
```

## GetHostInputRequestTypeDef

```python
# GetHostInputRequestTypeDef definition

class GetHostInputRequestTypeDef(TypedDict):
    HostArn: str,
```

## ListConnectionsInputRequestTypeDef

```python
# ListConnectionsInputRequestTypeDef definition

class ListConnectionsInputRequestTypeDef(TypedDict):
    ProviderTypeFilter: NotRequired[ProviderTypeType],  # (1)
    HostArnFilter: NotRequired[str],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-brackets: ProviderTypeType](./literals.md#providertypetype) 
## ListHostsInputRequestTypeDef

```python
# ListHostsInputRequestTypeDef definition

class ListHostsInputRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListTagsForResourceInputRequestTypeDef

```python
# ListTagsForResourceInputRequestTypeDef definition

class ListTagsForResourceInputRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## UntagResourceInputRequestTypeDef

```python
# UntagResourceInputRequestTypeDef definition

class UntagResourceInputRequestTypeDef(TypedDict):
    ResourceArn: str,
    TagKeys: Sequence[str],
```

## CreateConnectionInputRequestTypeDef

```python
# CreateConnectionInputRequestTypeDef definition

class CreateConnectionInputRequestTypeDef(TypedDict):
    ConnectionName: str,
    ProviderType: NotRequired[ProviderTypeType],  # (1)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (2)
    HostArn: NotRequired[str],
```

1. See [:material-code-brackets: ProviderTypeType](./literals.md#providertypetype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## TagResourceInputRequestTypeDef

```python
# TagResourceInputRequestTypeDef definition

class TagResourceInputRequestTypeDef(TypedDict):
    ResourceArn: str,
    Tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateConnectionOutputTypeDef

```python
# CreateConnectionOutputTypeDef definition

class CreateConnectionOutputTypeDef(TypedDict):
    ConnectionArn: str,
    Tags: List[TagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateHostOutputTypeDef

```python
# CreateHostOutputTypeDef definition

class CreateHostOutputTypeDef(TypedDict):
    HostArn: str,
    Tags: List[TagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetConnectionOutputTypeDef

```python
# GetConnectionOutputTypeDef definition

class GetConnectionOutputTypeDef(TypedDict):
    Connection: ConnectionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ConnectionTypeDef](./type_defs.md#connectiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListConnectionsOutputTypeDef

```python
# ListConnectionsOutputTypeDef definition

class ListConnectionsOutputTypeDef(TypedDict):
    Connections: List[ConnectionTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ConnectionTypeDef](./type_defs.md#connectiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceOutputTypeDef

```python
# ListTagsForResourceOutputTypeDef definition

class ListTagsForResourceOutputTypeDef(TypedDict):
    Tags: List[TagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateHostInputRequestTypeDef

```python
# CreateHostInputRequestTypeDef definition

class CreateHostInputRequestTypeDef(TypedDict):
    Name: str,
    ProviderType: ProviderTypeType,  # (1)
    ProviderEndpoint: str,
    VpcConfiguration: NotRequired[VpcConfigurationTypeDef],  # (2)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (3)
```

1. See [:material-code-brackets: ProviderTypeType](./literals.md#providertypetype) 
2. See [:material-code-braces: VpcConfigurationTypeDef](./type_defs.md#vpcconfigurationtypedef) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## GetHostOutputTypeDef

```python
# GetHostOutputTypeDef definition

class GetHostOutputTypeDef(TypedDict):
    Name: str,
    Status: str,
    ProviderType: ProviderTypeType,  # (1)
    ProviderEndpoint: str,
    VpcConfiguration: VpcConfigurationTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: ProviderTypeType](./literals.md#providertypetype) 
2. See [:material-code-braces: VpcConfigurationTypeDef](./type_defs.md#vpcconfigurationtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## HostTypeDef

```python
# HostTypeDef definition

class HostTypeDef(TypedDict):
    Name: NotRequired[str],
    HostArn: NotRequired[str],
    ProviderType: NotRequired[ProviderTypeType],  # (1)
    ProviderEndpoint: NotRequired[str],
    VpcConfiguration: NotRequired[VpcConfigurationTypeDef],  # (2)
    Status: NotRequired[str],
    StatusMessage: NotRequired[str],
```

1. See [:material-code-brackets: ProviderTypeType](./literals.md#providertypetype) 
2. See [:material-code-braces: VpcConfigurationTypeDef](./type_defs.md#vpcconfigurationtypedef) 
## UpdateHostInputRequestTypeDef

```python
# UpdateHostInputRequestTypeDef definition

class UpdateHostInputRequestTypeDef(TypedDict):
    HostArn: str,
    ProviderEndpoint: NotRequired[str],
    VpcConfiguration: NotRequired[VpcConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: VpcConfigurationTypeDef](./type_defs.md#vpcconfigurationtypedef) 
## ListHostsOutputTypeDef

```python
# ListHostsOutputTypeDef definition

class ListHostsOutputTypeDef(TypedDict):
    Hosts: List[HostTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: HostTypeDef](./type_defs.md#hosttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
