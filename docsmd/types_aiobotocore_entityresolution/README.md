# EntityResolution module

> [Index](../README.md) > EntityResolution


!!! note ""

    Auto-generated documentation for [EntityResolution](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution)
    type annotations stubs module [types-aiobotocore-entityresolution](https://pypi.org/project/types-aiobotocore-entityresolution/).

## How to install



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
# ListMatchingJobsPaginator usage example

from types_aiobotocore_entityresolution.paginator import ListMatchingJobsPaginator

def get_list_matching_jobs_paginator() -> ListMatchingJobsPaginator:
    return client.get_paginator("list_matching_jobs"))
```

- [ListMatchingJobsPaginator](./paginators.md#listmatchingjobspaginator)
- [ListMatchingWorkflowsPaginator](./paginators.md#listmatchingworkflowspaginator)
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
- [IncrementalRunTypeType](./literals.md#incrementalruntypetype)
- [JobStatusType](./literals.md#jobstatustype)
- [ListMatchingJobsPaginatorName](./literals.md#listmatchingjobspaginatorname)
- [ListMatchingWorkflowsPaginatorName](./literals.md#listmatchingworkflowspaginatorname)
- [ListSchemaMappingsPaginatorName](./literals.md#listschemamappingspaginatorname)
- [ResolutionTypeType](./literals.md#resolutiontypetype)
- [SchemaAttributeTypeType](./literals.md#schemaattributetypetype)
- [EntityResolutionServiceName](./literals.md#entityresolutionservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [IncrementalRunConfigTypeDef](./type_defs.md#incrementalrunconfigtypedef)
- [InputSourceTypeDef](./type_defs.md#inputsourcetypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [SchemaInputAttributeTypeDef](./type_defs.md#schemainputattributetypedef)
- [DeleteMatchingWorkflowInputRequestTypeDef](./type_defs.md#deletematchingworkflowinputrequesttypedef)
- [DeleteSchemaMappingInputRequestTypeDef](./type_defs.md#deleteschemamappinginputrequesttypedef)
- [ErrorDetailsTypeDef](./type_defs.md#errordetailstypedef)
- [GetMatchIdInputRequestTypeDef](./type_defs.md#getmatchidinputrequesttypedef)
- [GetMatchingJobInputRequestTypeDef](./type_defs.md#getmatchingjobinputrequesttypedef)
- [JobMetricsTypeDef](./type_defs.md#jobmetricstypedef)
- [GetMatchingWorkflowInputRequestTypeDef](./type_defs.md#getmatchingworkflowinputrequesttypedef)
- [GetSchemaMappingInputRequestTypeDef](./type_defs.md#getschemamappinginputrequesttypedef)
- [JobSummaryTypeDef](./type_defs.md#jobsummarytypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListMatchingJobsInputRequestTypeDef](./type_defs.md#listmatchingjobsinputrequesttypedef)
- [ListMatchingWorkflowsInputRequestTypeDef](./type_defs.md#listmatchingworkflowsinputrequesttypedef)
- [MatchingWorkflowSummaryTypeDef](./type_defs.md#matchingworkflowsummarytypedef)
- [ListSchemaMappingsInputRequestTypeDef](./type_defs.md#listschemamappingsinputrequesttypedef)
- [SchemaMappingSummaryTypeDef](./type_defs.md#schemamappingsummarytypedef)
- [ListTagsForResourceInputRequestTypeDef](./type_defs.md#listtagsforresourceinputrequesttypedef)
- [OutputAttributeTypeDef](./type_defs.md#outputattributetypedef)
- [RuleTypeDef](./type_defs.md#ruletypedef)
- [StartMatchingJobInputRequestTypeDef](./type_defs.md#startmatchingjobinputrequesttypedef)
- [TagResourceInputRequestTypeDef](./type_defs.md#tagresourceinputrequesttypedef)
- [UntagResourceInputRequestTypeDef](./type_defs.md#untagresourceinputrequesttypedef)
- [DeleteMatchingWorkflowOutputTypeDef](./type_defs.md#deletematchingworkflowoutputtypedef)
- [DeleteSchemaMappingOutputTypeDef](./type_defs.md#deleteschemamappingoutputtypedef)
- [GetMatchIdOutputTypeDef](./type_defs.md#getmatchidoutputtypedef)
- [ListTagsForResourceOutputTypeDef](./type_defs.md#listtagsforresourceoutputtypedef)
- [StartMatchingJobOutputTypeDef](./type_defs.md#startmatchingjoboutputtypedef)
- [CreateSchemaMappingInputRequestTypeDef](./type_defs.md#createschemamappinginputrequesttypedef)
- [CreateSchemaMappingOutputTypeDef](./type_defs.md#createschemamappingoutputtypedef)
- [GetSchemaMappingOutputTypeDef](./type_defs.md#getschemamappingoutputtypedef)
- [GetMatchingJobOutputTypeDef](./type_defs.md#getmatchingjoboutputtypedef)
- [ListMatchingJobsOutputTypeDef](./type_defs.md#listmatchingjobsoutputtypedef)
- [ListMatchingJobsInputListMatchingJobsPaginateTypeDef](./type_defs.md#listmatchingjobsinputlistmatchingjobspaginatetypedef)
- [ListMatchingWorkflowsInputListMatchingWorkflowsPaginateTypeDef](./type_defs.md#listmatchingworkflowsinputlistmatchingworkflowspaginatetypedef)
- [ListSchemaMappingsInputListSchemaMappingsPaginateTypeDef](./type_defs.md#listschemamappingsinputlistschemamappingspaginatetypedef)
- [ListMatchingWorkflowsOutputTypeDef](./type_defs.md#listmatchingworkflowsoutputtypedef)
- [ListSchemaMappingsOutputTypeDef](./type_defs.md#listschemamappingsoutputtypedef)
- [OutputSourceTypeDef](./type_defs.md#outputsourcetypedef)
- [RuleBasedPropertiesTypeDef](./type_defs.md#rulebasedpropertiestypedef)
- [ResolutionTechniquesTypeDef](./type_defs.md#resolutiontechniquestypedef)
- [CreateMatchingWorkflowInputRequestTypeDef](./type_defs.md#creatematchingworkflowinputrequesttypedef)
- [CreateMatchingWorkflowOutputTypeDef](./type_defs.md#creatematchingworkflowoutputtypedef)
- [GetMatchingWorkflowOutputTypeDef](./type_defs.md#getmatchingworkflowoutputtypedef)
- [UpdateMatchingWorkflowInputRequestTypeDef](./type_defs.md#updatematchingworkflowinputrequesttypedef)
- [UpdateMatchingWorkflowOutputTypeDef](./type_defs.md#updatematchingworkflowoutputtypedef)

