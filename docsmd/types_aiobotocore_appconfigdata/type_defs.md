# Type definitions

> [Index](../README.md) > [AppConfigData](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [AppConfigData](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfigdata.html#AppConfigData)
    type annotations stubs module [types-aiobotocore-appconfigdata](https://pypi.org/project/types-aiobotocore-appconfigdata/).



## GetLatestConfigurationRequestRequestTypeDef

```python
# GetLatestConfigurationRequestRequestTypeDef definition

class GetLatestConfigurationRequestRequestTypeDef(TypedDict):
    ConfigurationToken: str,
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

## StartConfigurationSessionRequestRequestTypeDef

```python
# StartConfigurationSessionRequestRequestTypeDef definition

class StartConfigurationSessionRequestRequestTypeDef(TypedDict):
    ApplicationIdentifier: str,
    EnvironmentIdentifier: str,
    ConfigurationProfileIdentifier: str,
    RequiredMinimumPollIntervalInSeconds: NotRequired[int],
```

## GetLatestConfigurationResponseTypeDef

```python
# GetLatestConfigurationResponseTypeDef definition

class GetLatestConfigurationResponseTypeDef(TypedDict):
    NextPollConfigurationToken: str,
    NextPollIntervalInSeconds: int,
    ContentType: str,
    Configuration: StreamingBody,
    VersionLabel: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartConfigurationSessionResponseTypeDef

```python
# StartConfigurationSessionResponseTypeDef definition

class StartConfigurationSessionResponseTypeDef(TypedDict):
    InitialConfigurationToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
