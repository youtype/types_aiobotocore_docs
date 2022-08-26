# DLM module

> [Index](../README.md) > DLM


!!! note ""

    Auto-generated documentation for [DLM](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dlm.html#DLM)
    type annotations stubs module [types-aiobotocore-dlm](https://pypi.org/project/types-aiobotocore-dlm/).

## How to install



### From PyPI with pip

Install `types-aiobotocore` for `DLM` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[dlm]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[dlm]'


# standalone installation
python -m pip install types-aiobotocore-dlm
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-dlm
```

## Usage

Code samples can be found in [Examples](./usage.md).

## DLMClient

Type annotations and code completion for  `#!python session.create_client("dlm")` as [DLMClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dlm.html#DLM.Client)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_dlm.client import DLMClient


session = get_session()
async with session.create_client("dlm") as client:
    client: DLMClient
```








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_dlm.literals import EventSourceValuesType

def get_value() -> EventSourceValuesType:
    return "MANAGED_CWE"
```

- [EventSourceValuesType](./literals.md#eventsourcevaluestype)
- [EventTypeValuesType](./literals.md#eventtypevaluestype)
- [GettablePolicyStateValuesType](./literals.md#gettablepolicystatevaluestype)
- [IntervalUnitValuesType](./literals.md#intervalunitvaluestype)
- [LocationValuesType](./literals.md#locationvaluestype)
- [PolicyTypeValuesType](./literals.md#policytypevaluestype)
- [ResourceLocationValuesType](./literals.md#resourcelocationvaluestype)
- [ResourceTypeValuesType](./literals.md#resourcetypevaluestype)
- [RetentionIntervalUnitValuesType](./literals.md#retentionintervalunitvaluestype)
- [SettablePolicyStateValuesType](./literals.md#settablepolicystatevaluestype)
- [DLMServiceName](./literals.md#dlmservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [RegionName](./literals.md#regionname)




## Typed dictionaries

Type annotations for [typed dictionaries](./type_defs.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_dlm.type_defs import ResponseMetadataTypeDef

def get_value() -> ResponseMetadataTypeDef:
    return {
        "RequestId": ...,
        "HostId": ...,
        "HTTPStatusCode": ...,
        "HTTPHeaders": ...,
        "RetryAttempts": ...,
    }
```

- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [CreateRuleTypeDef](./type_defs.md#createruletypedef)
- [CrossRegionCopyRetainRuleTypeDef](./type_defs.md#crossregioncopyretainruletypedef)
- [EncryptionConfigurationTypeDef](./type_defs.md#encryptionconfigurationtypedef)
- [CrossRegionCopyDeprecateRuleTypeDef](./type_defs.md#crossregioncopydeprecateruletypedef)
- [DeleteLifecyclePolicyRequestRequestTypeDef](./type_defs.md#deletelifecyclepolicyrequestrequesttypedef)
- [DeprecateRuleTypeDef](./type_defs.md#deprecateruletypedef)
- [EventParametersTypeDef](./type_defs.md#eventparameterstypedef)
- [FastRestoreRuleTypeDef](./type_defs.md#fastrestoreruletypedef)
- [GetLifecyclePoliciesRequestRequestTypeDef](./type_defs.md#getlifecyclepoliciesrequestrequesttypedef)
- [LifecyclePolicySummaryTypeDef](./type_defs.md#lifecyclepolicysummarytypedef)
- [GetLifecyclePolicyRequestRequestTypeDef](./type_defs.md#getlifecyclepolicyrequestrequesttypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [TagTypeDef](./type_defs.md#tagtypedef)
- [RetainRuleTypeDef](./type_defs.md#retainruletypedef)
- [ShareRuleTypeDef](./type_defs.md#shareruletypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [CreateLifecyclePolicyResponseTypeDef](./type_defs.md#createlifecyclepolicyresponsetypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [CrossRegionCopyActionTypeDef](./type_defs.md#crossregioncopyactiontypedef)
- [CrossRegionCopyRuleTypeDef](./type_defs.md#crossregioncopyruletypedef)
- [EventSourceTypeDef](./type_defs.md#eventsourcetypedef)
- [GetLifecyclePoliciesResponseTypeDef](./type_defs.md#getlifecyclepoliciesresponsetypedef)
- [ParametersTypeDef](./type_defs.md#parameterstypedef)
- [ActionTypeDef](./type_defs.md#actiontypedef)
- [ScheduleTypeDef](./type_defs.md#scheduletypedef)
- [PolicyDetailsTypeDef](./type_defs.md#policydetailstypedef)
- [CreateLifecyclePolicyRequestRequestTypeDef](./type_defs.md#createlifecyclepolicyrequestrequesttypedef)
- [LifecyclePolicyTypeDef](./type_defs.md#lifecyclepolicytypedef)
- [UpdateLifecyclePolicyRequestRequestTypeDef](./type_defs.md#updatelifecyclepolicyrequestrequesttypedef)
- [GetLifecyclePolicyResponseTypeDef](./type_defs.md#getlifecyclepolicyresponsetypedef)

