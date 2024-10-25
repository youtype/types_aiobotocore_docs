# Type definitions

> [Index](../README.md) > [KinesisVideoSignalingChannels](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [KinesisVideoSignalingChannels](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-signaling.html#KinesisVideoSignalingChannels)
    type annotations stubs module [types-aiobotocore-kinesis-video-signaling](https://pypi.org/project/types-aiobotocore-kinesis-video-signaling/).



## GetIceServerConfigRequestRequestTypeDef

```python
# GetIceServerConfigRequestRequestTypeDef definition

class GetIceServerConfigRequestRequestTypeDef(TypedDict):
    ChannelARN: str,
    ClientId: NotRequired[str],
    Service: NotRequired[ServiceType],  # (1)
    Username: NotRequired[str],
```

1. See [:material-code-brackets: ServiceType](./literals.md#servicetype) 
## IceServerTypeDef

```python
# IceServerTypeDef definition

class IceServerTypeDef(TypedDict):
    Uris: NotRequired[List[str]],
    Username: NotRequired[str],
    Password: NotRequired[str],
    Ttl: NotRequired[int],
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

## SendAlexaOfferToMasterRequestRequestTypeDef

```python
# SendAlexaOfferToMasterRequestRequestTypeDef definition

class SendAlexaOfferToMasterRequestRequestTypeDef(TypedDict):
    ChannelARN: str,
    SenderClientId: str,
    MessagePayload: str,
```

## GetIceServerConfigResponseTypeDef

```python
# GetIceServerConfigResponseTypeDef definition

class GetIceServerConfigResponseTypeDef(TypedDict):
    IceServerList: List[IceServerTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: IceServerTypeDef](./type_defs.md#iceservertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SendAlexaOfferToMasterResponseTypeDef

```python
# SendAlexaOfferToMasterResponseTypeDef definition

class SendAlexaOfferToMasterResponseTypeDef(TypedDict):
    Answer: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
