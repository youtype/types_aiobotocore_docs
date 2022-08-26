# ServiceQuotas module

> [Index](../README.md) > ServiceQuotas


!!! note ""

    Auto-generated documentation for [ServiceQuotas](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas)
    type annotations stubs module [types-aiobotocore-service-quotas](https://pypi.org/project/types-aiobotocore-service-quotas/).

## How to install



### From PyPI with pip

Install `types-aiobotocore` for `ServiceQuotas` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[service-quotas]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[service-quotas]'


# standalone installation
python -m pip install types-aiobotocore-service-quotas
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-service-quotas
```

## Usage

Code samples can be found in [Examples](./usage.md).

## ServiceQuotasClient

Type annotations and code completion for  `#!python session.create_client("service-quotas")` as [ServiceQuotasClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas.Client)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_service_quotas.client import ServiceQuotasClient


session = get_session()
async with session.create_client("service-quotas") as client:
    client: ServiceQuotasClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("service-quotas").get_paginator("...")`.

```python title="Usage example"
from types_aiobotocore_service_quotas.paginator import ListAWSDefaultServiceQuotasPaginator

def get_list_aws_default_service_quotas_paginator() -> ListAWSDefaultServiceQuotasPaginator:
    return client.get_paginator("list_aws_default_service_quotas"))
```

- [ListAWSDefaultServiceQuotasPaginator](./paginators.md#listawsdefaultservicequotaspaginator)
- [ListRequestedServiceQuotaChangeHistoryPaginator](./paginators.md#listrequestedservicequotachangehistorypaginator)
- [ListRequestedServiceQuotaChangeHistoryByQuotaPaginator](./paginators.md#listrequestedservicequotachangehistorybyquotapaginator)
- [ListServiceQuotaIncreaseRequestsInTemplatePaginator](./paginators.md#listservicequotaincreaserequestsintemplatepaginator)
- [ListServiceQuotasPaginator](./paginators.md#listservicequotaspaginator)
- [ListServicesPaginator](./paginators.md#listservicespaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_service_quotas.literals import ErrorCodeType

def get_value() -> ErrorCodeType:
    return "DEPENDENCY_ACCESS_DENIED_ERROR"
```

- [ErrorCodeType](./literals.md#errorcodetype)
- [ListAWSDefaultServiceQuotasPaginatorName](./literals.md#listawsdefaultservicequotaspaginatorname)
- [ListRequestedServiceQuotaChangeHistoryByQuotaPaginatorName](./literals.md#listrequestedservicequotachangehistorybyquotapaginatorname)
- [ListRequestedServiceQuotaChangeHistoryPaginatorName](./literals.md#listrequestedservicequotachangehistorypaginatorname)
- [ListServiceQuotaIncreaseRequestsInTemplatePaginatorName](./literals.md#listservicequotaincreaserequestsintemplatepaginatorname)
- [ListServiceQuotasPaginatorName](./literals.md#listservicequotaspaginatorname)
- [ListServicesPaginatorName](./literals.md#listservicespaginatorname)
- [PeriodUnitType](./literals.md#periodunittype)
- [RequestStatusType](./literals.md#requeststatustype)
- [ServiceQuotaTemplateAssociationStatusType](./literals.md#servicequotatemplateassociationstatustype)
- [ServiceQuotasServiceName](./literals.md#servicequotasservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Typed dictionaries

Type annotations for [typed dictionaries](./type_defs.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_service_quotas.type_defs import DeleteServiceQuotaIncreaseRequestFromTemplateRequestRequestTypeDef

def get_value() -> DeleteServiceQuotaIncreaseRequestFromTemplateRequestRequestTypeDef:
    return {
        "ServiceCode": ...,
        "QuotaCode": ...,
        "AwsRegion": ...,
    }
```

- [DeleteServiceQuotaIncreaseRequestFromTemplateRequestRequestTypeDef](./type_defs.md#deleteservicequotaincreaserequestfromtemplaterequestrequesttypedef)
- [ErrorReasonTypeDef](./type_defs.md#errorreasontypedef)
- [GetAWSDefaultServiceQuotaRequestRequestTypeDef](./type_defs.md#getawsdefaultservicequotarequestrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [GetRequestedServiceQuotaChangeRequestRequestTypeDef](./type_defs.md#getrequestedservicequotachangerequestrequesttypedef)
- [RequestedServiceQuotaChangeTypeDef](./type_defs.md#requestedservicequotachangetypedef)
- [GetServiceQuotaIncreaseRequestFromTemplateRequestRequestTypeDef](./type_defs.md#getservicequotaincreaserequestfromtemplaterequestrequesttypedef)
- [ServiceQuotaIncreaseRequestInTemplateTypeDef](./type_defs.md#servicequotaincreaserequestintemplatetypedef)
- [GetServiceQuotaRequestRequestTypeDef](./type_defs.md#getservicequotarequestrequesttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListAWSDefaultServiceQuotasRequestRequestTypeDef](./type_defs.md#listawsdefaultservicequotasrequestrequesttypedef)
- [ListRequestedServiceQuotaChangeHistoryByQuotaRequestRequestTypeDef](./type_defs.md#listrequestedservicequotachangehistorybyquotarequestrequesttypedef)
- [ListRequestedServiceQuotaChangeHistoryRequestRequestTypeDef](./type_defs.md#listrequestedservicequotachangehistoryrequestrequesttypedef)
- [ListServiceQuotaIncreaseRequestsInTemplateRequestRequestTypeDef](./type_defs.md#listservicequotaincreaserequestsintemplaterequestrequesttypedef)
- [ListServiceQuotasRequestRequestTypeDef](./type_defs.md#listservicequotasrequestrequesttypedef)
- [ListServicesRequestRequestTypeDef](./type_defs.md#listservicesrequestrequesttypedef)
- [ServiceInfoTypeDef](./type_defs.md#serviceinfotypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [TagTypeDef](./type_defs.md#tagtypedef)
- [MetricInfoTypeDef](./type_defs.md#metricinfotypedef)
- [PutServiceQuotaIncreaseRequestIntoTemplateRequestRequestTypeDef](./type_defs.md#putservicequotaincreaserequestintotemplaterequestrequesttypedef)
- [QuotaPeriodTypeDef](./type_defs.md#quotaperiodtypedef)
- [RequestServiceQuotaIncreaseRequestRequestTypeDef](./type_defs.md#requestservicequotaincreaserequestrequesttypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [GetAssociationForServiceQuotaTemplateResponseTypeDef](./type_defs.md#getassociationforservicequotatemplateresponsetypedef)
- [GetRequestedServiceQuotaChangeResponseTypeDef](./type_defs.md#getrequestedservicequotachangeresponsetypedef)
- [ListRequestedServiceQuotaChangeHistoryByQuotaResponseTypeDef](./type_defs.md#listrequestedservicequotachangehistorybyquotaresponsetypedef)
- [ListRequestedServiceQuotaChangeHistoryResponseTypeDef](./type_defs.md#listrequestedservicequotachangehistoryresponsetypedef)
- [RequestServiceQuotaIncreaseResponseTypeDef](./type_defs.md#requestservicequotaincreaseresponsetypedef)
- [GetServiceQuotaIncreaseRequestFromTemplateResponseTypeDef](./type_defs.md#getservicequotaincreaserequestfromtemplateresponsetypedef)
- [ListServiceQuotaIncreaseRequestsInTemplateResponseTypeDef](./type_defs.md#listservicequotaincreaserequestsintemplateresponsetypedef)
- [PutServiceQuotaIncreaseRequestIntoTemplateResponseTypeDef](./type_defs.md#putservicequotaincreaserequestintotemplateresponsetypedef)
- [ListAWSDefaultServiceQuotasRequestListAWSDefaultServiceQuotasPaginateTypeDef](./type_defs.md#listawsdefaultservicequotasrequestlistawsdefaultservicequotaspaginatetypedef)
- [ListRequestedServiceQuotaChangeHistoryByQuotaRequestListRequestedServiceQuotaChangeHistoryByQuotaPaginateTypeDef](./type_defs.md#listrequestedservicequotachangehistorybyquotarequestlistrequestedservicequotachangehistorybyquotapaginatetypedef)
- [ListRequestedServiceQuotaChangeHistoryRequestListRequestedServiceQuotaChangeHistoryPaginateTypeDef](./type_defs.md#listrequestedservicequotachangehistoryrequestlistrequestedservicequotachangehistorypaginatetypedef)
- [ListServiceQuotaIncreaseRequestsInTemplateRequestListServiceQuotaIncreaseRequestsInTemplatePaginateTypeDef](./type_defs.md#listservicequotaincreaserequestsintemplaterequestlistservicequotaincreaserequestsintemplatepaginatetypedef)
- [ListServiceQuotasRequestListServiceQuotasPaginateTypeDef](./type_defs.md#listservicequotasrequestlistservicequotaspaginatetypedef)
- [ListServicesRequestListServicesPaginateTypeDef](./type_defs.md#listservicesrequestlistservicespaginatetypedef)
- [ListServicesResponseTypeDef](./type_defs.md#listservicesresponsetypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [ServiceQuotaTypeDef](./type_defs.md#servicequotatypedef)
- [GetAWSDefaultServiceQuotaResponseTypeDef](./type_defs.md#getawsdefaultservicequotaresponsetypedef)
- [GetServiceQuotaResponseTypeDef](./type_defs.md#getservicequotaresponsetypedef)
- [ListAWSDefaultServiceQuotasResponseTypeDef](./type_defs.md#listawsdefaultservicequotasresponsetypedef)
- [ListServiceQuotasResponseTypeDef](./type_defs.md#listservicequotasresponsetypedef)

