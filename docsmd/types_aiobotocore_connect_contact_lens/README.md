# ConnectContactLens module

> [Index](../README.md) > ConnectContactLens


!!! note ""

    Auto-generated documentation for [ConnectContactLens](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect-contact-lens.html#connectcontactlens)
    type annotations stubs module [types-aiobotocore-connect-contact-lens](https://pypi.org/project/types-aiobotocore-connect-contact-lens/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy-boto3-builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==3.1.1' mypy-boto3-builder`
1. Select `aiobotocore` AWS SDK.
1. Add `ConnectContactLens` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `ConnectContactLens` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[connect-contact-lens]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[connect-contact-lens]'

# standalone installation
python -m pip install types-aiobotocore-connect-contact-lens
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-connect-contact-lens
```

## Usage

Code samples can be found in [Examples](./usage.md).

## ConnectContactLensClient

Type annotations and code completion for  `#!python session.create_client("connect-contact-lens")` as [ConnectContactLensClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect-contact-lens.html#ConnectContactLens.Client)

```python
# ConnectContactLensClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_connect_contact_lens.client import ConnectContactLensClient


session = get_session()
async with session.create_client("connect-contact-lens") as client:
    client: ConnectContactLensClient
```








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# PostContactSummaryFailureCodeType usage example

from types_aiobotocore_connect_contact_lens.literals import PostContactSummaryFailureCodeType

def get_value() -> PostContactSummaryFailureCodeType:
    return "FAILED_SAFETY_GUIDELINES"
```

- [PostContactSummaryFailureCodeType](./literals.md#postcontactsummaryfailurecodetype)
- [PostContactSummaryStatusType](./literals.md#postcontactsummarystatustype)
- [SentimentValueType](./literals.md#sentimentvaluetype)
- [ConnectContactLensServiceName](./literals.md#connectcontactlensservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [PointOfInterestTypeDef](./type_defs.md#pointofinteresttypedef)
- [CharacterOffsetsTypeDef](./type_defs.md#characteroffsetstypedef)
- [ListRealtimeContactAnalysisSegmentsRequestTypeDef](./type_defs.md#listrealtimecontactanalysissegmentsrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [PostContactSummaryTypeDef](./type_defs.md#postcontactsummarytypedef)
- [CategoryDetailsTypeDef](./type_defs.md#categorydetailstypedef)
- [IssueDetectedTypeDef](./type_defs.md#issuedetectedtypedef)
- [CategoriesTypeDef](./type_defs.md#categoriestypedef)
- [TranscriptTypeDef](./type_defs.md#transcripttypedef)
- [RealtimeContactAnalysisSegmentTypeDef](./type_defs.md#realtimecontactanalysissegmenttypedef)
- [ListRealtimeContactAnalysisSegmentsResponseTypeDef](./type_defs.md#listrealtimecontactanalysissegmentsresponsetypedef)

