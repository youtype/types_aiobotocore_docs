# B2BI module

> [Index](../README.md) > B2BI


!!! note ""

    Auto-generated documentation for [B2BI](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/b2bi.html#b2bi)
    type annotations stubs module [types-aiobotocore-b2bi](https://pypi.org/project/types-aiobotocore-b2bi/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.16.0' mypy_boto3_builder`
1. Select `aiobotocore` AWS SDK.
1. Add `B2BI` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `B2BI` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[b2bi]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[b2bi]'

# standalone installation
python -m pip install types-aiobotocore-b2bi
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-b2bi
```

## Usage

Code samples can be found in [Examples](./usage.md).

## B2BIClient

Type annotations and code completion for  `#!python session.create_client("b2bi")` as [B2BIClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/b2bi.html#B2BI.Client)

```python
# B2BIClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_b2bi.client import B2BIClient


session = get_session()
async with session.create_client("b2bi") as client:
    client: B2BIClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("b2bi").get_paginator("...")`.

```python
# ListCapabilitiesPaginator usage example

from types_aiobotocore_b2bi.paginator import ListCapabilitiesPaginator

def get_list_capabilities_paginator() -> ListCapabilitiesPaginator:
    return client.get_paginator("list_capabilities"))
```

- [ListCapabilitiesPaginator](./paginators.md#listcapabilitiespaginator)
- [ListPartnershipsPaginator](./paginators.md#listpartnershipspaginator)
- [ListProfilesPaginator](./paginators.md#listprofilespaginator)
- [ListTransformersPaginator](./paginators.md#listtransformerspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# CapabilityDirectionType usage example

from types_aiobotocore_b2bi.literals import CapabilityDirectionType

def get_value() -> CapabilityDirectionType:
    return "INBOUND"
```

- [CapabilityDirectionType](./literals.md#capabilitydirectiontype)
- [CapabilityTypeType](./literals.md#capabilitytypetype)
- [ConversionSourceFormatType](./literals.md#conversionsourceformattype)
- [ConversionTargetFormatType](./literals.md#conversiontargetformattype)
- [FileFormatType](./literals.md#fileformattype)
- [FromFormatType](./literals.md#fromformattype)
- [ListCapabilitiesPaginatorName](./literals.md#listcapabilitiespaginatorname)
- [ListPartnershipsPaginatorName](./literals.md#listpartnershipspaginatorname)
- [ListProfilesPaginatorName](./literals.md#listprofilespaginatorname)
- [ListTransformersPaginatorName](./literals.md#listtransformerspaginatorname)
- [LoggingType](./literals.md#loggingtype)
- [MappingTemplateLanguageType](./literals.md#mappingtemplatelanguagetype)
- [MappingTypeType](./literals.md#mappingtypetype)
- [ToFormatType](./literals.md#toformattype)
- [TransformerJobStatusType](./literals.md#transformerjobstatustype)
- [TransformerStatusType](./literals.md#transformerstatustype)
- [X12TransactionSetType](./literals.md#x12transactionsettype)
- [X12VersionType](./literals.md#x12versiontype)
- [B2BIServiceName](./literals.md#b2biservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [CapabilitySummaryTypeDef](./type_defs.md#capabilitysummarytypedef)
- [InputFileSourceTypeDef](./type_defs.md#inputfilesourcetypedef)
- [X12DetailsTypeDef](./type_defs.md#x12detailstypedef)
- [S3LocationTypeDef](./type_defs.md#s3locationtypedef)
- [TagTypeDef](./type_defs.md#tagtypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [MappingTypeDef](./type_defs.md#mappingtypedef)
- [DeleteCapabilityRequestRequestTypeDef](./type_defs.md#deletecapabilityrequestrequesttypedef)
- [DeletePartnershipRequestRequestTypeDef](./type_defs.md#deletepartnershiprequestrequesttypedef)
- [DeleteProfileRequestRequestTypeDef](./type_defs.md#deleteprofilerequestrequesttypedef)
- [DeleteTransformerRequestRequestTypeDef](./type_defs.md#deletetransformerrequestrequesttypedef)
- [GenerateMappingRequestRequestTypeDef](./type_defs.md#generatemappingrequestrequesttypedef)
- [GetCapabilityRequestRequestTypeDef](./type_defs.md#getcapabilityrequestrequesttypedef)
- [GetPartnershipRequestRequestTypeDef](./type_defs.md#getpartnershiprequestrequesttypedef)
- [GetProfileRequestRequestTypeDef](./type_defs.md#getprofilerequestrequesttypedef)
- [GetTransformerJobRequestRequestTypeDef](./type_defs.md#gettransformerjobrequestrequesttypedef)
- [GetTransformerRequestRequestTypeDef](./type_defs.md#gettransformerrequestrequesttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListCapabilitiesRequestRequestTypeDef](./type_defs.md#listcapabilitiesrequestrequesttypedef)
- [ListPartnershipsRequestRequestTypeDef](./type_defs.md#listpartnershipsrequestrequesttypedef)
- [ListProfilesRequestRequestTypeDef](./type_defs.md#listprofilesrequestrequesttypedef)
- [ProfileSummaryTypeDef](./type_defs.md#profilesummarytypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [ListTransformersRequestRequestTypeDef](./type_defs.md#listtransformersrequestrequesttypedef)
- [SampleDocumentKeysTypeDef](./type_defs.md#sampledocumentkeystypedef)
- [TestMappingRequestRequestTypeDef](./type_defs.md#testmappingrequestrequesttypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [UpdateProfileRequestRequestTypeDef](./type_defs.md#updateprofilerequestrequesttypedef)
- [X12DelimitersTypeDef](./type_defs.md#x12delimiterstypedef)
- [X12FunctionalGroupHeadersTypeDef](./type_defs.md#x12functionalgroupheaderstypedef)
- [X12InterchangeControlHeadersTypeDef](./type_defs.md#x12interchangecontrolheaderstypedef)
- [ConversionSourceTypeDef](./type_defs.md#conversionsourcetypedef)
- [ConversionTargetFormatDetailsTypeDef](./type_defs.md#conversiontargetformatdetailstypedef)
- [EdiTypeTypeDef](./type_defs.md#editypetypedef)
- [FormatOptionsTypeDef](./type_defs.md#formatoptionstypedef)
- [TemplateDetailsTypeDef](./type_defs.md#templatedetailstypedef)
- [OutputSampleFileSourceTypeDef](./type_defs.md#outputsamplefilesourcetypedef)
- [StartTransformerJobRequestRequestTypeDef](./type_defs.md#starttransformerjobrequestrequesttypedef)
- [CreateProfileRequestRequestTypeDef](./type_defs.md#createprofilerequestrequesttypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [CreateProfileResponseTypeDef](./type_defs.md#createprofileresponsetypedef)
- [CreateStarterMappingTemplateResponseTypeDef](./type_defs.md#createstartermappingtemplateresponsetypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [GenerateMappingResponseTypeDef](./type_defs.md#generatemappingresponsetypedef)
- [GetProfileResponseTypeDef](./type_defs.md#getprofileresponsetypedef)
- [GetTransformerJobResponseTypeDef](./type_defs.md#gettransformerjobresponsetypedef)
- [ListCapabilitiesResponseTypeDef](./type_defs.md#listcapabilitiesresponsetypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [StartTransformerJobResponseTypeDef](./type_defs.md#starttransformerjobresponsetypedef)
- [TestConversionResponseTypeDef](./type_defs.md#testconversionresponsetypedef)
- [TestMappingResponseTypeDef](./type_defs.md#testmappingresponsetypedef)
- [TestParsingResponseTypeDef](./type_defs.md#testparsingresponsetypedef)
- [UpdateProfileResponseTypeDef](./type_defs.md#updateprofileresponsetypedef)
- [ListCapabilitiesRequestListCapabilitiesPaginateTypeDef](./type_defs.md#listcapabilitiesrequestlistcapabilitiespaginatetypedef)
- [ListPartnershipsRequestListPartnershipsPaginateTypeDef](./type_defs.md#listpartnershipsrequestlistpartnershipspaginatetypedef)
- [ListProfilesRequestListProfilesPaginateTypeDef](./type_defs.md#listprofilesrequestlistprofilespaginatetypedef)
- [ListTransformersRequestListTransformersPaginateTypeDef](./type_defs.md#listtransformersrequestlisttransformerspaginatetypedef)
- [ListProfilesResponseTypeDef](./type_defs.md#listprofilesresponsetypedef)
- [SampleDocumentsOutputTypeDef](./type_defs.md#sampledocumentsoutputtypedef)
- [SampleDocumentsTypeDef](./type_defs.md#sampledocumentstypedef)
- [X12OutboundEdiHeadersTypeDef](./type_defs.md#x12outboundediheaderstypedef)
- [EdiConfigurationTypeDef](./type_defs.md#ediconfigurationtypedef)
- [TestParsingRequestRequestTypeDef](./type_defs.md#testparsingrequestrequesttypedef)
- [InputConversionTypeDef](./type_defs.md#inputconversiontypedef)
- [OutputConversionTypeDef](./type_defs.md#outputconversiontypedef)
- [CreateStarterMappingTemplateRequestRequestTypeDef](./type_defs.md#createstartermappingtemplaterequestrequesttypedef)
- [ConversionTargetTypeDef](./type_defs.md#conversiontargettypedef)
- [X12EnvelopeTypeDef](./type_defs.md#x12envelopetypedef)
- [CapabilityConfigurationTypeDef](./type_defs.md#capabilityconfigurationtypedef)
- [CreateTransformerRequestRequestTypeDef](./type_defs.md#createtransformerrequestrequesttypedef)
- [CreateTransformerResponseTypeDef](./type_defs.md#createtransformerresponsetypedef)
- [GetTransformerResponseTypeDef](./type_defs.md#gettransformerresponsetypedef)
- [TransformerSummaryTypeDef](./type_defs.md#transformersummarytypedef)
- [UpdateTransformerRequestRequestTypeDef](./type_defs.md#updatetransformerrequestrequesttypedef)
- [UpdateTransformerResponseTypeDef](./type_defs.md#updatetransformerresponsetypedef)
- [TestConversionRequestRequestTypeDef](./type_defs.md#testconversionrequestrequesttypedef)
- [OutboundEdiOptionsTypeDef](./type_defs.md#outboundedioptionstypedef)
- [CreateCapabilityRequestRequestTypeDef](./type_defs.md#createcapabilityrequestrequesttypedef)
- [CreateCapabilityResponseTypeDef](./type_defs.md#createcapabilityresponsetypedef)
- [GetCapabilityResponseTypeDef](./type_defs.md#getcapabilityresponsetypedef)
- [UpdateCapabilityRequestRequestTypeDef](./type_defs.md#updatecapabilityrequestrequesttypedef)
- [UpdateCapabilityResponseTypeDef](./type_defs.md#updatecapabilityresponsetypedef)
- [ListTransformersResponseTypeDef](./type_defs.md#listtransformersresponsetypedef)
- [CapabilityOptionsTypeDef](./type_defs.md#capabilityoptionstypedef)
- [CreatePartnershipRequestRequestTypeDef](./type_defs.md#createpartnershiprequestrequesttypedef)
- [CreatePartnershipResponseTypeDef](./type_defs.md#createpartnershipresponsetypedef)
- [GetPartnershipResponseTypeDef](./type_defs.md#getpartnershipresponsetypedef)
- [PartnershipSummaryTypeDef](./type_defs.md#partnershipsummarytypedef)
- [UpdatePartnershipRequestRequestTypeDef](./type_defs.md#updatepartnershiprequestrequesttypedef)
- [UpdatePartnershipResponseTypeDef](./type_defs.md#updatepartnershipresponsetypedef)
- [ListPartnershipsResponseTypeDef](./type_defs.md#listpartnershipsresponsetypedef)

