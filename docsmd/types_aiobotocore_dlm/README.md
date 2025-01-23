# DLM module

> [Index](../README.md) > DLM


!!! note ""

    Auto-generated documentation for [DLM](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dlm.html#dlm)
    type annotations stubs module [types-aiobotocore-dlm](https://pypi.org/project/types-aiobotocore-dlm/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.19.0' mypy_boto3_builder`
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
- [CrossRegionCopyRetainRuleTypeDef](./type_defs.md#crossregioncopyretainruletypedef)
- [EncryptionConfigurationTypeDef](./type_defs.md#encryptionconfigurationtypedef)
- [CrossRegionCopyDeprecateRuleTypeDef](./type_defs.md#crossregioncopydeprecateruletypedef)
- [DeleteLifecyclePolicyRequestRequestTypeDef](./type_defs.md#deletelifecyclepolicyrequestrequesttypedef)
- [DeprecateRuleTypeDef](./type_defs.md#deprecateruletypedef)
- [EventParametersOutputTypeDef](./type_defs.md#eventparametersoutputtypedef)
- [EventParametersTypeDef](./type_defs.md#eventparameterstypedef)
- [TagTypeDef](./type_defs.md#tagtypedef)
- [FastRestoreRuleOutputTypeDef](./type_defs.md#fastrestoreruleoutputtypedef)
- [FastRestoreRuleTypeDef](./type_defs.md#fastrestoreruletypedef)
- [GetLifecyclePoliciesRequestRequestTypeDef](./type_defs.md#getlifecyclepoliciesrequestrequesttypedef)
- [LifecyclePolicySummaryTypeDef](./type_defs.md#lifecyclepolicysummarytypedef)
- [GetLifecyclePolicyRequestRequestTypeDef](./type_defs.md#getlifecyclepolicyrequestrequesttypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [RetainRuleTypeDef](./type_defs.md#retainruletypedef)
- [ShareRuleOutputTypeDef](./type_defs.md#shareruleoutputtypedef)
- [ScriptTypeDef](./type_defs.md#scripttypedef)
- [ShareRuleTypeDef](./type_defs.md#shareruletypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [ArchiveRetainRuleTypeDef](./type_defs.md#archiveretainruletypedef)
- [CreateLifecyclePolicyResponseTypeDef](./type_defs.md#createlifecyclepolicyresponsetypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [CreateRuleOutputTypeDef](./type_defs.md#createruleoutputtypedef)
- [CrossRegionCopyActionTypeDef](./type_defs.md#crossregioncopyactiontypedef)
- [CrossRegionCopyRuleTypeDef](./type_defs.md#crossregioncopyruletypedef)
- [EventSourceOutputTypeDef](./type_defs.md#eventsourceoutputtypedef)
- [EventParametersUnionTypeDef](./type_defs.md#eventparametersuniontypedef)
- [ExclusionsOutputTypeDef](./type_defs.md#exclusionsoutputtypedef)
- [ExclusionsTypeDef](./type_defs.md#exclusionstypedef)
- [ParametersOutputTypeDef](./type_defs.md#parametersoutputtypedef)
- [ParametersTypeDef](./type_defs.md#parameterstypedef)
- [FastRestoreRuleUnionTypeDef](./type_defs.md#fastrestoreruleuniontypedef)
- [GetLifecyclePoliciesResponseTypeDef](./type_defs.md#getlifecyclepoliciesresponsetypedef)
- [ScriptUnionTypeDef](./type_defs.md#scriptuniontypedef)
- [ShareRuleUnionTypeDef](./type_defs.md#shareruleuniontypedef)
- [ArchiveRuleTypeDef](./type_defs.md#archiveruletypedef)
- [ActionOutputTypeDef](./type_defs.md#actionoutputtypedef)
- [ActionTypeDef](./type_defs.md#actiontypedef)
- [EventSourceTypeDef](./type_defs.md#eventsourcetypedef)
- [ExclusionsUnionTypeDef](./type_defs.md#exclusionsuniontypedef)
- [ParametersUnionTypeDef](./type_defs.md#parametersuniontypedef)
- [CreateRuleTypeDef](./type_defs.md#createruletypedef)
- [ScheduleOutputTypeDef](./type_defs.md#scheduleoutputtypedef)
- [ActionUnionTypeDef](./type_defs.md#actionuniontypedef)
- [EventSourceUnionTypeDef](./type_defs.md#eventsourceuniontypedef)
- [CreateRuleUnionTypeDef](./type_defs.md#createruleuniontypedef)
- [PolicyDetailsOutputTypeDef](./type_defs.md#policydetailsoutputtypedef)
- [ScheduleTypeDef](./type_defs.md#scheduletypedef)
- [LifecyclePolicyTypeDef](./type_defs.md#lifecyclepolicytypedef)
- [ScheduleUnionTypeDef](./type_defs.md#scheduleuniontypedef)
- [GetLifecyclePolicyResponseTypeDef](./type_defs.md#getlifecyclepolicyresponsetypedef)
- [PolicyDetailsTypeDef](./type_defs.md#policydetailstypedef)
- [CreateLifecyclePolicyRequestRequestTypeDef](./type_defs.md#createlifecyclepolicyrequestrequesttypedef)
- [UpdateLifecyclePolicyRequestRequestTypeDef](./type_defs.md#updatelifecyclepolicyrequestrequesttypedef)

