# EntityResolution module

> [Index](../README.md) > EntityResolution


!!! note ""

    Auto-generated documentation for [EntityResolution](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#entityresolution)
    type annotations stubs module [types-aiobotocore-entityresolution](https://pypi.org/project/types-aiobotocore-entityresolution/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.19.0' mypy_boto3_builder`
1. Select `aiobotocore` AWS SDK.
1. Add `EntityResolution` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `EntityResolution` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[entityresolution]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[entityresolution]'

# standalone installation
python -m pip install types-aiobotocore-entityresolution
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-entityresolution
```

## Usage

Code samples can be found in [Examples](./usage.md).

## EntityResolutionClient

Type annotations and code completion for  `#!python session.create_client("entityresolution")` as [EntityResolutionClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Client)

```python
# EntityResolutionClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_entityresolution.client import EntityResolutionClient


session = get_session()
async with session.create_client("entityresolution") as client:
    client: EntityResolutionClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("entityresolution").get_paginator("...")`.

```python
# ListIdMappingJobsPaginator usage example

from types_aiobotocore_entityresolution.paginator import ListIdMappingJobsPaginator

def get_list_id_mapping_jobs_paginator() -> ListIdMappingJobsPaginator:
    return client.get_paginator("list_id_mapping_jobs"))
```

- [ListIdMappingJobsPaginator](./paginators.md#listidmappingjobspaginator)
- [ListIdMappingWorkflowsPaginator](./paginators.md#listidmappingworkflowspaginator)
- [ListIdNamespacesPaginator](./paginators.md#listidnamespacespaginator)
- [ListMatchingJobsPaginator](./paginators.md#listmatchingjobspaginator)
- [ListMatchingWorkflowsPaginator](./paginators.md#listmatchingworkflowspaginator)
- [ListProviderServicesPaginator](./paginators.md#listproviderservicespaginator)
- [ListSchemaMappingsPaginator](./paginators.md#listschemamappingspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# AttributeMatchingModelType usage example

from types_aiobotocore_entityresolution.literals import AttributeMatchingModelType

def get_value() -> AttributeMatchingModelType:
    return "MANY_TO_MANY"
```

- [AttributeMatchingModelType](./literals.md#attributematchingmodeltype)
- [DeleteUniqueIdErrorTypeType](./literals.md#deleteuniqueiderrortypetype)
- [DeleteUniqueIdStatusType](./literals.md#deleteuniqueidstatustype)
- [IdMappingTypeType](./literals.md#idmappingtypetype)
- [IdMappingWorkflowRuleDefinitionTypeType](./literals.md#idmappingworkflowruledefinitiontypetype)
- [IdNamespaceTypeType](./literals.md#idnamespacetypetype)
- [IncrementalRunTypeType](./literals.md#incrementalruntypetype)
- [JobStatusType](./literals.md#jobstatustype)
- [ListIdMappingJobsPaginatorName](./literals.md#listidmappingjobspaginatorname)
- [ListIdMappingWorkflowsPaginatorName](./literals.md#listidmappingworkflowspaginatorname)
- [ListIdNamespacesPaginatorName](./literals.md#listidnamespacespaginatorname)
- [ListMatchingJobsPaginatorName](./literals.md#listmatchingjobspaginatorname)
- [ListMatchingWorkflowsPaginatorName](./literals.md#listmatchingworkflowspaginatorname)
- [ListProviderServicesPaginatorName](./literals.md#listproviderservicespaginatorname)
- [ListSchemaMappingsPaginatorName](./literals.md#listschemamappingspaginatorname)
- [MatchPurposeType](./literals.md#matchpurposetype)
- [RecordMatchingModelType](./literals.md#recordmatchingmodeltype)
- [ResolutionTypeType](./literals.md#resolutiontypetype)
- [SchemaAttributeTypeType](./literals.md#schemaattributetypetype)
- [ServiceTypeType](./literals.md#servicetypetype)
- [StatementEffectType](./literals.md#statementeffecttype)
- [EntityResolutionServiceName](./literals.md#entityresolutionservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AddPolicyStatementInputRequestTypeDef](./type_defs.md#addpolicystatementinputrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [BatchDeleteUniqueIdInputRequestTypeDef](./type_defs.md#batchdeleteuniqueidinputrequesttypedef)
- [DeleteUniqueIdErrorTypeDef](./type_defs.md#deleteuniqueiderrortypedef)
- [DeletedUniqueIdTypeDef](./type_defs.md#deleteduniqueidtypedef)
- [IdMappingWorkflowInputSourceTypeDef](./type_defs.md#idmappingworkflowinputsourcetypedef)
- [IdMappingWorkflowOutputSourceTypeDef](./type_defs.md#idmappingworkflowoutputsourcetypedef)
- [IdNamespaceInputSourceTypeDef](./type_defs.md#idnamespaceinputsourcetypedef)
- [IncrementalRunConfigTypeDef](./type_defs.md#incrementalrunconfigtypedef)
- [InputSourceTypeDef](./type_defs.md#inputsourcetypedef)
- [SchemaInputAttributeTypeDef](./type_defs.md#schemainputattributetypedef)
- [DeleteIdMappingWorkflowInputRequestTypeDef](./type_defs.md#deleteidmappingworkflowinputrequesttypedef)
- [DeleteIdNamespaceInputRequestTypeDef](./type_defs.md#deleteidnamespaceinputrequesttypedef)
- [DeleteMatchingWorkflowInputRequestTypeDef](./type_defs.md#deletematchingworkflowinputrequesttypedef)
- [DeletePolicyStatementInputRequestTypeDef](./type_defs.md#deletepolicystatementinputrequesttypedef)
- [DeleteSchemaMappingInputRequestTypeDef](./type_defs.md#deleteschemamappinginputrequesttypedef)
- [ErrorDetailsTypeDef](./type_defs.md#errordetailstypedef)
- [GetIdMappingJobInputRequestTypeDef](./type_defs.md#getidmappingjobinputrequesttypedef)
- [IdMappingJobMetricsTypeDef](./type_defs.md#idmappingjobmetricstypedef)
- [IdMappingJobOutputSourceTypeDef](./type_defs.md#idmappingjoboutputsourcetypedef)
- [GetIdMappingWorkflowInputRequestTypeDef](./type_defs.md#getidmappingworkflowinputrequesttypedef)
- [GetIdNamespaceInputRequestTypeDef](./type_defs.md#getidnamespaceinputrequesttypedef)
- [GetMatchIdInputRequestTypeDef](./type_defs.md#getmatchidinputrequesttypedef)
- [GetMatchingJobInputRequestTypeDef](./type_defs.md#getmatchingjobinputrequesttypedef)
- [JobMetricsTypeDef](./type_defs.md#jobmetricstypedef)
- [JobOutputSourceTypeDef](./type_defs.md#joboutputsourcetypedef)
- [GetMatchingWorkflowInputRequestTypeDef](./type_defs.md#getmatchingworkflowinputrequesttypedef)
- [GetPolicyInputRequestTypeDef](./type_defs.md#getpolicyinputrequesttypedef)
- [GetProviderServiceInputRequestTypeDef](./type_defs.md#getproviderserviceinputrequesttypedef)
- [ProviderIdNameSpaceConfigurationTypeDef](./type_defs.md#provideridnamespaceconfigurationtypedef)
- [ProviderIntermediateDataAccessConfigurationTypeDef](./type_defs.md#providerintermediatedataaccessconfigurationtypedef)
- [GetSchemaMappingInputRequestTypeDef](./type_defs.md#getschemamappinginputrequesttypedef)
- [RuleOutputTypeDef](./type_defs.md#ruleoutputtypedef)
- [IdMappingWorkflowSummaryTypeDef](./type_defs.md#idmappingworkflowsummarytypedef)
- [IdNamespaceIdMappingWorkflowMetadataTypeDef](./type_defs.md#idnamespaceidmappingworkflowmetadatatypedef)
- [NamespaceProviderPropertiesOutputTypeDef](./type_defs.md#namespaceproviderpropertiesoutputtypedef)
- [IntermediateSourceConfigurationTypeDef](./type_defs.md#intermediatesourceconfigurationtypedef)
- [JobSummaryTypeDef](./type_defs.md#jobsummarytypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListIdMappingJobsInputRequestTypeDef](./type_defs.md#listidmappingjobsinputrequesttypedef)
- [ListIdMappingWorkflowsInputRequestTypeDef](./type_defs.md#listidmappingworkflowsinputrequesttypedef)
- [ListIdNamespacesInputRequestTypeDef](./type_defs.md#listidnamespacesinputrequesttypedef)
- [ListMatchingJobsInputRequestTypeDef](./type_defs.md#listmatchingjobsinputrequesttypedef)
- [ListMatchingWorkflowsInputRequestTypeDef](./type_defs.md#listmatchingworkflowsinputrequesttypedef)
- [MatchingWorkflowSummaryTypeDef](./type_defs.md#matchingworkflowsummarytypedef)
- [ListProviderServicesInputRequestTypeDef](./type_defs.md#listproviderservicesinputrequesttypedef)
- [ProviderServiceSummaryTypeDef](./type_defs.md#providerservicesummarytypedef)
- [ListSchemaMappingsInputRequestTypeDef](./type_defs.md#listschemamappingsinputrequesttypedef)
- [SchemaMappingSummaryTypeDef](./type_defs.md#schemamappingsummarytypedef)
- [ListTagsForResourceInputRequestTypeDef](./type_defs.md#listtagsforresourceinputrequesttypedef)
- [NamespaceProviderPropertiesTypeDef](./type_defs.md#namespaceproviderpropertiestypedef)
- [OutputAttributeTypeDef](./type_defs.md#outputattributetypedef)
- [ProviderSchemaAttributeTypeDef](./type_defs.md#providerschemaattributetypedef)
- [ProviderMarketplaceConfigurationTypeDef](./type_defs.md#providermarketplaceconfigurationtypedef)
- [PutPolicyInputRequestTypeDef](./type_defs.md#putpolicyinputrequesttypedef)
- [RuleTypeDef](./type_defs.md#ruletypedef)
- [StartMatchingJobInputRequestTypeDef](./type_defs.md#startmatchingjobinputrequesttypedef)
- [TagResourceInputRequestTypeDef](./type_defs.md#tagresourceinputrequesttypedef)
- [UntagResourceInputRequestTypeDef](./type_defs.md#untagresourceinputrequesttypedef)
- [AddPolicyStatementOutputTypeDef](./type_defs.md#addpolicystatementoutputtypedef)
- [DeleteIdMappingWorkflowOutputTypeDef](./type_defs.md#deleteidmappingworkflowoutputtypedef)
- [DeleteIdNamespaceOutputTypeDef](./type_defs.md#deleteidnamespaceoutputtypedef)
- [DeleteMatchingWorkflowOutputTypeDef](./type_defs.md#deletematchingworkflowoutputtypedef)
- [DeletePolicyStatementOutputTypeDef](./type_defs.md#deletepolicystatementoutputtypedef)
- [DeleteSchemaMappingOutputTypeDef](./type_defs.md#deleteschemamappingoutputtypedef)
- [GetMatchIdOutputTypeDef](./type_defs.md#getmatchidoutputtypedef)
- [GetPolicyOutputTypeDef](./type_defs.md#getpolicyoutputtypedef)
- [ListTagsForResourceOutputTypeDef](./type_defs.md#listtagsforresourceoutputtypedef)
- [PutPolicyOutputTypeDef](./type_defs.md#putpolicyoutputtypedef)
- [StartMatchingJobOutputTypeDef](./type_defs.md#startmatchingjoboutputtypedef)
- [BatchDeleteUniqueIdOutputTypeDef](./type_defs.md#batchdeleteuniqueidoutputtypedef)
- [CreateSchemaMappingInputRequestTypeDef](./type_defs.md#createschemamappinginputrequesttypedef)
- [CreateSchemaMappingOutputTypeDef](./type_defs.md#createschemamappingoutputtypedef)
- [GetSchemaMappingOutputTypeDef](./type_defs.md#getschemamappingoutputtypedef)
- [UpdateSchemaMappingInputRequestTypeDef](./type_defs.md#updateschemamappinginputrequesttypedef)
- [UpdateSchemaMappingOutputTypeDef](./type_defs.md#updateschemamappingoutputtypedef)
- [GetIdMappingJobOutputTypeDef](./type_defs.md#getidmappingjoboutputtypedef)
- [StartIdMappingJobInputRequestTypeDef](./type_defs.md#startidmappingjobinputrequesttypedef)
- [StartIdMappingJobOutputTypeDef](./type_defs.md#startidmappingjoboutputtypedef)
- [GetMatchingJobOutputTypeDef](./type_defs.md#getmatchingjoboutputtypedef)
- [IdMappingRuleBasedPropertiesOutputTypeDef](./type_defs.md#idmappingrulebasedpropertiesoutputtypedef)
- [NamespaceRuleBasedPropertiesOutputTypeDef](./type_defs.md#namespacerulebasedpropertiesoutputtypedef)
- [RuleBasedPropertiesOutputTypeDef](./type_defs.md#rulebasedpropertiesoutputtypedef)
- [ListIdMappingWorkflowsOutputTypeDef](./type_defs.md#listidmappingworkflowsoutputtypedef)
- [IdNamespaceSummaryTypeDef](./type_defs.md#idnamespacesummarytypedef)
- [ProviderPropertiesOutputTypeDef](./type_defs.md#providerpropertiesoutputtypedef)
- [ProviderPropertiesTypeDef](./type_defs.md#providerpropertiestypedef)
- [ListIdMappingJobsOutputTypeDef](./type_defs.md#listidmappingjobsoutputtypedef)
- [ListMatchingJobsOutputTypeDef](./type_defs.md#listmatchingjobsoutputtypedef)
- [ListIdMappingJobsInputPaginateTypeDef](./type_defs.md#listidmappingjobsinputpaginatetypedef)
- [ListIdMappingWorkflowsInputPaginateTypeDef](./type_defs.md#listidmappingworkflowsinputpaginatetypedef)
- [ListIdNamespacesInputPaginateTypeDef](./type_defs.md#listidnamespacesinputpaginatetypedef)
- [ListMatchingJobsInputPaginateTypeDef](./type_defs.md#listmatchingjobsinputpaginatetypedef)
- [ListMatchingWorkflowsInputPaginateTypeDef](./type_defs.md#listmatchingworkflowsinputpaginatetypedef)
- [ListProviderServicesInputPaginateTypeDef](./type_defs.md#listproviderservicesinputpaginatetypedef)
- [ListSchemaMappingsInputPaginateTypeDef](./type_defs.md#listschemamappingsinputpaginatetypedef)
- [ListMatchingWorkflowsOutputTypeDef](./type_defs.md#listmatchingworkflowsoutputtypedef)
- [ListProviderServicesOutputTypeDef](./type_defs.md#listproviderservicesoutputtypedef)
- [ListSchemaMappingsOutputTypeDef](./type_defs.md#listschemamappingsoutputtypedef)
- [NamespaceProviderPropertiesUnionTypeDef](./type_defs.md#namespaceproviderpropertiesuniontypedef)
- [OutputSourceOutputTypeDef](./type_defs.md#outputsourceoutputtypedef)
- [OutputSourceTypeDef](./type_defs.md#outputsourcetypedef)
- [ProviderComponentSchemaTypeDef](./type_defs.md#providercomponentschematypedef)
- [ProviderEndpointConfigurationTypeDef](./type_defs.md#providerendpointconfigurationtypedef)
- [RuleUnionTypeDef](./type_defs.md#ruleuniontypedef)
- [IdNamespaceIdMappingWorkflowPropertiesOutputTypeDef](./type_defs.md#idnamespaceidmappingworkflowpropertiesoutputtypedef)
- [ListIdNamespacesOutputTypeDef](./type_defs.md#listidnamespacesoutputtypedef)
- [IdMappingTechniquesOutputTypeDef](./type_defs.md#idmappingtechniquesoutputtypedef)
- [ResolutionTechniquesOutputTypeDef](./type_defs.md#resolutiontechniquesoutputtypedef)
- [ProviderPropertiesUnionTypeDef](./type_defs.md#providerpropertiesuniontypedef)
- [OutputSourceUnionTypeDef](./type_defs.md#outputsourceuniontypedef)
- [GetProviderServiceOutputTypeDef](./type_defs.md#getproviderserviceoutputtypedef)
- [IdMappingRuleBasedPropertiesTypeDef](./type_defs.md#idmappingrulebasedpropertiestypedef)
- [NamespaceRuleBasedPropertiesTypeDef](./type_defs.md#namespacerulebasedpropertiestypedef)
- [RuleBasedPropertiesTypeDef](./type_defs.md#rulebasedpropertiestypedef)
- [CreateIdNamespaceOutputTypeDef](./type_defs.md#createidnamespaceoutputtypedef)
- [GetIdNamespaceOutputTypeDef](./type_defs.md#getidnamespaceoutputtypedef)
- [UpdateIdNamespaceOutputTypeDef](./type_defs.md#updateidnamespaceoutputtypedef)
- [CreateIdMappingWorkflowOutputTypeDef](./type_defs.md#createidmappingworkflowoutputtypedef)
- [GetIdMappingWorkflowOutputTypeDef](./type_defs.md#getidmappingworkflowoutputtypedef)
- [UpdateIdMappingWorkflowOutputTypeDef](./type_defs.md#updateidmappingworkflowoutputtypedef)
- [CreateMatchingWorkflowOutputTypeDef](./type_defs.md#creatematchingworkflowoutputtypedef)
- [GetMatchingWorkflowOutputTypeDef](./type_defs.md#getmatchingworkflowoutputtypedef)
- [UpdateMatchingWorkflowOutputTypeDef](./type_defs.md#updatematchingworkflowoutputtypedef)
- [IdMappingRuleBasedPropertiesUnionTypeDef](./type_defs.md#idmappingrulebasedpropertiesuniontypedef)
- [NamespaceRuleBasedPropertiesUnionTypeDef](./type_defs.md#namespacerulebasedpropertiesuniontypedef)
- [RuleBasedPropertiesUnionTypeDef](./type_defs.md#rulebasedpropertiesuniontypedef)
- [IdMappingTechniquesTypeDef](./type_defs.md#idmappingtechniquestypedef)
- [IdNamespaceIdMappingWorkflowPropertiesTypeDef](./type_defs.md#idnamespaceidmappingworkflowpropertiestypedef)
- [ResolutionTechniquesTypeDef](./type_defs.md#resolutiontechniquestypedef)
- [CreateIdMappingWorkflowInputRequestTypeDef](./type_defs.md#createidmappingworkflowinputrequesttypedef)
- [UpdateIdMappingWorkflowInputRequestTypeDef](./type_defs.md#updateidmappingworkflowinputrequesttypedef)
- [IdNamespaceIdMappingWorkflowPropertiesUnionTypeDef](./type_defs.md#idnamespaceidmappingworkflowpropertiesuniontypedef)
- [UpdateIdNamespaceInputRequestTypeDef](./type_defs.md#updateidnamespaceinputrequesttypedef)
- [CreateMatchingWorkflowInputRequestTypeDef](./type_defs.md#creatematchingworkflowinputrequesttypedef)
- [UpdateMatchingWorkflowInputRequestTypeDef](./type_defs.md#updatematchingworkflowinputrequesttypedef)
- [CreateIdNamespaceInputRequestTypeDef](./type_defs.md#createidnamespaceinputrequesttypedef)

