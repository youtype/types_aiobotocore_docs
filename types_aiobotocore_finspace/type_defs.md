<a id="typed-dictionaries-for-aiobotocore-finspace-module"></a>

# Typed dictionaries for aiobotocore finspace module

> [Index](..) > [finspace](.) > Typed dictionaries

Auto-generated documentation for
[finspace](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace)
type annotations stubs module
[types-aiobotocore-finspace](https://pypi.org/project/types-aiobotocore-finspace/).

- [Typed dictionaries for aiobotocore finspace module](#typed-dictionaries-for-aiobotocore-finspace-module)
  - [CreateEnvironmentRequestRequestTypeDef](#createenvironmentrequestrequesttypedef)
  - [CreateEnvironmentResponseTypeDef](#createenvironmentresponsetypedef)
  - [DeleteEnvironmentRequestRequestTypeDef](#deleteenvironmentrequestrequesttypedef)
  - [EnvironmentTypeDef](#environmenttypedef)
  - [FederationParametersTypeDef](#federationparameterstypedef)
  - [GetEnvironmentRequestRequestTypeDef](#getenvironmentrequestrequesttypedef)
  - [GetEnvironmentResponseTypeDef](#getenvironmentresponsetypedef)
  - [ListEnvironmentsRequestRequestTypeDef](#listenvironmentsrequestrequesttypedef)
  - [ListEnvironmentsResponseTypeDef](#listenvironmentsresponsetypedef)
  - [ListTagsForResourceRequestRequestTypeDef](#listtagsforresourcerequestrequesttypedef)
  - [ListTagsForResourceResponseTypeDef](#listtagsforresourceresponsetypedef)
  - [ResponseMetadataTypeDef](#responsemetadatatypedef)
  - [SuperuserParametersTypeDef](#superuserparameterstypedef)
  - [TagResourceRequestRequestTypeDef](#tagresourcerequestrequesttypedef)
  - [UntagResourceRequestRequestTypeDef](#untagresourcerequestrequesttypedef)
  - [UpdateEnvironmentRequestRequestTypeDef](#updateenvironmentrequestrequesttypedef)
  - [UpdateEnvironmentResponseTypeDef](#updateenvironmentresponsetypedef)

<a id="createenvironmentrequestrequesttypedef"></a>

## CreateEnvironmentRequestRequestTypeDef

```python
from types_aiobotocore_finspace.type_defs import CreateEnvironmentRequestRequestTypeDef
```

Required fields:

- `name`: `str`

Optional fields:

- `description`: `str`
- `kmsKeyId`: `str`
- `tags`: `Mapping`\[`str`, `str`\]
- `federationMode`: [FederationModeType](./literals.md#federationmodetype)
- `federationParameters`:
  [FederationParametersTypeDef](./type_defs.md#federationparameterstypedef)
- `superuserParameters`:
  [SuperuserParametersTypeDef](./type_defs.md#superuserparameterstypedef)
- `dataBundles`: `Sequence`\[`str`\]

<a id="createenvironmentresponsetypedef"></a>

## CreateEnvironmentResponseTypeDef

```python
from types_aiobotocore_finspace.type_defs import CreateEnvironmentResponseTypeDef
```

Required fields:

- `environmentId`: `str`
- `environmentArn`: `str`
- `environmentUrl`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="deleteenvironmentrequestrequesttypedef"></a>

## DeleteEnvironmentRequestRequestTypeDef

```python
from types_aiobotocore_finspace.type_defs import DeleteEnvironmentRequestRequestTypeDef
```

Required fields:

- `environmentId`: `str`

<a id="environmenttypedef"></a>

## EnvironmentTypeDef

```python
from types_aiobotocore_finspace.type_defs import EnvironmentTypeDef
```

Optional fields:

- `name`: `str`
- `environmentId`: `str`
- `awsAccountId`: `str`
- `status`: [EnvironmentStatusType](./literals.md#environmentstatustype)
- `environmentUrl`: `str`
- `description`: `str`
- `environmentArn`: `str`
- `sageMakerStudioDomainUrl`: `str`
- `kmsKeyId`: `str`
- `dedicatedServiceAccountId`: `str`
- `federationMode`: [FederationModeType](./literals.md#federationmodetype)
- `federationParameters`:
  [FederationParametersTypeDef](./type_defs.md#federationparameterstypedef)

<a id="federationparameterstypedef"></a>

## FederationParametersTypeDef

```python
from types_aiobotocore_finspace.type_defs import FederationParametersTypeDef
```

Optional fields:

- `samlMetadataDocument`: `str`
- `samlMetadataURL`: `str`
- `applicationCallBackURL`: `str`
- `federationURN`: `str`
- `federationProviderName`: `str`
- `attributeMap`: `Mapping`\[`str`, `str`\]

<a id="getenvironmentrequestrequesttypedef"></a>

## GetEnvironmentRequestRequestTypeDef

```python
from types_aiobotocore_finspace.type_defs import GetEnvironmentRequestRequestTypeDef
```

Required fields:

- `environmentId`: `str`

<a id="getenvironmentresponsetypedef"></a>

## GetEnvironmentResponseTypeDef

```python
from types_aiobotocore_finspace.type_defs import GetEnvironmentResponseTypeDef
```

Required fields:

- `environment`: [EnvironmentTypeDef](./type_defs.md#environmenttypedef)
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="listenvironmentsrequestrequesttypedef"></a>

## ListEnvironmentsRequestRequestTypeDef

```python
from types_aiobotocore_finspace.type_defs import ListEnvironmentsRequestRequestTypeDef
```

Optional fields:

- `nextToken`: `str`
- `maxResults`: `int`

<a id="listenvironmentsresponsetypedef"></a>

## ListEnvironmentsResponseTypeDef

```python
from types_aiobotocore_finspace.type_defs import ListEnvironmentsResponseTypeDef
```

Required fields:

- `environments`:
  `List`\[[EnvironmentTypeDef](./type_defs.md#environmenttypedef)\]
- `nextToken`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="listtagsforresourcerequestrequesttypedef"></a>

## ListTagsForResourceRequestRequestTypeDef

```python
from types_aiobotocore_finspace.type_defs import ListTagsForResourceRequestRequestTypeDef
```

Required fields:

- `resourceArn`: `str`

<a id="listtagsforresourceresponsetypedef"></a>

## ListTagsForResourceResponseTypeDef

```python
from types_aiobotocore_finspace.type_defs import ListTagsForResourceResponseTypeDef
```

Required fields:

- `tags`: `Dict`\[`str`, `str`\]
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="responsemetadatatypedef"></a>

## ResponseMetadataTypeDef

```python
from types_aiobotocore_finspace.type_defs import ResponseMetadataTypeDef
```

Required fields:

- `RequestId`: `str`
- `HostId`: `str`
- `HTTPStatusCode`: `int`
- `HTTPHeaders`: `Dict`\[`str`, `str`\]
- `RetryAttempts`: `int`

<a id="superuserparameterstypedef"></a>

## SuperuserParametersTypeDef

```python
from types_aiobotocore_finspace.type_defs import SuperuserParametersTypeDef
```

Required fields:

- `emailAddress`: `str`
- `firstName`: `str`
- `lastName`: `str`

<a id="tagresourcerequestrequesttypedef"></a>

## TagResourceRequestRequestTypeDef

```python
from types_aiobotocore_finspace.type_defs import TagResourceRequestRequestTypeDef
```

Required fields:

- `resourceArn`: `str`
- `tags`: `Mapping`\[`str`, `str`\]

<a id="untagresourcerequestrequesttypedef"></a>

## UntagResourceRequestRequestTypeDef

```python
from types_aiobotocore_finspace.type_defs import UntagResourceRequestRequestTypeDef
```

Required fields:

- `resourceArn`: `str`
- `tagKeys`: `Sequence`\[`str`\]

<a id="updateenvironmentrequestrequesttypedef"></a>

## UpdateEnvironmentRequestRequestTypeDef

```python
from types_aiobotocore_finspace.type_defs import UpdateEnvironmentRequestRequestTypeDef
```

Required fields:

- `environmentId`: `str`

Optional fields:

- `name`: `str`
- `description`: `str`
- `federationMode`: [FederationModeType](./literals.md#federationmodetype)
- `federationParameters`:
  [FederationParametersTypeDef](./type_defs.md#federationparameterstypedef)

<a id="updateenvironmentresponsetypedef"></a>

## UpdateEnvironmentResponseTypeDef

```python
from types_aiobotocore_finspace.type_defs import UpdateEnvironmentResponseTypeDef
```

Required fields:

- `environment`: [EnvironmentTypeDef](./type_defs.md#environmenttypedef)
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
