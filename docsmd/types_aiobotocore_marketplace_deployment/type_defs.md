# Type definitions

> [Index](../README.md) > [MarketplaceDeploymentService](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [MarketplaceDeploymentService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-deployment.html#MarketplaceDeploymentService)
    type annotations stubs module [types-aiobotocore-marketplace-deployment](https://pypi.org/project/types-aiobotocore-marketplace-deployment/).

## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```




## DeploymentParameterInputTypeDef

```python
# DeploymentParameterInputTypeDef definition

class DeploymentParameterInputTypeDef(TypedDict):
    name: str,
    secretString: str,
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
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

## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    tags: NotRequired[Mapping[str, str]],
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    tagKeys: Sequence[str],
```

## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutDeploymentParameterResponseTypeDef

```python
# PutDeploymentParameterResponseTypeDef definition

class PutDeploymentParameterResponseTypeDef(TypedDict):
    agreementId: str,
    deploymentParameterId: str,
    resourceArn: str,
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutDeploymentParameterRequestRequestTypeDef

```python
# PutDeploymentParameterRequestRequestTypeDef definition

class PutDeploymentParameterRequestRequestTypeDef(TypedDict):
    agreementId: str,
    catalog: str,
    deploymentParameter: DeploymentParameterInputTypeDef,  # (1)
    productId: str,
    clientToken: NotRequired[str],
    expirationDate: NotRequired[TimestampTypeDef],
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: DeploymentParameterInputTypeDef](./type_defs.md#deploymentparameterinputtypedef) 
