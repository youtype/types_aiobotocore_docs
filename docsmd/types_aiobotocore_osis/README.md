# OpenSearchIngestion module

> [Index](../README.md) > OpenSearchIngestion


!!! note ""

    Auto-generated documentation for [OpenSearchIngestion](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/osis.html#opensearchingestion)
    type annotations stubs module [types-aiobotocore-osis](https://pypi.org/project/types-aiobotocore-osis/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy-boto3-builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.23.2' mypy-boto3-builder`
1. Select `aiobotocore` AWS SDK.
1. Add `OpenSearchIngestion` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `OpenSearchIngestion` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[osis]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[osis]'

# standalone installation
python -m pip install types-aiobotocore-osis
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-osis
```

## Usage

Code samples can be found in [Examples](./usage.md).

## OpenSearchIngestionClient

Type annotations and code completion for  `#!python session.create_client("osis")` as [OpenSearchIngestionClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/osis.html#OpenSearchIngestion.Client)

```python
# OpenSearchIngestionClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_osis.client import OpenSearchIngestionClient


session = get_session()
async with session.create_client("osis") as client:
    client: OpenSearchIngestionClient
```








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# ChangeProgressStageStatusesType usage example

from types_aiobotocore_osis.literals import ChangeProgressStageStatusesType

def get_value() -> ChangeProgressStageStatusesType:
    return "COMPLETED"
```

- [ChangeProgressStageStatusesType](./literals.md#changeprogressstagestatusestype)
- [ChangeProgressStatusesType](./literals.md#changeprogressstatusestype)
- [PipelineStatusType](./literals.md#pipelinestatustype)
- [VpcEndpointManagementType](./literals.md#vpcendpointmanagementtype)
- [VpcEndpointServiceNameType](./literals.md#vpcendpointservicenametype)
- [OpenSearchIngestionServiceName](./literals.md#opensearchingestionservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [BufferOptionsTypeDef](./type_defs.md#bufferoptionstypedef)
- [ChangeProgressStageTypeDef](./type_defs.md#changeprogressstagetypedef)
- [CloudWatchLogDestinationTypeDef](./type_defs.md#cloudwatchlogdestinationtypedef)
- [EncryptionAtRestOptionsTypeDef](./type_defs.md#encryptionatrestoptionstypedef)
- [TagTypeDef](./type_defs.md#tagtypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [DeletePipelineRequestTypeDef](./type_defs.md#deletepipelinerequesttypedef)
- [GetPipelineBlueprintRequestTypeDef](./type_defs.md#getpipelineblueprintrequesttypedef)
- [PipelineBlueprintTypeDef](./type_defs.md#pipelineblueprinttypedef)
- [GetPipelineChangeProgressRequestTypeDef](./type_defs.md#getpipelinechangeprogressrequesttypedef)
- [GetPipelineRequestTypeDef](./type_defs.md#getpipelinerequesttypedef)
- [PipelineBlueprintSummaryTypeDef](./type_defs.md#pipelineblueprintsummarytypedef)
- [ListPipelinesRequestTypeDef](./type_defs.md#listpipelinesrequesttypedef)
- [ListTagsForResourceRequestTypeDef](./type_defs.md#listtagsforresourcerequesttypedef)
- [PipelineDestinationTypeDef](./type_defs.md#pipelinedestinationtypedef)
- [PipelineStatusReasonTypeDef](./type_defs.md#pipelinestatusreasontypedef)
- [ServiceVpcEndpointTypeDef](./type_defs.md#servicevpcendpointtypedef)
- [StartPipelineRequestTypeDef](./type_defs.md#startpipelinerequesttypedef)
- [StopPipelineRequestTypeDef](./type_defs.md#stoppipelinerequesttypedef)
- [UntagResourceRequestTypeDef](./type_defs.md#untagresourcerequesttypedef)
- [ValidatePipelineRequestTypeDef](./type_defs.md#validatepipelinerequesttypedef)
- [ValidationMessageTypeDef](./type_defs.md#validationmessagetypedef)
- [VpcAttachmentOptionsTypeDef](./type_defs.md#vpcattachmentoptionstypedef)
- [ChangeProgressStatusTypeDef](./type_defs.md#changeprogressstatustypedef)
- [LogPublishingOptionsTypeDef](./type_defs.md#logpublishingoptionstypedef)
- [TagResourceRequestTypeDef](./type_defs.md#tagresourcerequesttypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [GetPipelineBlueprintResponseTypeDef](./type_defs.md#getpipelineblueprintresponsetypedef)
- [ListPipelineBlueprintsResponseTypeDef](./type_defs.md#listpipelineblueprintsresponsetypedef)
- [PipelineSummaryTypeDef](./type_defs.md#pipelinesummarytypedef)
- [ValidatePipelineResponseTypeDef](./type_defs.md#validatepipelineresponsetypedef)
- [VpcOptionsOutputTypeDef](./type_defs.md#vpcoptionsoutputtypedef)
- [VpcOptionsTypeDef](./type_defs.md#vpcoptionstypedef)
- [GetPipelineChangeProgressResponseTypeDef](./type_defs.md#getpipelinechangeprogressresponsetypedef)
- [UpdatePipelineRequestTypeDef](./type_defs.md#updatepipelinerequesttypedef)
- [ListPipelinesResponseTypeDef](./type_defs.md#listpipelinesresponsetypedef)
- [VpcEndpointTypeDef](./type_defs.md#vpcendpointtypedef)
- [VpcOptionsUnionTypeDef](./type_defs.md#vpcoptionsuniontypedef)
- [PipelineTypeDef](./type_defs.md#pipelinetypedef)
- [CreatePipelineRequestTypeDef](./type_defs.md#createpipelinerequesttypedef)
- [CreatePipelineResponseTypeDef](./type_defs.md#createpipelineresponsetypedef)
- [GetPipelineResponseTypeDef](./type_defs.md#getpipelineresponsetypedef)
- [StartPipelineResponseTypeDef](./type_defs.md#startpipelineresponsetypedef)
- [StopPipelineResponseTypeDef](./type_defs.md#stoppipelineresponsetypedef)
- [UpdatePipelineResponseTypeDef](./type_defs.md#updatepipelineresponsetypedef)

