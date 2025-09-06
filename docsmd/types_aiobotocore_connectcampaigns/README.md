# ConnectCampaignService module

> [Index](../README.md) > ConnectCampaignService


!!! note ""

    Auto-generated documentation for [ConnectCampaignService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcampaigns.html#connectcampaignservice)
    type annotations stubs module [types-aiobotocore-connectcampaigns](https://pypi.org/project/types-aiobotocore-connectcampaigns/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy-boto3-builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.24.2' mypy-boto3-builder`
1. Select `aiobotocore` AWS SDK.
1. Add `ConnectCampaignService` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `ConnectCampaignService` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[connectcampaigns]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[connectcampaigns]'

# standalone installation
python -m pip install types-aiobotocore-connectcampaigns
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-connectcampaigns
```

## Usage

Code samples can be found in [Examples](./usage.md).

## ConnectCampaignServiceClient

Type annotations and code completion for  `#!python session.create_client("connectcampaigns")` as [ConnectCampaignServiceClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcampaigns.html#ConnectCampaignService.Client)

```python
# ConnectCampaignServiceClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_connectcampaigns.client import ConnectCampaignServiceClient


session = get_session()
async with session.create_client("connectcampaigns") as client:
    client: ConnectCampaignServiceClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("connectcampaigns").get_paginator("...")`.

```python
# ListCampaignsPaginator usage example

from types_aiobotocore_connectcampaigns.paginator import ListCampaignsPaginator

def get_list_campaigns_paginator() -> ListCampaignsPaginator:
    return client.get_paginator("list_campaigns"))
```

- [ListCampaignsPaginator](./paginators.md#listcampaignspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# CampaignStateType usage example

from types_aiobotocore_connectcampaigns.literals import CampaignStateType

def get_value() -> CampaignStateType:
    return "Failed"
```

- [CampaignStateType](./literals.md#campaignstatetype)
- [EncryptionTypeType](./literals.md#encryptiontypetype)
- [FailureCodeType](./literals.md#failurecodetype)
- [GetCampaignStateBatchFailureCodeType](./literals.md#getcampaignstatebatchfailurecodetype)
- [InstanceIdFilterOperatorType](./literals.md#instanceidfilteroperatortype)
- [InstanceOnboardingJobFailureCodeType](./literals.md#instanceonboardingjobfailurecodetype)
- [InstanceOnboardingJobStatusCodeType](./literals.md#instanceonboardingjobstatuscodetype)
- [ListCampaignsPaginatorName](./literals.md#listcampaignspaginatorname)
- [ConnectCampaignServiceServiceName](./literals.md#connectcampaignserviceservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AgentlessDialerConfigTypeDef](./type_defs.md#agentlessdialerconfigtypedef)
- [AnswerMachineDetectionConfigTypeDef](./type_defs.md#answermachinedetectionconfigtypedef)
- [InstanceIdFilterTypeDef](./type_defs.md#instanceidfiltertypedef)
- [CampaignSummaryTypeDef](./type_defs.md#campaignsummarytypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [DeleteCampaignRequestTypeDef](./type_defs.md#deletecampaignrequesttypedef)
- [DeleteConnectInstanceConfigRequestTypeDef](./type_defs.md#deleteconnectinstanceconfigrequesttypedef)
- [DeleteInstanceOnboardingJobRequestTypeDef](./type_defs.md#deleteinstanceonboardingjobrequesttypedef)
- [DescribeCampaignRequestTypeDef](./type_defs.md#describecampaignrequesttypedef)
- [TimestampTypeDef](./type_defs.md#timestamptypedef)
- [PredictiveDialerConfigTypeDef](./type_defs.md#predictivedialerconfigtypedef)
- [ProgressiveDialerConfigTypeDef](./type_defs.md#progressivedialerconfigtypedef)
- [EncryptionConfigTypeDef](./type_defs.md#encryptionconfigtypedef)
- [FailedCampaignStateResponseTypeDef](./type_defs.md#failedcampaignstateresponsetypedef)
- [FailedRequestTypeDef](./type_defs.md#failedrequesttypedef)
- [GetCampaignStateBatchRequestTypeDef](./type_defs.md#getcampaignstatebatchrequesttypedef)
- [SuccessfulCampaignStateResponseTypeDef](./type_defs.md#successfulcampaignstateresponsetypedef)
- [GetCampaignStateRequestTypeDef](./type_defs.md#getcampaignstaterequesttypedef)
- [GetConnectInstanceConfigRequestTypeDef](./type_defs.md#getconnectinstanceconfigrequesttypedef)
- [GetInstanceOnboardingJobStatusRequestTypeDef](./type_defs.md#getinstanceonboardingjobstatusrequesttypedef)
- [InstanceOnboardingJobStatusTypeDef](./type_defs.md#instanceonboardingjobstatustypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListTagsForResourceRequestTypeDef](./type_defs.md#listtagsforresourcerequesttypedef)
- [PauseCampaignRequestTypeDef](./type_defs.md#pausecampaignrequesttypedef)
- [SuccessfulRequestTypeDef](./type_defs.md#successfulrequesttypedef)
- [ResumeCampaignRequestTypeDef](./type_defs.md#resumecampaignrequesttypedef)
- [StartCampaignRequestTypeDef](./type_defs.md#startcampaignrequesttypedef)
- [StopCampaignRequestTypeDef](./type_defs.md#stopcampaignrequesttypedef)
- [TagResourceRequestTypeDef](./type_defs.md#tagresourcerequesttypedef)
- [UntagResourceRequestTypeDef](./type_defs.md#untagresourcerequesttypedef)
- [UpdateCampaignNameRequestTypeDef](./type_defs.md#updatecampaignnamerequesttypedef)
- [OutboundCallConfigTypeDef](./type_defs.md#outboundcallconfigtypedef)
- [UpdateCampaignOutboundCallConfigRequestTypeDef](./type_defs.md#updatecampaignoutboundcallconfigrequesttypedef)
- [CampaignFiltersTypeDef](./type_defs.md#campaignfilterstypedef)
- [CreateCampaignResponseTypeDef](./type_defs.md#createcampaignresponsetypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [GetCampaignStateResponseTypeDef](./type_defs.md#getcampaignstateresponsetypedef)
- [ListCampaignsResponseTypeDef](./type_defs.md#listcampaignsresponsetypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [DialRequestTypeDef](./type_defs.md#dialrequesttypedef)
- [DialerConfigTypeDef](./type_defs.md#dialerconfigtypedef)
- [InstanceConfigTypeDef](./type_defs.md#instanceconfigtypedef)
- [StartInstanceOnboardingJobRequestTypeDef](./type_defs.md#startinstanceonboardingjobrequesttypedef)
- [GetCampaignStateBatchResponseTypeDef](./type_defs.md#getcampaignstatebatchresponsetypedef)
- [GetInstanceOnboardingJobStatusResponseTypeDef](./type_defs.md#getinstanceonboardingjobstatusresponsetypedef)
- [StartInstanceOnboardingJobResponseTypeDef](./type_defs.md#startinstanceonboardingjobresponsetypedef)
- [PutDialRequestBatchResponseTypeDef](./type_defs.md#putdialrequestbatchresponsetypedef)
- [ListCampaignsRequestPaginateTypeDef](./type_defs.md#listcampaignsrequestpaginatetypedef)
- [ListCampaignsRequestTypeDef](./type_defs.md#listcampaignsrequesttypedef)
- [PutDialRequestBatchRequestTypeDef](./type_defs.md#putdialrequestbatchrequesttypedef)
- [CampaignTypeDef](./type_defs.md#campaigntypedef)
- [CreateCampaignRequestTypeDef](./type_defs.md#createcampaignrequesttypedef)
- [UpdateCampaignDialerConfigRequestTypeDef](./type_defs.md#updatecampaigndialerconfigrequesttypedef)
- [GetConnectInstanceConfigResponseTypeDef](./type_defs.md#getconnectinstanceconfigresponsetypedef)
- [DescribeCampaignResponseTypeDef](./type_defs.md#describecampaignresponsetypedef)

