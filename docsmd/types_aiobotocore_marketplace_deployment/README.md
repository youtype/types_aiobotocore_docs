# MarketplaceDeploymentService module

> [Index](../README.md) > MarketplaceDeploymentService


!!! note ""

    Auto-generated documentation for [MarketplaceDeploymentService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-deployment.html#marketplacedeploymentservice)
    type annotations stubs module [types-aiobotocore-marketplace-deployment](https://pypi.org/project/types-aiobotocore-marketplace-deployment/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy-boto3-builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==3.1.1' mypy-boto3-builder`
1. Select `aiobotocore` AWS SDK.
1. Add `MarketplaceDeploymentService` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `MarketplaceDeploymentService` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[marketplace-deployment]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[marketplace-deployment]'

# standalone installation
python -m pip install types-aiobotocore-marketplace-deployment
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-marketplace-deployment
```

## Usage

Code samples can be found in [Examples](./usage.md).

## MarketplaceDeploymentServiceClient

Type annotations and code completion for  `#!python session.create_client("marketplace-deployment")` as [MarketplaceDeploymentServiceClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-deployment.html#MarketplaceDeploymentService.Client)

```python
# MarketplaceDeploymentServiceClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_marketplace_deployment.client import MarketplaceDeploymentServiceClient


session = get_session()
async with session.create_client("marketplace-deployment") as client:
    client: MarketplaceDeploymentServiceClient
```








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# MarketplaceDeploymentServiceServiceName usage example

from types_aiobotocore_marketplace_deployment.literals import MarketplaceDeploymentServiceServiceName

def get_value() -> MarketplaceDeploymentServiceServiceName:
    return "marketplace-deployment"
```

- [MarketplaceDeploymentServiceServiceName](./literals.md#marketplacedeploymentserviceservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [DeploymentParameterInputTypeDef](./type_defs.md#deploymentparameterinputtypedef)
- [ListTagsForResourceRequestTypeDef](./type_defs.md#listtagsforresourcerequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [TimestampTypeDef](./type_defs.md#timestamptypedef)
- [TagResourceRequestTypeDef](./type_defs.md#tagresourcerequesttypedef)
- [UntagResourceRequestTypeDef](./type_defs.md#untagresourcerequesttypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [PutDeploymentParameterResponseTypeDef](./type_defs.md#putdeploymentparameterresponsetypedef)
- [PutDeploymentParameterRequestTypeDef](./type_defs.md#putdeploymentparameterrequesttypedef)

