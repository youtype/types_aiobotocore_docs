# FIS module

> [Index](../README.md) > FIS


!!! note ""

    Auto-generated documentation for [FIS](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fis.html#FIS)
    type annotations stubs module [types-aiobotocore-fis](https://pypi.org/project/types-aiobotocore-fis/).

## How to install



### From PyPI with pip

Install `types-aiobotocore` for `FIS` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[fis]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[fis]'


# standalone installation
python -m pip install types-aiobotocore-fis
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-fis
```

## Usage

Code samples can be found in [Examples](./usage.md).

## FISClient

Type annotations and code completion for  `#!python session.create_client("fis")` as [FISClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fis.html#FIS.Client)

```python
# FISClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_fis.client import FISClient


session = get_session()
async with session.create_client("fis") as client:
    client: FISClient
```








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# AccountTargetingType usage example

from types_aiobotocore_fis.literals import AccountTargetingType

def get_value() -> AccountTargetingType:
    return "multi-account"
```

- [AccountTargetingType](./literals.md#accounttargetingtype)
- [ActionsModeType](./literals.md#actionsmodetype)
- [EmptyTargetResolutionModeType](./literals.md#emptytargetresolutionmodetype)
- [ExperimentActionStatusType](./literals.md#experimentactionstatustype)
- [ExperimentStatusType](./literals.md#experimentstatustype)
- [SafetyLeverStatusInputType](./literals.md#safetyleverstatusinputtype)
- [SafetyLeverStatusType](./literals.md#safetyleverstatustype)
- [FISServiceName](./literals.md#fisservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [ActionParameterTypeDef](./type_defs.md#actionparametertypedef)
- [ActionTargetTypeDef](./type_defs.md#actiontargettypedef)
- [CreateExperimentTemplateActionInputTypeDef](./type_defs.md#createexperimenttemplateactioninputtypedef)
- [CreateExperimentTemplateExperimentOptionsInputTypeDef](./type_defs.md#createexperimenttemplateexperimentoptionsinputtypedef)
- [ExperimentTemplateCloudWatchLogsLogConfigurationInputTypeDef](./type_defs.md#experimenttemplatecloudwatchlogslogconfigurationinputtypedef)
- [ExperimentTemplateS3LogConfigurationInputTypeDef](./type_defs.md#experimenttemplates3logconfigurationinputtypedef)
- [CreateExperimentTemplateStopConditionInputTypeDef](./type_defs.md#createexperimenttemplatestopconditioninputtypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [ExperimentTemplateTargetInputFilterTypeDef](./type_defs.md#experimenttemplatetargetinputfiltertypedef)
- [CreateTargetAccountConfigurationRequestRequestTypeDef](./type_defs.md#createtargetaccountconfigurationrequestrequesttypedef)
- [TargetAccountConfigurationTypeDef](./type_defs.md#targetaccountconfigurationtypedef)
- [DeleteExperimentTemplateRequestRequestTypeDef](./type_defs.md#deleteexperimenttemplaterequestrequesttypedef)
- [DeleteTargetAccountConfigurationRequestRequestTypeDef](./type_defs.md#deletetargetaccountconfigurationrequestrequesttypedef)
- [ExperimentActionStateTypeDef](./type_defs.md#experimentactionstatetypedef)
- [ExperimentCloudWatchLogsLogConfigurationTypeDef](./type_defs.md#experimentcloudwatchlogslogconfigurationtypedef)
- [ExperimentErrorTypeDef](./type_defs.md#experimenterrortypedef)
- [ExperimentS3LogConfigurationTypeDef](./type_defs.md#experiments3logconfigurationtypedef)
- [ExperimentOptionsTypeDef](./type_defs.md#experimentoptionstypedef)
- [ExperimentStopConditionTypeDef](./type_defs.md#experimentstopconditiontypedef)
- [ExperimentTargetAccountConfigurationSummaryTypeDef](./type_defs.md#experimenttargetaccountconfigurationsummarytypedef)
- [ExperimentTargetAccountConfigurationTypeDef](./type_defs.md#experimenttargetaccountconfigurationtypedef)
- [ExperimentTargetFilterTypeDef](./type_defs.md#experimenttargetfiltertypedef)
- [ExperimentTemplateActionTypeDef](./type_defs.md#experimenttemplateactiontypedef)
- [ExperimentTemplateCloudWatchLogsLogConfigurationTypeDef](./type_defs.md#experimenttemplatecloudwatchlogslogconfigurationtypedef)
- [ExperimentTemplateExperimentOptionsTypeDef](./type_defs.md#experimenttemplateexperimentoptionstypedef)
- [ExperimentTemplateS3LogConfigurationTypeDef](./type_defs.md#experimenttemplates3logconfigurationtypedef)
- [ExperimentTemplateStopConditionTypeDef](./type_defs.md#experimenttemplatestopconditiontypedef)
- [ExperimentTemplateSummaryTypeDef](./type_defs.md#experimenttemplatesummarytypedef)
- [ExperimentTemplateTargetFilterTypeDef](./type_defs.md#experimenttemplatetargetfiltertypedef)
- [GetActionRequestRequestTypeDef](./type_defs.md#getactionrequestrequesttypedef)
- [GetExperimentRequestRequestTypeDef](./type_defs.md#getexperimentrequestrequesttypedef)
- [GetExperimentTargetAccountConfigurationRequestRequestTypeDef](./type_defs.md#getexperimenttargetaccountconfigurationrequestrequesttypedef)
- [GetExperimentTemplateRequestRequestTypeDef](./type_defs.md#getexperimenttemplaterequestrequesttypedef)
- [GetSafetyLeverRequestRequestTypeDef](./type_defs.md#getsafetyleverrequestrequesttypedef)
- [GetTargetAccountConfigurationRequestRequestTypeDef](./type_defs.md#gettargetaccountconfigurationrequestrequesttypedef)
- [GetTargetResourceTypeRequestRequestTypeDef](./type_defs.md#gettargetresourcetyperequestrequesttypedef)
- [ListActionsRequestRequestTypeDef](./type_defs.md#listactionsrequestrequesttypedef)
- [ListExperimentResolvedTargetsRequestRequestTypeDef](./type_defs.md#listexperimentresolvedtargetsrequestrequesttypedef)
- [ResolvedTargetTypeDef](./type_defs.md#resolvedtargettypedef)
- [ListExperimentTargetAccountConfigurationsRequestRequestTypeDef](./type_defs.md#listexperimenttargetaccountconfigurationsrequestrequesttypedef)
- [ListExperimentTemplatesRequestRequestTypeDef](./type_defs.md#listexperimenttemplatesrequestrequesttypedef)
- [ListExperimentsRequestRequestTypeDef](./type_defs.md#listexperimentsrequestrequesttypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [ListTargetAccountConfigurationsRequestRequestTypeDef](./type_defs.md#listtargetaccountconfigurationsrequestrequesttypedef)
- [TargetAccountConfigurationSummaryTypeDef](./type_defs.md#targetaccountconfigurationsummarytypedef)
- [ListTargetResourceTypesRequestRequestTypeDef](./type_defs.md#listtargetresourcetypesrequestrequesttypedef)
- [TargetResourceTypeSummaryTypeDef](./type_defs.md#targetresourcetypesummarytypedef)
- [SafetyLeverStateTypeDef](./type_defs.md#safetyleverstatetypedef)
- [StartExperimentExperimentOptionsInputTypeDef](./type_defs.md#startexperimentexperimentoptionsinputtypedef)
- [StopExperimentRequestRequestTypeDef](./type_defs.md#stopexperimentrequestrequesttypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [TargetResourceTypeParameterTypeDef](./type_defs.md#targetresourcetypeparametertypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [UpdateExperimentTemplateActionInputItemTypeDef](./type_defs.md#updateexperimenttemplateactioninputitemtypedef)
- [UpdateExperimentTemplateExperimentOptionsInputTypeDef](./type_defs.md#updateexperimenttemplateexperimentoptionsinputtypedef)
- [UpdateExperimentTemplateStopConditionInputTypeDef](./type_defs.md#updateexperimenttemplatestopconditioninputtypedef)
- [UpdateSafetyLeverStateInputTypeDef](./type_defs.md#updatesafetyleverstateinputtypedef)
- [UpdateTargetAccountConfigurationRequestRequestTypeDef](./type_defs.md#updatetargetaccountconfigurationrequestrequesttypedef)
- [ActionSummaryTypeDef](./type_defs.md#actionsummarytypedef)
- [ActionTypeDef](./type_defs.md#actiontypedef)
- [CreateExperimentTemplateLogConfigurationInputTypeDef](./type_defs.md#createexperimenttemplatelogconfigurationinputtypedef)
- [UpdateExperimentTemplateLogConfigurationInputTypeDef](./type_defs.md#updateexperimenttemplatelogconfigurationinputtypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [CreateExperimentTemplateTargetInputTypeDef](./type_defs.md#createexperimenttemplatetargetinputtypedef)
- [UpdateExperimentTemplateTargetInputTypeDef](./type_defs.md#updateexperimenttemplatetargetinputtypedef)
- [CreateTargetAccountConfigurationResponseTypeDef](./type_defs.md#createtargetaccountconfigurationresponsetypedef)
- [DeleteTargetAccountConfigurationResponseTypeDef](./type_defs.md#deletetargetaccountconfigurationresponsetypedef)
- [GetTargetAccountConfigurationResponseTypeDef](./type_defs.md#gettargetaccountconfigurationresponsetypedef)
- [UpdateTargetAccountConfigurationResponseTypeDef](./type_defs.md#updatetargetaccountconfigurationresponsetypedef)
- [ExperimentActionTypeDef](./type_defs.md#experimentactiontypedef)
- [ExperimentStateTypeDef](./type_defs.md#experimentstatetypedef)
- [ExperimentLogConfigurationTypeDef](./type_defs.md#experimentlogconfigurationtypedef)
- [ListExperimentTargetAccountConfigurationsResponseTypeDef](./type_defs.md#listexperimenttargetaccountconfigurationsresponsetypedef)
- [GetExperimentTargetAccountConfigurationResponseTypeDef](./type_defs.md#getexperimenttargetaccountconfigurationresponsetypedef)
- [ExperimentTargetTypeDef](./type_defs.md#experimenttargettypedef)
- [ExperimentTemplateLogConfigurationTypeDef](./type_defs.md#experimenttemplatelogconfigurationtypedef)
- [ListExperimentTemplatesResponseTypeDef](./type_defs.md#listexperimenttemplatesresponsetypedef)
- [ExperimentTemplateTargetTypeDef](./type_defs.md#experimenttemplatetargettypedef)
- [ListExperimentResolvedTargetsResponseTypeDef](./type_defs.md#listexperimentresolvedtargetsresponsetypedef)
- [ListTargetAccountConfigurationsResponseTypeDef](./type_defs.md#listtargetaccountconfigurationsresponsetypedef)
- [ListTargetResourceTypesResponseTypeDef](./type_defs.md#listtargetresourcetypesresponsetypedef)
- [SafetyLeverTypeDef](./type_defs.md#safetylevertypedef)
- [StartExperimentRequestRequestTypeDef](./type_defs.md#startexperimentrequestrequesttypedef)
- [TargetResourceTypeTypeDef](./type_defs.md#targetresourcetypetypedef)
- [UpdateSafetyLeverStateRequestRequestTypeDef](./type_defs.md#updatesafetyleverstaterequestrequesttypedef)
- [ListActionsResponseTypeDef](./type_defs.md#listactionsresponsetypedef)
- [GetActionResponseTypeDef](./type_defs.md#getactionresponsetypedef)
- [CreateExperimentTemplateRequestRequestTypeDef](./type_defs.md#createexperimenttemplaterequestrequesttypedef)
- [UpdateExperimentTemplateRequestRequestTypeDef](./type_defs.md#updateexperimenttemplaterequestrequesttypedef)
- [ExperimentSummaryTypeDef](./type_defs.md#experimentsummarytypedef)
- [ExperimentTypeDef](./type_defs.md#experimenttypedef)
- [ExperimentTemplateTypeDef](./type_defs.md#experimenttemplatetypedef)
- [GetSafetyLeverResponseTypeDef](./type_defs.md#getsafetyleverresponsetypedef)
- [UpdateSafetyLeverStateResponseTypeDef](./type_defs.md#updatesafetyleverstateresponsetypedef)
- [GetTargetResourceTypeResponseTypeDef](./type_defs.md#gettargetresourcetyperesponsetypedef)
- [ListExperimentsResponseTypeDef](./type_defs.md#listexperimentsresponsetypedef)
- [GetExperimentResponseTypeDef](./type_defs.md#getexperimentresponsetypedef)
- [StartExperimentResponseTypeDef](./type_defs.md#startexperimentresponsetypedef)
- [StopExperimentResponseTypeDef](./type_defs.md#stopexperimentresponsetypedef)
- [CreateExperimentTemplateResponseTypeDef](./type_defs.md#createexperimenttemplateresponsetypedef)
- [DeleteExperimentTemplateResponseTypeDef](./type_defs.md#deleteexperimenttemplateresponsetypedef)
- [GetExperimentTemplateResponseTypeDef](./type_defs.md#getexperimenttemplateresponsetypedef)
- [UpdateExperimentTemplateResponseTypeDef](./type_defs.md#updateexperimenttemplateresponsetypedef)

