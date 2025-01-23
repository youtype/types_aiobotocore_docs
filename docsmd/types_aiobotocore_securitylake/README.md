# SecurityLake module

> [Index](../README.md) > SecurityLake


!!! note ""

    Auto-generated documentation for [SecurityLake](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#securitylake)
    type annotations stubs module [types-aiobotocore-securitylake](https://pypi.org/project/types-aiobotocore-securitylake/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.19.0' mypy_boto3_builder`
1. Select `aiobotocore` AWS SDK.
1. Add `SecurityLake` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `SecurityLake` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[securitylake]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[securitylake]'

# standalone installation
python -m pip install types-aiobotocore-securitylake
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-securitylake
```

## Usage

Code samples can be found in [Examples](./usage.md).

## SecurityLakeClient

Type annotations and code completion for  `#!python session.create_client("securitylake")` as [SecurityLakeClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake.Client)

```python
# SecurityLakeClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_securitylake.client import SecurityLakeClient


session = get_session()
async with session.create_client("securitylake") as client:
    client: SecurityLakeClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("securitylake").get_paginator("...")`.

```python
# GetDataLakeSourcesPaginator usage example

from types_aiobotocore_securitylake.paginator import GetDataLakeSourcesPaginator

def get_get_data_lake_sources_paginator() -> GetDataLakeSourcesPaginator:
    return client.get_paginator("get_data_lake_sources"))
```

- [GetDataLakeSourcesPaginator](./paginators.md#getdatalakesourcespaginator)
- [ListDataLakeExceptionsPaginator](./paginators.md#listdatalakeexceptionspaginator)
- [ListLogSourcesPaginator](./paginators.md#listlogsourcespaginator)
- [ListSubscribersPaginator](./paginators.md#listsubscriberspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# AccessTypeType usage example

from types_aiobotocore_securitylake.literals import AccessTypeType

def get_value() -> AccessTypeType:
    return "LAKEFORMATION"
```

- [AccessTypeType](./literals.md#accesstypetype)
- [AwsLogSourceNameType](./literals.md#awslogsourcenametype)
- [DataLakeStatusType](./literals.md#datalakestatustype)
- [GetDataLakeSourcesPaginatorName](./literals.md#getdatalakesourcespaginatorname)
- [HttpMethodType](./literals.md#httpmethodtype)
- [ListDataLakeExceptionsPaginatorName](./literals.md#listdatalakeexceptionspaginatorname)
- [ListLogSourcesPaginatorName](./literals.md#listlogsourcespaginatorname)
- [ListSubscribersPaginatorName](./literals.md#listsubscriberspaginatorname)
- [SourceCollectionStatusType](./literals.md#sourcecollectionstatustype)
- [SubscriberStatusType](./literals.md#subscriberstatustype)
- [SecurityLakeServiceName](./literals.md#securitylakeservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AwsIdentityTypeDef](./type_defs.md#awsidentitytypedef)
- [AwsLogSourceConfigurationTypeDef](./type_defs.md#awslogsourceconfigurationtypedef)
- [AwsLogSourceResourceTypeDef](./type_defs.md#awslogsourceresourcetypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [CreateDataLakeExceptionSubscriptionRequestRequestTypeDef](./type_defs.md#createdatalakeexceptionsubscriptionrequestrequesttypedef)
- [TagTypeDef](./type_defs.md#tagtypedef)
- [CustomLogSourceAttributesTypeDef](./type_defs.md#customlogsourceattributestypedef)
- [CustomLogSourceCrawlerConfigurationTypeDef](./type_defs.md#customlogsourcecrawlerconfigurationtypedef)
- [CustomLogSourceProviderTypeDef](./type_defs.md#customlogsourceprovidertypedef)
- [DataLakeEncryptionConfigurationTypeDef](./type_defs.md#datalakeencryptionconfigurationtypedef)
- [DataLakeExceptionTypeDef](./type_defs.md#datalakeexceptiontypedef)
- [DataLakeLifecycleExpirationTypeDef](./type_defs.md#datalakelifecycleexpirationtypedef)
- [DataLakeLifecycleTransitionTypeDef](./type_defs.md#datalakelifecycletransitiontypedef)
- [DataLakeReplicationConfigurationOutputTypeDef](./type_defs.md#datalakereplicationconfigurationoutputtypedef)
- [DataLakeReplicationConfigurationTypeDef](./type_defs.md#datalakereplicationconfigurationtypedef)
- [DataLakeSourceStatusTypeDef](./type_defs.md#datalakesourcestatustypedef)
- [DataLakeUpdateExceptionTypeDef](./type_defs.md#datalakeupdateexceptiontypedef)
- [DeleteCustomLogSourceRequestRequestTypeDef](./type_defs.md#deletecustomlogsourcerequestrequesttypedef)
- [DeleteDataLakeRequestRequestTypeDef](./type_defs.md#deletedatalakerequestrequesttypedef)
- [DeleteSubscriberNotificationRequestRequestTypeDef](./type_defs.md#deletesubscribernotificationrequestrequesttypedef)
- [DeleteSubscriberRequestRequestTypeDef](./type_defs.md#deletesubscriberrequestrequesttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [GetDataLakeSourcesRequestRequestTypeDef](./type_defs.md#getdatalakesourcesrequestrequesttypedef)
- [GetSubscriberRequestRequestTypeDef](./type_defs.md#getsubscriberrequestrequesttypedef)
- [HttpsNotificationConfigurationTypeDef](./type_defs.md#httpsnotificationconfigurationtypedef)
- [ListDataLakeExceptionsRequestRequestTypeDef](./type_defs.md#listdatalakeexceptionsrequestrequesttypedef)
- [ListDataLakesRequestRequestTypeDef](./type_defs.md#listdatalakesrequestrequesttypedef)
- [ListSubscribersRequestRequestTypeDef](./type_defs.md#listsubscribersrequestrequesttypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [RegisterDataLakeDelegatedAdministratorRequestRequestTypeDef](./type_defs.md#registerdatalakedelegatedadministratorrequestrequesttypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [UpdateDataLakeExceptionSubscriptionRequestRequestTypeDef](./type_defs.md#updatedatalakeexceptionsubscriptionrequestrequesttypedef)
- [CreateAwsLogSourceRequestRequestTypeDef](./type_defs.md#createawslogsourcerequestrequesttypedef)
- [DeleteAwsLogSourceRequestRequestTypeDef](./type_defs.md#deleteawslogsourcerequestrequesttypedef)
- [DataLakeAutoEnableNewAccountConfigurationOutputTypeDef](./type_defs.md#datalakeautoenablenewaccountconfigurationoutputtypedef)
- [DataLakeAutoEnableNewAccountConfigurationTypeDef](./type_defs.md#datalakeautoenablenewaccountconfigurationtypedef)
- [CreateAwsLogSourceResponseTypeDef](./type_defs.md#createawslogsourceresponsetypedef)
- [CreateSubscriberNotificationResponseTypeDef](./type_defs.md#createsubscribernotificationresponsetypedef)
- [DeleteAwsLogSourceResponseTypeDef](./type_defs.md#deleteawslogsourceresponsetypedef)
- [GetDataLakeExceptionSubscriptionResponseTypeDef](./type_defs.md#getdatalakeexceptionsubscriptionresponsetypedef)
- [UpdateSubscriberNotificationResponseTypeDef](./type_defs.md#updatesubscribernotificationresponsetypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [CustomLogSourceConfigurationTypeDef](./type_defs.md#customlogsourceconfigurationtypedef)
- [CustomLogSourceResourceTypeDef](./type_defs.md#customlogsourceresourcetypedef)
- [ListDataLakeExceptionsResponseTypeDef](./type_defs.md#listdatalakeexceptionsresponsetypedef)
- [DataLakeLifecycleConfigurationOutputTypeDef](./type_defs.md#datalakelifecycleconfigurationoutputtypedef)
- [DataLakeLifecycleConfigurationTypeDef](./type_defs.md#datalakelifecycleconfigurationtypedef)
- [DataLakeReplicationConfigurationUnionTypeDef](./type_defs.md#datalakereplicationconfigurationuniontypedef)
- [DataLakeSourceTypeDef](./type_defs.md#datalakesourcetypedef)
- [DataLakeUpdateStatusTypeDef](./type_defs.md#datalakeupdatestatustypedef)
- [GetDataLakeSourcesRequestPaginateTypeDef](./type_defs.md#getdatalakesourcesrequestpaginatetypedef)
- [ListDataLakeExceptionsRequestPaginateTypeDef](./type_defs.md#listdatalakeexceptionsrequestpaginatetypedef)
- [ListSubscribersRequestPaginateTypeDef](./type_defs.md#listsubscribersrequestpaginatetypedef)
- [NotificationConfigurationTypeDef](./type_defs.md#notificationconfigurationtypedef)
- [GetDataLakeOrganizationConfigurationResponseTypeDef](./type_defs.md#getdatalakeorganizationconfigurationresponsetypedef)
- [DataLakeAutoEnableNewAccountConfigurationUnionTypeDef](./type_defs.md#datalakeautoenablenewaccountconfigurationuniontypedef)
- [DeleteDataLakeOrganizationConfigurationRequestRequestTypeDef](./type_defs.md#deletedatalakeorganizationconfigurationrequestrequesttypedef)
- [CreateCustomLogSourceRequestRequestTypeDef](./type_defs.md#createcustomlogsourcerequestrequesttypedef)
- [CreateCustomLogSourceResponseTypeDef](./type_defs.md#createcustomlogsourceresponsetypedef)
- [LogSourceResourceTypeDef](./type_defs.md#logsourceresourcetypedef)
- [DataLakeLifecycleConfigurationUnionTypeDef](./type_defs.md#datalakelifecycleconfigurationuniontypedef)
- [GetDataLakeSourcesResponseTypeDef](./type_defs.md#getdatalakesourcesresponsetypedef)
- [DataLakeResourceTypeDef](./type_defs.md#datalakeresourcetypedef)
- [CreateSubscriberNotificationRequestRequestTypeDef](./type_defs.md#createsubscribernotificationrequestrequesttypedef)
- [UpdateSubscriberNotificationRequestRequestTypeDef](./type_defs.md#updatesubscribernotificationrequestrequesttypedef)
- [CreateDataLakeOrganizationConfigurationRequestRequestTypeDef](./type_defs.md#createdatalakeorganizationconfigurationrequestrequesttypedef)
- [CreateSubscriberRequestRequestTypeDef](./type_defs.md#createsubscriberrequestrequesttypedef)
- [ListLogSourcesRequestPaginateTypeDef](./type_defs.md#listlogsourcesrequestpaginatetypedef)
- [ListLogSourcesRequestRequestTypeDef](./type_defs.md#listlogsourcesrequestrequesttypedef)
- [LogSourceTypeDef](./type_defs.md#logsourcetypedef)
- [SubscriberResourceTypeDef](./type_defs.md#subscriberresourcetypedef)
- [UpdateSubscriberRequestRequestTypeDef](./type_defs.md#updatesubscriberrequestrequesttypedef)
- [DataLakeConfigurationTypeDef](./type_defs.md#datalakeconfigurationtypedef)
- [CreateDataLakeResponseTypeDef](./type_defs.md#createdatalakeresponsetypedef)
- [ListDataLakesResponseTypeDef](./type_defs.md#listdatalakesresponsetypedef)
- [UpdateDataLakeResponseTypeDef](./type_defs.md#updatedatalakeresponsetypedef)
- [ListLogSourcesResponseTypeDef](./type_defs.md#listlogsourcesresponsetypedef)
- [CreateSubscriberResponseTypeDef](./type_defs.md#createsubscriberresponsetypedef)
- [GetSubscriberResponseTypeDef](./type_defs.md#getsubscriberresponsetypedef)
- [ListSubscribersResponseTypeDef](./type_defs.md#listsubscribersresponsetypedef)
- [UpdateSubscriberResponseTypeDef](./type_defs.md#updatesubscriberresponsetypedef)
- [CreateDataLakeRequestRequestTypeDef](./type_defs.md#createdatalakerequestrequesttypedef)
- [UpdateDataLakeRequestRequestTypeDef](./type_defs.md#updatedatalakerequestrequesttypedef)

