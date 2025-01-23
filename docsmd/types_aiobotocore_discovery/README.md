# ApplicationDiscoveryService module

> [Index](../README.md) > ApplicationDiscoveryService


!!! note ""

    Auto-generated documentation for [ApplicationDiscoveryService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#applicationdiscoveryservice)
    type annotations stubs module [types-aiobotocore-discovery](https://pypi.org/project/types-aiobotocore-discovery/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.19.0' mypy_boto3_builder`
1. Select `aiobotocore` AWS SDK.
1. Add `ApplicationDiscoveryService` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `ApplicationDiscoveryService` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[discovery]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[discovery]'

# standalone installation
python -m pip install types-aiobotocore-discovery
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-discovery
```

## Usage

Code samples can be found in [Examples](./usage.md).

## ApplicationDiscoveryServiceClient

Type annotations and code completion for  `#!python session.create_client("discovery")` as [ApplicationDiscoveryServiceClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService.Client)

```python
# ApplicationDiscoveryServiceClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_discovery.client import ApplicationDiscoveryServiceClient


session = get_session()
async with session.create_client("discovery") as client:
    client: ApplicationDiscoveryServiceClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("discovery").get_paginator("...")`.

```python
# DescribeAgentsPaginator usage example

from types_aiobotocore_discovery.paginator import DescribeAgentsPaginator

def get_describe_agents_paginator() -> DescribeAgentsPaginator:
    return client.get_paginator("describe_agents"))
```

- [DescribeAgentsPaginator](./paginators.md#describeagentspaginator)
- [DescribeContinuousExportsPaginator](./paginators.md#describecontinuousexportspaginator)
- [DescribeExportConfigurationsPaginator](./paginators.md#describeexportconfigurationspaginator)
- [DescribeExportTasksPaginator](./paginators.md#describeexporttaskspaginator)
- [DescribeImportTasksPaginator](./paginators.md#describeimporttaskspaginator)
- [DescribeTagsPaginator](./paginators.md#describetagspaginator)
- [ListConfigurationsPaginator](./paginators.md#listconfigurationspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# AgentStatusType usage example

from types_aiobotocore_discovery.literals import AgentStatusType

def get_value() -> AgentStatusType:
    return "BLACKLISTED"
```

- [AgentStatusType](./literals.md#agentstatustype)
- [BatchDeleteConfigurationTaskStatusType](./literals.md#batchdeleteconfigurationtaskstatustype)
- [BatchDeleteImportDataErrorCodeType](./literals.md#batchdeleteimportdataerrorcodetype)
- [ConfigurationItemTypeType](./literals.md#configurationitemtypetype)
- [ContinuousExportStatusType](./literals.md#continuousexportstatustype)
- [DataSourceType](./literals.md#datasourcetype)
- [DeleteAgentErrorCodeType](./literals.md#deleteagenterrorcodetype)
- [DeletionConfigurationItemTypeType](./literals.md#deletionconfigurationitemtypetype)
- [DescribeAgentsPaginatorName](./literals.md#describeagentspaginatorname)
- [DescribeContinuousExportsPaginatorName](./literals.md#describecontinuousexportspaginatorname)
- [DescribeExportConfigurationsPaginatorName](./literals.md#describeexportconfigurationspaginatorname)
- [DescribeExportTasksPaginatorName](./literals.md#describeexporttaskspaginatorname)
- [DescribeImportTasksPaginatorName](./literals.md#describeimporttaskspaginatorname)
- [DescribeTagsPaginatorName](./literals.md#describetagspaginatorname)
- [ExportDataFormatType](./literals.md#exportdataformattype)
- [ExportStatusType](./literals.md#exportstatustype)
- [FileClassificationType](./literals.md#fileclassificationtype)
- [ImportStatusType](./literals.md#importstatustype)
- [ImportTaskFilterNameType](./literals.md#importtaskfilternametype)
- [ListConfigurationsPaginatorName](./literals.md#listconfigurationspaginatorname)
- [OfferingClassType](./literals.md#offeringclasstype)
- [OrderStringType](./literals.md#orderstringtype)
- [PurchasingOptionType](./literals.md#purchasingoptiontype)
- [TenancyType](./literals.md#tenancytype)
- [TermLengthType](./literals.md#termlengthtype)
- [ApplicationDiscoveryServiceServiceName](./literals.md#applicationdiscoveryserviceservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AgentConfigurationStatusTypeDef](./type_defs.md#agentconfigurationstatustypedef)
- [AgentNetworkInfoTypeDef](./type_defs.md#agentnetworkinfotypedef)
- [AssociateConfigurationItemsToApplicationRequestRequestTypeDef](./type_defs.md#associateconfigurationitemstoapplicationrequestrequesttypedef)
- [BatchDeleteAgentErrorTypeDef](./type_defs.md#batchdeleteagenterrortypedef)
- [DeleteAgentTypeDef](./type_defs.md#deleteagenttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [DeletionWarningTypeDef](./type_defs.md#deletionwarningtypedef)
- [FailedConfigurationTypeDef](./type_defs.md#failedconfigurationtypedef)
- [BatchDeleteImportDataErrorTypeDef](./type_defs.md#batchdeleteimportdataerrortypedef)
- [BatchDeleteImportDataRequestRequestTypeDef](./type_defs.md#batchdeleteimportdatarequestrequesttypedef)
- [ConfigurationTagTypeDef](./type_defs.md#configurationtagtypedef)
- [ContinuousExportDescriptionTypeDef](./type_defs.md#continuousexportdescriptiontypedef)
- [CreateApplicationRequestRequestTypeDef](./type_defs.md#createapplicationrequestrequesttypedef)
- [TagTypeDef](./type_defs.md#tagtypedef)
- [CustomerAgentInfoTypeDef](./type_defs.md#customeragentinfotypedef)
- [CustomerAgentlessCollectorInfoTypeDef](./type_defs.md#customeragentlesscollectorinfotypedef)
- [CustomerConnectorInfoTypeDef](./type_defs.md#customerconnectorinfotypedef)
- [CustomerMeCollectorInfoTypeDef](./type_defs.md#customermecollectorinfotypedef)
- [DeleteApplicationsRequestRequestTypeDef](./type_defs.md#deleteapplicationsrequestrequesttypedef)
- [FilterTypeDef](./type_defs.md#filtertypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [DescribeBatchDeleteConfigurationTaskRequestRequestTypeDef](./type_defs.md#describebatchdeleteconfigurationtaskrequestrequesttypedef)
- [DescribeConfigurationsRequestRequestTypeDef](./type_defs.md#describeconfigurationsrequestrequesttypedef)
- [DescribeContinuousExportsRequestRequestTypeDef](./type_defs.md#describecontinuousexportsrequestrequesttypedef)
- [DescribeExportConfigurationsRequestRequestTypeDef](./type_defs.md#describeexportconfigurationsrequestrequesttypedef)
- [ExportInfoTypeDef](./type_defs.md#exportinfotypedef)
- [ExportFilterTypeDef](./type_defs.md#exportfiltertypedef)
- [ImportTaskFilterTypeDef](./type_defs.md#importtaskfiltertypedef)
- [ImportTaskTypeDef](./type_defs.md#importtasktypedef)
- [TagFilterTypeDef](./type_defs.md#tagfiltertypedef)
- [DisassociateConfigurationItemsFromApplicationRequestRequestTypeDef](./type_defs.md#disassociateconfigurationitemsfromapplicationrequestrequesttypedef)
- [ReservedInstanceOptionsTypeDef](./type_defs.md#reservedinstanceoptionstypedef)
- [UsageMetricBasisTypeDef](./type_defs.md#usagemetricbasistypedef)
- [OrderByElementTypeDef](./type_defs.md#orderbyelementtypedef)
- [ListServerNeighborsRequestRequestTypeDef](./type_defs.md#listserverneighborsrequestrequesttypedef)
- [NeighborConnectionDetailTypeDef](./type_defs.md#neighborconnectiondetailtypedef)
- [StartBatchDeleteConfigurationTaskRequestRequestTypeDef](./type_defs.md#startbatchdeleteconfigurationtaskrequestrequesttypedef)
- [StartDataCollectionByAgentIdsRequestRequestTypeDef](./type_defs.md#startdatacollectionbyagentidsrequestrequesttypedef)
- [TimestampTypeDef](./type_defs.md#timestamptypedef)
- [StartImportTaskRequestRequestTypeDef](./type_defs.md#startimporttaskrequestrequesttypedef)
- [StopContinuousExportRequestRequestTypeDef](./type_defs.md#stopcontinuousexportrequestrequesttypedef)
- [StopDataCollectionByAgentIdsRequestRequestTypeDef](./type_defs.md#stopdatacollectionbyagentidsrequestrequesttypedef)
- [UpdateApplicationRequestRequestTypeDef](./type_defs.md#updateapplicationrequestrequesttypedef)
- [AgentInfoTypeDef](./type_defs.md#agentinfotypedef)
- [BatchDeleteAgentsRequestRequestTypeDef](./type_defs.md#batchdeleteagentsrequestrequesttypedef)
- [BatchDeleteAgentsResponseTypeDef](./type_defs.md#batchdeleteagentsresponsetypedef)
- [CreateApplicationResponseTypeDef](./type_defs.md#createapplicationresponsetypedef)
- [DescribeConfigurationsResponseTypeDef](./type_defs.md#describeconfigurationsresponsetypedef)
- [ExportConfigurationsResponseTypeDef](./type_defs.md#exportconfigurationsresponsetypedef)
- [ListConfigurationsResponseTypeDef](./type_defs.md#listconfigurationsresponsetypedef)
- [StartBatchDeleteConfigurationTaskResponseTypeDef](./type_defs.md#startbatchdeleteconfigurationtaskresponsetypedef)
- [StartContinuousExportResponseTypeDef](./type_defs.md#startcontinuousexportresponsetypedef)
- [StartDataCollectionByAgentIdsResponseTypeDef](./type_defs.md#startdatacollectionbyagentidsresponsetypedef)
- [StartExportTaskResponseTypeDef](./type_defs.md#startexporttaskresponsetypedef)
- [StopContinuousExportResponseTypeDef](./type_defs.md#stopcontinuousexportresponsetypedef)
- [StopDataCollectionByAgentIdsResponseTypeDef](./type_defs.md#stopdatacollectionbyagentidsresponsetypedef)
- [BatchDeleteConfigurationTaskTypeDef](./type_defs.md#batchdeleteconfigurationtasktypedef)
- [BatchDeleteImportDataResponseTypeDef](./type_defs.md#batchdeleteimportdataresponsetypedef)
- [DescribeTagsResponseTypeDef](./type_defs.md#describetagsresponsetypedef)
- [DescribeContinuousExportsResponseTypeDef](./type_defs.md#describecontinuousexportsresponsetypedef)
- [CreateTagsRequestRequestTypeDef](./type_defs.md#createtagsrequestrequesttypedef)
- [DeleteTagsRequestRequestTypeDef](./type_defs.md#deletetagsrequestrequesttypedef)
- [GetDiscoverySummaryResponseTypeDef](./type_defs.md#getdiscoverysummaryresponsetypedef)
- [DescribeAgentsRequestRequestTypeDef](./type_defs.md#describeagentsrequestrequesttypedef)
- [DescribeAgentsRequestPaginateTypeDef](./type_defs.md#describeagentsrequestpaginatetypedef)
- [DescribeContinuousExportsRequestPaginateTypeDef](./type_defs.md#describecontinuousexportsrequestpaginatetypedef)
- [DescribeExportConfigurationsRequestPaginateTypeDef](./type_defs.md#describeexportconfigurationsrequestpaginatetypedef)
- [DescribeExportConfigurationsResponseTypeDef](./type_defs.md#describeexportconfigurationsresponsetypedef)
- [DescribeExportTasksResponseTypeDef](./type_defs.md#describeexporttasksresponsetypedef)
- [DescribeExportTasksRequestPaginateTypeDef](./type_defs.md#describeexporttasksrequestpaginatetypedef)
- [DescribeExportTasksRequestRequestTypeDef](./type_defs.md#describeexporttasksrequestrequesttypedef)
- [DescribeImportTasksRequestPaginateTypeDef](./type_defs.md#describeimporttasksrequestpaginatetypedef)
- [DescribeImportTasksRequestRequestTypeDef](./type_defs.md#describeimporttasksrequestrequesttypedef)
- [DescribeImportTasksResponseTypeDef](./type_defs.md#describeimporttasksresponsetypedef)
- [StartImportTaskResponseTypeDef](./type_defs.md#startimporttaskresponsetypedef)
- [DescribeTagsRequestPaginateTypeDef](./type_defs.md#describetagsrequestpaginatetypedef)
- [DescribeTagsRequestRequestTypeDef](./type_defs.md#describetagsrequestrequesttypedef)
- [Ec2RecommendationsExportPreferencesTypeDef](./type_defs.md#ec2recommendationsexportpreferencestypedef)
- [ListConfigurationsRequestPaginateTypeDef](./type_defs.md#listconfigurationsrequestpaginatetypedef)
- [ListConfigurationsRequestRequestTypeDef](./type_defs.md#listconfigurationsrequestrequesttypedef)
- [ListServerNeighborsResponseTypeDef](./type_defs.md#listserverneighborsresponsetypedef)
- [DescribeAgentsResponseTypeDef](./type_defs.md#describeagentsresponsetypedef)
- [DescribeBatchDeleteConfigurationTaskResponseTypeDef](./type_defs.md#describebatchdeleteconfigurationtaskresponsetypedef)
- [ExportPreferencesTypeDef](./type_defs.md#exportpreferencestypedef)
- [StartExportTaskRequestRequestTypeDef](./type_defs.md#startexporttaskrequestrequesttypedef)

