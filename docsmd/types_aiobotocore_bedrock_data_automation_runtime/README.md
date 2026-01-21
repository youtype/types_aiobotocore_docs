# RuntimeforBedrockDataAutomation module

> [Index](../README.md) > RuntimeforBedrockDataAutomation


!!! note ""

    Auto-generated documentation for [RuntimeforBedrockDataAutomation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-data-automation-runtime.html#runtimeforbedrockdataautomation)
    type annotations stubs module [types-aiobotocore-bedrock-data-automation-runtime](https://pypi.org/project/types-aiobotocore-bedrock-data-automation-runtime/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy-boto3-builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==3.1.1' mypy-boto3-builder`
1. Select `aiobotocore` AWS SDK.
1. Add `RuntimeforBedrockDataAutomation` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `RuntimeforBedrockDataAutomation` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[bedrock-data-automation-runtime]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[bedrock-data-automation-runtime]'

# standalone installation
python -m pip install types-aiobotocore-bedrock-data-automation-runtime
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-bedrock-data-automation-runtime
```

## Usage

Code samples can be found in [Examples](./usage.md).

## RuntimeforBedrockDataAutomationClient

Type annotations and code completion for  `#!python session.create_client("bedrock-data-automation-runtime")` as [RuntimeforBedrockDataAutomationClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-data-automation-runtime.html#RuntimeforBedrockDataAutomation.Client)

```python
# RuntimeforBedrockDataAutomationClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_bedrock_data_automation_runtime.client import RuntimeforBedrockDataAutomationClient


session = get_session()
async with session.create_client("bedrock-data-automation-runtime") as client:
    client: RuntimeforBedrockDataAutomationClient
```








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# AutomationJobStatusType usage example

from types_aiobotocore_bedrock_data_automation_runtime.literals import AutomationJobStatusType

def get_value() -> AutomationJobStatusType:
    return "ClientError"
```

- [AutomationJobStatusType](./literals.md#automationjobstatustype)
- [BlueprintStageType](./literals.md#blueprintstagetype)
- [CustomOutputStatusType](./literals.md#customoutputstatustype)
- [DataAutomationStageType](./literals.md#dataautomationstagetype)
- [SemanticModalityType](./literals.md#semanticmodalitytype)
- [RuntimeforBedrockDataAutomationServiceName](./literals.md#runtimeforbedrockdataautomationservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [BlobTypeDef](./type_defs.md#blobtypedef)
- [BlueprintTypeDef](./type_defs.md#blueprinttypedef)
- [DataAutomationConfigurationTypeDef](./type_defs.md#dataautomationconfigurationtypedef)
- [EncryptionConfigurationTypeDef](./type_defs.md#encryptionconfigurationtypedef)
- [EventBridgeConfigurationTypeDef](./type_defs.md#eventbridgeconfigurationtypedef)
- [GetDataAutomationStatusRequestTypeDef](./type_defs.md#getdataautomationstatusrequesttypedef)
- [OutputConfigurationTypeDef](./type_defs.md#outputconfigurationtypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [TagTypeDef](./type_defs.md#tagtypedef)
- [OutputSegmentTypeDef](./type_defs.md#outputsegmenttypedef)
- [ListTagsForResourceRequestTypeDef](./type_defs.md#listtagsforresourcerequesttypedef)
- [TimestampSegmentTypeDef](./type_defs.md#timestampsegmenttypedef)
- [UntagResourceRequestTypeDef](./type_defs.md#untagresourcerequesttypedef)
- [SyncInputConfigurationTypeDef](./type_defs.md#syncinputconfigurationtypedef)
- [NotificationConfigurationTypeDef](./type_defs.md#notificationconfigurationtypedef)
- [GetDataAutomationStatusResponseTypeDef](./type_defs.md#getdataautomationstatusresponsetypedef)
- [InvokeDataAutomationAsyncResponseTypeDef](./type_defs.md#invokedataautomationasyncresponsetypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [TagResourceRequestTypeDef](./type_defs.md#tagresourcerequesttypedef)
- [InvokeDataAutomationResponseTypeDef](./type_defs.md#invokedataautomationresponsetypedef)
- [VideoSegmentConfigurationTypeDef](./type_defs.md#videosegmentconfigurationtypedef)
- [InvokeDataAutomationRequestTypeDef](./type_defs.md#invokedataautomationrequesttypedef)
- [VideoAssetProcessingConfigurationTypeDef](./type_defs.md#videoassetprocessingconfigurationtypedef)
- [AssetProcessingConfigurationTypeDef](./type_defs.md#assetprocessingconfigurationtypedef)
- [InputConfigurationTypeDef](./type_defs.md#inputconfigurationtypedef)
- [InvokeDataAutomationAsyncRequestTypeDef](./type_defs.md#invokedataautomationasyncrequesttypedef)

