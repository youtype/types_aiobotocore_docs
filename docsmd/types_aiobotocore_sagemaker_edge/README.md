# SagemakerEdgeManager module

> [Index](../README.md) > SagemakerEdgeManager


!!! note ""

    Auto-generated documentation for [SagemakerEdgeManager](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-edge.html#SagemakerEdgeManager)
    type annotations stubs module [types-aiobotocore-sagemaker-edge](https://pypi.org/project/types-aiobotocore-sagemaker-edge/).

## How to install



### From PyPI with pip

Install `types-aiobotocore` for `SagemakerEdgeManager` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[sagemaker-edge]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[sagemaker-edge]'


# standalone installation
python -m pip install types-aiobotocore-sagemaker-edge
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-sagemaker-edge
```

## Usage

Code samples can be found in [Examples](./usage.md).

## SagemakerEdgeManagerClient

Type annotations and code completion for  `#!python session.create_client("sagemaker-edge")` as [SagemakerEdgeManagerClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-edge.html#SagemakerEdgeManager.Client)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_sagemaker_edge.client import SagemakerEdgeManagerClient


session = get_session()
async with session.create_client("sagemaker-edge") as client:
    client: SagemakerEdgeManagerClient
```








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_sagemaker_edge.literals import ChecksumTypeType

def get_value() -> ChecksumTypeType:
    return "SHA1"
```

- [ChecksumTypeType](./literals.md#checksumtypetype)
- [DeploymentStatusType](./literals.md#deploymentstatustype)
- [DeploymentTypeType](./literals.md#deploymenttypetype)
- [FailureHandlingPolicyType](./literals.md#failurehandlingpolicytype)
- [ModelStateType](./literals.md#modelstatetype)
- [SagemakerEdgeManagerServiceName](./literals.md#sagemakeredgemanagerservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [RegionName](./literals.md#regionname)




## Typed dictionaries

Type annotations for [typed dictionaries](./type_defs.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_sagemaker_edge.type_defs import ChecksumTypeDef

def get_value() -> ChecksumTypeDef:
    return {
        "Type": ...,
    }
```

- [ChecksumTypeDef](./type_defs.md#checksumtypedef)
- [DeploymentModelTypeDef](./type_defs.md#deploymentmodeltypedef)
- [EdgeMetricTypeDef](./type_defs.md#edgemetrictypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [GetDeploymentsRequestRequestTypeDef](./type_defs.md#getdeploymentsrequestrequesttypedef)
- [GetDeviceRegistrationRequestRequestTypeDef](./type_defs.md#getdeviceregistrationrequestrequesttypedef)
- [DefinitionTypeDef](./type_defs.md#definitiontypedef)
- [DeploymentResultTypeDef](./type_defs.md#deploymentresulttypedef)
- [ModelTypeDef](./type_defs.md#modeltypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [GetDeviceRegistrationResultTypeDef](./type_defs.md#getdeviceregistrationresulttypedef)
- [EdgeDeploymentTypeDef](./type_defs.md#edgedeploymenttypedef)
- [SendHeartbeatRequestRequestTypeDef](./type_defs.md#sendheartbeatrequestrequesttypedef)
- [GetDeploymentsResultTypeDef](./type_defs.md#getdeploymentsresulttypedef)

