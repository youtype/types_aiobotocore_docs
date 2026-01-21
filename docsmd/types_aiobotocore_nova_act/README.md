# NovaActService module

> [Index](../README.md) > NovaActService


!!! note ""

    Auto-generated documentation for [NovaActService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nova-act.html#novaactservice)
    type annotations stubs module [types-aiobotocore-nova-act](https://pypi.org/project/types-aiobotocore-nova-act/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy-boto3-builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==3.1.1' mypy-boto3-builder`
1. Select `aiobotocore` AWS SDK.
1. Add `NovaActService` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `NovaActService` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[nova-act]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[nova-act]'

# standalone installation
python -m pip install types-aiobotocore-nova-act
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-nova-act
```

## Usage

Code samples can be found in [Examples](./usage.md).

## NovaActServiceClient

Type annotations and code completion for  `#!python session.create_client("nova-act")` as [NovaActServiceClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nova-act.html#NovaActService.Client)

```python
# NovaActServiceClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_nova_act.client import NovaActServiceClient


session = get_session()
async with session.create_client("nova-act") as client:
    client: NovaActServiceClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("nova-act").get_paginator("...")`.

```python
# ListActsPaginator usage example

from types_aiobotocore_nova_act.paginator import ListActsPaginator

def get_list_acts_paginator() -> ListActsPaginator:
    return client.get_paginator("list_acts"))
```

- [ListActsPaginator](./paginators.md#listactspaginator)
- [ListSessionsPaginator](./paginators.md#listsessionspaginator)
- [ListWorkflowDefinitionsPaginator](./paginators.md#listworkflowdefinitionspaginator)
- [ListWorkflowRunsPaginator](./paginators.md#listworkflowrunspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# ActStatusType usage example

from types_aiobotocore_nova_act.literals import ActStatusType

def get_value() -> ActStatusType:
    return "FAILED"
```

- [ActStatusType](./literals.md#actstatustype)
- [ListActsPaginatorName](./literals.md#listactspaginatorname)
- [ListSessionsPaginatorName](./literals.md#listsessionspaginatorname)
- [ListWorkflowDefinitionsPaginatorName](./literals.md#listworkflowdefinitionspaginatorname)
- [ListWorkflowRunsPaginatorName](./literals.md#listworkflowrunspaginatorname)
- [ModelStatusType](./literals.md#modelstatustype)
- [SortOrderType](./literals.md#sortordertype)
- [TraceLocationTypeType](./literals.md#tracelocationtypetype)
- [WorkflowDefinitionStatusType](./literals.md#workflowdefinitionstatustype)
- [WorkflowRunStatusType](./literals.md#workflowrunstatustype)
- [NovaActServiceServiceName](./literals.md#novaactserviceservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [ActErrorTypeDef](./type_defs.md#acterrortypedef)
- [TraceLocationTypeDef](./type_defs.md#tracelocationtypedef)
- [CallResultContentTypeDef](./type_defs.md#callresultcontenttypedef)
- [CallTypeDef](./type_defs.md#calltypedef)
- [ClientInfoTypeDef](./type_defs.md#clientinfotypedef)
- [CompatibilityInformationTypeDef](./type_defs.md#compatibilityinformationtypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [CreateSessionRequestTypeDef](./type_defs.md#createsessionrequesttypedef)
- [WorkflowExportConfigTypeDef](./type_defs.md#workflowexportconfigtypedef)
- [DeleteWorkflowDefinitionRequestTypeDef](./type_defs.md#deleteworkflowdefinitionrequesttypedef)
- [DeleteWorkflowRunRequestTypeDef](./type_defs.md#deleteworkflowrunrequesttypedef)
- [GetWorkflowDefinitionRequestTypeDef](./type_defs.md#getworkflowdefinitionrequesttypedef)
- [GetWorkflowRunRequestTypeDef](./type_defs.md#getworkflowrunrequesttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListActsRequestTypeDef](./type_defs.md#listactsrequesttypedef)
- [ListModelsRequestTypeDef](./type_defs.md#listmodelsrequesttypedef)
- [ModelAliasTypeDef](./type_defs.md#modelaliastypedef)
- [ListSessionsRequestTypeDef](./type_defs.md#listsessionsrequesttypedef)
- [SessionSummaryTypeDef](./type_defs.md#sessionsummarytypedef)
- [ListWorkflowDefinitionsRequestTypeDef](./type_defs.md#listworkflowdefinitionsrequesttypedef)
- [WorkflowDefinitionSummaryTypeDef](./type_defs.md#workflowdefinitionsummarytypedef)
- [ListWorkflowRunsRequestTypeDef](./type_defs.md#listworkflowrunsrequesttypedef)
- [ModelLifecycleTypeDef](./type_defs.md#modellifecycletypedef)
- [ToolInputSchemaTypeDef](./type_defs.md#toolinputschematypedef)
- [UpdateWorkflowRunRequestTypeDef](./type_defs.md#updateworkflowrunrequesttypedef)
- [UpdateActRequestTypeDef](./type_defs.md#updateactrequesttypedef)
- [ActSummaryTypeDef](./type_defs.md#actsummarytypedef)
- [WorkflowRunSummaryTypeDef](./type_defs.md#workflowrunsummarytypedef)
- [CallResultTypeDef](./type_defs.md#callresulttypedef)
- [CreateWorkflowRunRequestTypeDef](./type_defs.md#createworkflowrunrequesttypedef)
- [CreateActResponseTypeDef](./type_defs.md#createactresponsetypedef)
- [CreateSessionResponseTypeDef](./type_defs.md#createsessionresponsetypedef)
- [CreateWorkflowDefinitionResponseTypeDef](./type_defs.md#createworkflowdefinitionresponsetypedef)
- [CreateWorkflowRunResponseTypeDef](./type_defs.md#createworkflowrunresponsetypedef)
- [DeleteWorkflowDefinitionResponseTypeDef](./type_defs.md#deleteworkflowdefinitionresponsetypedef)
- [DeleteWorkflowRunResponseTypeDef](./type_defs.md#deleteworkflowrunresponsetypedef)
- [GetWorkflowRunResponseTypeDef](./type_defs.md#getworkflowrunresponsetypedef)
- [InvokeActStepResponseTypeDef](./type_defs.md#invokeactstepresponsetypedef)
- [CreateWorkflowDefinitionRequestTypeDef](./type_defs.md#createworkflowdefinitionrequesttypedef)
- [GetWorkflowDefinitionResponseTypeDef](./type_defs.md#getworkflowdefinitionresponsetypedef)
- [ListActsRequestPaginateTypeDef](./type_defs.md#listactsrequestpaginatetypedef)
- [ListSessionsRequestPaginateTypeDef](./type_defs.md#listsessionsrequestpaginatetypedef)
- [ListWorkflowDefinitionsRequestPaginateTypeDef](./type_defs.md#listworkflowdefinitionsrequestpaginatetypedef)
- [ListWorkflowRunsRequestPaginateTypeDef](./type_defs.md#listworkflowrunsrequestpaginatetypedef)
- [ListSessionsResponseTypeDef](./type_defs.md#listsessionsresponsetypedef)
- [ListWorkflowDefinitionsResponseTypeDef](./type_defs.md#listworkflowdefinitionsresponsetypedef)
- [ModelSummaryTypeDef](./type_defs.md#modelsummarytypedef)
- [ToolSpecTypeDef](./type_defs.md#toolspectypedef)
- [ListActsResponseTypeDef](./type_defs.md#listactsresponsetypedef)
- [ListWorkflowRunsResponseTypeDef](./type_defs.md#listworkflowrunsresponsetypedef)
- [InvokeActStepRequestTypeDef](./type_defs.md#invokeactsteprequesttypedef)
- [ListModelsResponseTypeDef](./type_defs.md#listmodelsresponsetypedef)
- [CreateActRequestTypeDef](./type_defs.md#createactrequesttypedef)

