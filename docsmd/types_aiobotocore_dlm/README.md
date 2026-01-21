# DLM module

> [Index](../README.md) > DLM


!!! note ""

    Auto-generated documentation for [DLM](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dlm.html#dlm)
    type annotations stubs module [types-aiobotocore-dlm](https://pypi.org/project/types-aiobotocore-dlm/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy-boto3-builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==3.1.1' mypy-boto3-builder`
1. Select `aiobotocore` AWS SDK.
1. Add `DLM` service.
1. Use provided commands to install generated packages.



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

```python
# DLMClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_dlm.client import DLMClient


session = get_session()
async with session.create_client("dlm") as client:
    client: DLMClient
```








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# DefaultPoliciesTypeValuesType usage example

from types_aiobotocore_dlm.literals import DefaultPoliciesTypeValuesType

def get_value() -> DefaultPoliciesTypeValuesType:
    return "ALL"
```

- [DefaultPoliciesTypeValuesType](./literals.md#defaultpoliciestypevaluestype)
- [DefaultPolicyTypeValuesType](./literals.md#defaultpolicytypevaluestype)
- [EventSourceValuesType](./literals.md#eventsourcevaluestype)
- [EventTypeValuesType](./literals.md#eventtypevaluestype)
- [ExecutionHandlerServiceValuesType](./literals.md#executionhandlerservicevaluestype)
- [GettablePolicyStateValuesType](./literals.md#gettablepolicystatevaluestype)
- [IntervalUnitValuesType](./literals.md#intervalunitvaluestype)
- [LocationValuesType](./literals.md#locationvaluestype)
- [PolicyLanguageValuesType](./literals.md#policylanguagevaluestype)
- [PolicyTypeValuesType](./literals.md#policytypevaluestype)
- [ResourceLocationValuesType](./literals.md#resourcelocationvaluestype)
- [ResourceTypeValuesType](./literals.md#resourcetypevaluestype)
- [RetentionIntervalUnitValuesType](./literals.md#retentionintervalunitvaluestype)
- [SettablePolicyStateValuesType](./literals.md#settablepolicystatevaluestype)
- [StageValuesType](./literals.md#stagevaluestype)
- [DLMServiceName](./literals.md#dlmservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [RetentionArchiveTierTypeDef](./type_defs.md#retentionarchivetiertypedef)
- [CrossRegionCopyTargetTypeDef](./type_defs.md#crossregioncopytargettypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [ScriptOutputTypeDef](./type_defs.md#scriptoutputtypedef)
- [ScriptTypeDef](./type_defs.md#scripttypedef)
- [CrossRegionCopyRetainRuleTypeDef](./type_defs.md#crossregioncopyretainruletypedef)
- [EncryptionConfigurationTypeDef](./type_defs.md#encryptionconfigurationtypedef)
- [CrossRegionCopyDeprecateRuleTypeDef](./type_defs.md#crossregioncopydeprecateruletypedef)
- [DeleteLifecyclePolicyRequestTypeDef](./type_defs.md#deletelifecyclepolicyrequesttypedef)
- [DeprecateRuleTypeDef](./type_defs.md#deprecateruletypedef)
- [EventParametersOutputTypeDef](./type_defs.md#eventparametersoutputtypedef)
- [EventParametersTypeDef](./type_defs.md#eventparameterstypedef)
- [TagTypeDef](./type_defs.md#tagtypedef)
- [FastRestoreRuleOutputTypeDef](./type_defs.md#fastrestoreruleoutputtypedef)
- [FastRestoreRuleTypeDef](./type_defs.md#fastrestoreruletypedef)
- [GetLifecyclePoliciesRequestTypeDef](./type_defs.md#getlifecyclepoliciesrequesttypedef)
- [LifecyclePolicySummaryTypeDef](./type_defs.md#lifecyclepolicysummarytypedef)
- [GetLifecyclePolicyRequestTypeDef](./type_defs.md#getlifecyclepolicyrequesttypedef)
- [ListTagsForResourceRequestTypeDef](./type_defs.md#listtagsforresourcerequesttypedef)
- [RetainRuleTypeDef](./type_defs.md#retainruletypedef)
- [ShareRuleOutputTypeDef](./type_defs.md#shareruleoutputtypedef)
- [ShareRuleTypeDef](./type_defs.md#shareruletypedef)
- [TagResourceRequestTypeDef](./type_defs.md#tagresourcerequesttypedef)
- [UntagResourceRequestTypeDef](./type_defs.md#untagresourcerequesttypedef)
- [ArchiveRetainRuleTypeDef](./type_defs.md#archiveretainruletypedef)
- [CreateLifecyclePolicyResponseTypeDef](./type_defs.md#createlifecyclepolicyresponsetypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [CreateRuleOutputTypeDef](./type_defs.md#createruleoutputtypedef)
- [CreateRuleTypeDef](./type_defs.md#createruletypedef)
- [CrossRegionCopyActionTypeDef](./type_defs.md#crossregioncopyactiontypedef)
- [CrossRegionCopyRuleTypeDef](./type_defs.md#crossregioncopyruletypedef)
- [EventSourceOutputTypeDef](./type_defs.md#eventsourceoutputtypedef)
- [EventSourceTypeDef](./type_defs.md#eventsourcetypedef)
- [ExclusionsOutputTypeDef](./type_defs.md#exclusionsoutputtypedef)
- [ExclusionsTypeDef](./type_defs.md#exclusionstypedef)
- [ParametersOutputTypeDef](./type_defs.md#parametersoutputtypedef)
- [ParametersTypeDef](./type_defs.md#parameterstypedef)
- [GetLifecyclePoliciesResponseTypeDef](./type_defs.md#getlifecyclepoliciesresponsetypedef)
- [ArchiveRuleTypeDef](./type_defs.md#archiveruletypedef)
- [ActionOutputTypeDef](./type_defs.md#actionoutputtypedef)
- [ActionTypeDef](./type_defs.md#actiontypedef)
- [ExclusionsUnionTypeDef](./type_defs.md#exclusionsuniontypedef)
- [ScheduleOutputTypeDef](./type_defs.md#scheduleoutputtypedef)
- [ScheduleTypeDef](./type_defs.md#scheduletypedef)
- [PolicyDetailsOutputTypeDef](./type_defs.md#policydetailsoutputtypedef)
- [PolicyDetailsTypeDef](./type_defs.md#policydetailstypedef)
- [LifecyclePolicyTypeDef](./type_defs.md#lifecyclepolicytypedef)
- [PolicyDetailsUnionTypeDef](./type_defs.md#policydetailsuniontypedef)
- [GetLifecyclePolicyResponseTypeDef](./type_defs.md#getlifecyclepolicyresponsetypedef)
- [CreateLifecyclePolicyRequestTypeDef](./type_defs.md#createlifecyclepolicyrequesttypedef)
- [UpdateLifecyclePolicyRequestTypeDef](./type_defs.md#updatelifecyclepolicyrequesttypedef)

