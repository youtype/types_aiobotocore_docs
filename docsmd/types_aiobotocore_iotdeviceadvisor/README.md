# IoTDeviceAdvisor module

> [Index](../README.md) > IoTDeviceAdvisor


!!! note ""

    Auto-generated documentation for [IoTDeviceAdvisor](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotdeviceadvisor.html#iotdeviceadvisor)
    type annotations stubs module [types-aiobotocore-iotdeviceadvisor](https://pypi.org/project/types-aiobotocore-iotdeviceadvisor/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy-boto3-builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==3.1.1' mypy-boto3-builder`
1. Select `aiobotocore` AWS SDK.
1. Add `IoTDeviceAdvisor` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `IoTDeviceAdvisor` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[iotdeviceadvisor]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[iotdeviceadvisor]'

# standalone installation
python -m pip install types-aiobotocore-iotdeviceadvisor
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-iotdeviceadvisor
```

## Usage

Code samples can be found in [Examples](./usage.md).

## IoTDeviceAdvisorClient

Type annotations and code completion for  `#!python session.create_client("iotdeviceadvisor")` as [IoTDeviceAdvisorClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotdeviceadvisor.html#IoTDeviceAdvisor.Client)

```python
# IoTDeviceAdvisorClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_iotdeviceadvisor.client import IoTDeviceAdvisorClient


session = get_session()
async with session.create_client("iotdeviceadvisor") as client:
    client: IoTDeviceAdvisorClient
```








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# AuthenticationMethodType usage example

from types_aiobotocore_iotdeviceadvisor.literals import AuthenticationMethodType

def get_value() -> AuthenticationMethodType:
    return "SignatureVersion4"
```

- [AuthenticationMethodType](./literals.md#authenticationmethodtype)
- [ProtocolType](./literals.md#protocoltype)
- [StatusType](./literals.md#statustype)
- [SuiteRunStatusType](./literals.md#suiterunstatustype)
- [TestCaseScenarioStatusType](./literals.md#testcasescenariostatustype)
- [TestCaseScenarioTypeType](./literals.md#testcasescenariotypetype)
- [IoTDeviceAdvisorServiceName](./literals.md#iotdeviceadvisorservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [DeleteSuiteDefinitionRequestTypeDef](./type_defs.md#deletesuitedefinitionrequesttypedef)
- [DeviceUnderTestTypeDef](./type_defs.md#deviceundertesttypedef)
- [GetEndpointRequestTypeDef](./type_defs.md#getendpointrequesttypedef)
- [GetSuiteDefinitionRequestTypeDef](./type_defs.md#getsuitedefinitionrequesttypedef)
- [GetSuiteRunReportRequestTypeDef](./type_defs.md#getsuiterunreportrequesttypedef)
- [GetSuiteRunRequestTypeDef](./type_defs.md#getsuiterunrequesttypedef)
- [ListSuiteDefinitionsRequestTypeDef](./type_defs.md#listsuitedefinitionsrequesttypedef)
- [ListSuiteRunsRequestTypeDef](./type_defs.md#listsuiterunsrequesttypedef)
- [SuiteRunInformationTypeDef](./type_defs.md#suiteruninformationtypedef)
- [ListTagsForResourceRequestTypeDef](./type_defs.md#listtagsforresourcerequesttypedef)
- [StopSuiteRunRequestTypeDef](./type_defs.md#stopsuiterunrequesttypedef)
- [TagResourceRequestTypeDef](./type_defs.md#tagresourcerequesttypedef)
- [TestCaseScenarioTypeDef](./type_defs.md#testcasescenariotypedef)
- [UntagResourceRequestTypeDef](./type_defs.md#untagresourcerequesttypedef)
- [CreateSuiteDefinitionResponseTypeDef](./type_defs.md#createsuitedefinitionresponsetypedef)
- [GetEndpointResponseTypeDef](./type_defs.md#getendpointresponsetypedef)
- [GetSuiteRunReportResponseTypeDef](./type_defs.md#getsuiterunreportresponsetypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [StartSuiteRunResponseTypeDef](./type_defs.md#startsuiterunresponsetypedef)
- [UpdateSuiteDefinitionResponseTypeDef](./type_defs.md#updatesuitedefinitionresponsetypedef)
- [SuiteDefinitionConfigurationOutputTypeDef](./type_defs.md#suitedefinitionconfigurationoutputtypedef)
- [SuiteDefinitionConfigurationTypeDef](./type_defs.md#suitedefinitionconfigurationtypedef)
- [SuiteDefinitionInformationTypeDef](./type_defs.md#suitedefinitioninformationtypedef)
- [SuiteRunConfigurationOutputTypeDef](./type_defs.md#suiterunconfigurationoutputtypedef)
- [SuiteRunConfigurationTypeDef](./type_defs.md#suiterunconfigurationtypedef)
- [ListSuiteRunsResponseTypeDef](./type_defs.md#listsuiterunsresponsetypedef)
- [TestCaseRunTypeDef](./type_defs.md#testcaseruntypedef)
- [GetSuiteDefinitionResponseTypeDef](./type_defs.md#getsuitedefinitionresponsetypedef)
- [SuiteDefinitionConfigurationUnionTypeDef](./type_defs.md#suitedefinitionconfigurationuniontypedef)
- [ListSuiteDefinitionsResponseTypeDef](./type_defs.md#listsuitedefinitionsresponsetypedef)
- [SuiteRunConfigurationUnionTypeDef](./type_defs.md#suiterunconfigurationuniontypedef)
- [GroupResultTypeDef](./type_defs.md#groupresulttypedef)
- [CreateSuiteDefinitionRequestTypeDef](./type_defs.md#createsuitedefinitionrequesttypedef)
- [UpdateSuiteDefinitionRequestTypeDef](./type_defs.md#updatesuitedefinitionrequesttypedef)
- [StartSuiteRunRequestTypeDef](./type_defs.md#startsuiterunrequesttypedef)
- [TestResultTypeDef](./type_defs.md#testresulttypedef)
- [GetSuiteRunResponseTypeDef](./type_defs.md#getsuiterunresponsetypedef)

