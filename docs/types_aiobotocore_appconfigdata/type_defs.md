<a id="typed-dictionaries-for-aiobotocore-appconfigdata-module"></a>

# Typed dictionaries for aiobotocore AppConfigData module

> [Index](../README.md) > [AppConfigData](./README.md) > Typed dictionaries

Auto-generated documentation for
[AppConfigData](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfigdata.html#AppConfigData)
type annotations stubs module
[types-aiobotocore-appconfigdata](https://pypi.org/project/types-aiobotocore-appconfigdata/).

- [Typed dictionaries for aiobotocore AppConfigData module](#typed-dictionaries-for-aiobotocore-appconfigdata-module)
  - [GetLatestConfigurationRequestRequestTypeDef](#getlatestconfigurationrequestrequesttypedef)
  - [GetLatestConfigurationResponseTypeDef](#getlatestconfigurationresponsetypedef)
  - [ResponseMetadataTypeDef](#responsemetadatatypedef)
  - [StartConfigurationSessionRequestRequestTypeDef](#startconfigurationsessionrequestrequesttypedef)
  - [StartConfigurationSessionResponseTypeDef](#startconfigurationsessionresponsetypedef)

<a id="getlatestconfigurationrequestrequesttypedef"></a>

## GetLatestConfigurationRequestRequestTypeDef

```python
from types_aiobotocore_appconfigdata.type_defs import GetLatestConfigurationRequestRequestTypeDef
```

Required fields:

- `ConfigurationToken`: `str`

<a id="getlatestconfigurationresponsetypedef"></a>

## GetLatestConfigurationResponseTypeDef

```python
from types_aiobotocore_appconfigdata.type_defs import GetLatestConfigurationResponseTypeDef
```

Required fields:

- `NextPollConfigurationToken`: `str`
- `NextPollIntervalInSeconds`: `int`
- `ContentType`: `str`
- `Configuration`: `StreamingBody`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="responsemetadatatypedef"></a>

## ResponseMetadataTypeDef

```python
from types_aiobotocore_appconfigdata.type_defs import ResponseMetadataTypeDef
```

Required fields:

- `RequestId`: `str`
- `HostId`: `str`
- `HTTPStatusCode`: `int`
- `HTTPHeaders`: `Dict`\[`str`, `str`\]
- `RetryAttempts`: `int`

<a id="startconfigurationsessionrequestrequesttypedef"></a>

## StartConfigurationSessionRequestRequestTypeDef

```python
from types_aiobotocore_appconfigdata.type_defs import StartConfigurationSessionRequestRequestTypeDef
```

Required fields:

- `ApplicationIdentifier`: `str`
- `EnvironmentIdentifier`: `str`
- `ConfigurationProfileIdentifier`: `str`

Optional fields:

- `RequiredMinimumPollIntervalInSeconds`: `int`

<a id="startconfigurationsessionresponsetypedef"></a>

## StartConfigurationSessionResponseTypeDef

```python
from types_aiobotocore_appconfigdata.type_defs import StartConfigurationSessionResponseTypeDef
```

Required fields:

- `InitialConfigurationToken`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
