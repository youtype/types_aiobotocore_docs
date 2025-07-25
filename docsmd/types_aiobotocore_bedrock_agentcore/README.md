# BedrockAgentCoreDataPlaneFrontingLayer module

> [Index](../README.md) > BedrockAgentCoreDataPlaneFrontingLayer


!!! note ""

    Auto-generated documentation for [BedrockAgentCoreDataPlaneFrontingLayer](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore.html#bedrockagentcoredataplanefrontinglayer)
    type annotations stubs module [types-aiobotocore-bedrock-agentcore](https://pypi.org/project/types-aiobotocore-bedrock-agentcore/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy-boto3-builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.23.2' mypy-boto3-builder`
1. Select `aiobotocore` AWS SDK.
1. Add `BedrockAgentCoreDataPlaneFrontingLayer` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `BedrockAgentCoreDataPlaneFrontingLayer` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[bedrock-agentcore]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[bedrock-agentcore]'

# standalone installation
python -m pip install types-aiobotocore-bedrock-agentcore
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-bedrock-agentcore
```

## Usage

Code samples can be found in [Examples](./usage.md).

## BedrockAgentCoreDataPlaneFrontingLayerClient

Type annotations and code completion for  `#!python session.create_client("bedrock-agentcore")` as [BedrockAgentCoreDataPlaneFrontingLayerClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore.html#BedrockAgentCoreDataPlaneFrontingLayer.Client)

```python
# BedrockAgentCoreDataPlaneFrontingLayerClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_bedrock_agentcore.client import BedrockAgentCoreDataPlaneFrontingLayerClient


session = get_session()
async with session.create_client("bedrock-agentcore") as client:
    client: BedrockAgentCoreDataPlaneFrontingLayerClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("bedrock-agentcore").get_paginator("...")`.

```python
# ListActorsPaginator usage example

from types_aiobotocore_bedrock_agentcore.paginator import ListActorsPaginator

def get_list_actors_paginator() -> ListActorsPaginator:
    return client.get_paginator("list_actors"))
```

- [ListActorsPaginator](./paginators.md#listactorspaginator)
- [ListEventsPaginator](./paginators.md#listeventspaginator)
- [ListMemoryRecordsPaginator](./paginators.md#listmemoryrecordspaginator)
- [ListSessionsPaginator](./paginators.md#listsessionspaginator)
- [RetrieveMemoryRecordsPaginator](./paginators.md#retrievememoryrecordspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# AutomationStreamStatusType usage example

from types_aiobotocore_bedrock_agentcore.literals import AutomationStreamStatusType

def get_value() -> AutomationStreamStatusType:
    return "DISABLED"
```

- [AutomationStreamStatusType](./literals.md#automationstreamstatustype)
- [BrowserSessionStatusType](./literals.md#browsersessionstatustype)
- [CodeInterpreterSessionStatusType](./literals.md#codeinterpretersessionstatustype)
- [ContentBlockTypeType](./literals.md#contentblocktypetype)
- [ListActorsPaginatorName](./literals.md#listactorspaginatorname)
- [ListEventsPaginatorName](./literals.md#listeventspaginatorname)
- [ListMemoryRecordsPaginatorName](./literals.md#listmemoryrecordspaginatorname)
- [ListSessionsPaginatorName](./literals.md#listsessionspaginatorname)
- [Oauth2FlowTypeType](./literals.md#oauth2flowtypetype)
- [ProgrammingLanguageType](./literals.md#programminglanguagetype)
- [ResourceContentTypeType](./literals.md#resourcecontenttypetype)
- [RetrieveMemoryRecordsPaginatorName](./literals.md#retrievememoryrecordspaginatorname)
- [RoleType](./literals.md#roletype)
- [TaskStatusType](./literals.md#taskstatustype)
- [ToolNameType](./literals.md#toolnametype)
- [ValidationExceptionReasonType](./literals.md#validationexceptionreasontype)
- [BedrockAgentCoreDataPlaneFrontingLayerServiceName](./literals.md#bedrockagentcoredataplanefrontinglayerservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AccessDeniedExceptionTypeDef](./type_defs.md#accessdeniedexceptiontypedef)
- [ActorSummaryTypeDef](./type_defs.md#actorsummarytypedef)
- [AutomationStreamTypeDef](./type_defs.md#automationstreamtypedef)
- [AutomationStreamUpdateTypeDef](./type_defs.md#automationstreamupdatetypedef)
- [BlobTypeDef](./type_defs.md#blobtypedef)
- [BranchFilterTypeDef](./type_defs.md#branchfiltertypedef)
- [BranchTypeDef](./type_defs.md#branchtypedef)
- [LiveViewStreamTypeDef](./type_defs.md#liveviewstreamtypedef)
- [BrowserSessionSummaryTypeDef](./type_defs.md#browsersessionsummarytypedef)
- [ToolResultStructuredContentTypeDef](./type_defs.md#toolresultstructuredcontenttypedef)
- [CodeInterpreterSessionSummaryTypeDef](./type_defs.md#codeinterpretersessionsummarytypedef)
- [ConflictExceptionTypeDef](./type_defs.md#conflictexceptiontypedef)
- [InternalServerExceptionTypeDef](./type_defs.md#internalserverexceptiontypedef)
- [ResourceNotFoundExceptionTypeDef](./type_defs.md#resourcenotfoundexceptiontypedef)
- [ServiceQuotaExceededExceptionTypeDef](./type_defs.md#servicequotaexceededexceptiontypedef)
- [ThrottlingExceptionTypeDef](./type_defs.md#throttlingexceptiontypedef)
- [ResourceContentTypeDef](./type_defs.md#resourcecontenttypedef)
- [ContentTypeDef](./type_defs.md#contenttypedef)
- [TimestampTypeDef](./type_defs.md#timestamptypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [DeleteEventInputTypeDef](./type_defs.md#deleteeventinputtypedef)
- [DeleteMemoryRecordInputTypeDef](./type_defs.md#deletememoryrecordinputtypedef)
- [GetBrowserSessionRequestTypeDef](./type_defs.md#getbrowsersessionrequesttypedef)
- [ViewPortTypeDef](./type_defs.md#viewporttypedef)
- [GetCodeInterpreterSessionRequestTypeDef](./type_defs.md#getcodeinterpretersessionrequesttypedef)
- [GetEventInputTypeDef](./type_defs.md#geteventinputtypedef)
- [GetMemoryRecordInputTypeDef](./type_defs.md#getmemoryrecordinputtypedef)
- [GetResourceApiKeyRequestTypeDef](./type_defs.md#getresourceapikeyrequesttypedef)
- [GetResourceOauth2TokenRequestTypeDef](./type_defs.md#getresourceoauth2tokenrequesttypedef)
- [GetWorkloadAccessTokenForJWTRequestTypeDef](./type_defs.md#getworkloadaccesstokenforjwtrequesttypedef)
- [GetWorkloadAccessTokenForUserIdRequestTypeDef](./type_defs.md#getworkloadaccesstokenforuseridrequesttypedef)
- [GetWorkloadAccessTokenRequestTypeDef](./type_defs.md#getworkloadaccesstokenrequesttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListActorsInputTypeDef](./type_defs.md#listactorsinputtypedef)
- [ListBrowserSessionsRequestTypeDef](./type_defs.md#listbrowsersessionsrequesttypedef)
- [ListCodeInterpreterSessionsRequestTypeDef](./type_defs.md#listcodeinterpretersessionsrequesttypedef)
- [ListMemoryRecordsInputTypeDef](./type_defs.md#listmemoryrecordsinputtypedef)
- [ListSessionsInputTypeDef](./type_defs.md#listsessionsinputtypedef)
- [SessionSummaryTypeDef](./type_defs.md#sessionsummarytypedef)
- [MemoryContentTypeDef](./type_defs.md#memorycontenttypedef)
- [SearchCriteriaTypeDef](./type_defs.md#searchcriteriatypedef)
- [StartCodeInterpreterSessionRequestTypeDef](./type_defs.md#startcodeinterpretersessionrequesttypedef)
- [StopBrowserSessionRequestTypeDef](./type_defs.md#stopbrowsersessionrequesttypedef)
- [StopCodeInterpreterSessionRequestTypeDef](./type_defs.md#stopcodeinterpretersessionrequesttypedef)
- [ValidationExceptionFieldTypeDef](./type_defs.md#validationexceptionfieldtypedef)
- [StreamUpdateTypeDef](./type_defs.md#streamupdatetypedef)
- [InputContentBlockTypeDef](./type_defs.md#inputcontentblocktypedef)
- [InvokeAgentRuntimeRequestTypeDef](./type_defs.md#invokeagentruntimerequesttypedef)
- [FilterInputTypeDef](./type_defs.md#filterinputtypedef)
- [BrowserSessionStreamTypeDef](./type_defs.md#browsersessionstreamtypedef)
- [ContentBlockTypeDef](./type_defs.md#contentblocktypedef)
- [ConversationalTypeDef](./type_defs.md#conversationaltypedef)
- [DeleteEventOutputTypeDef](./type_defs.md#deleteeventoutputtypedef)
- [DeleteMemoryRecordOutputTypeDef](./type_defs.md#deletememoryrecordoutputtypedef)
- [GetCodeInterpreterSessionResponseTypeDef](./type_defs.md#getcodeinterpretersessionresponsetypedef)
- [GetResourceApiKeyResponseTypeDef](./type_defs.md#getresourceapikeyresponsetypedef)
- [GetResourceOauth2TokenResponseTypeDef](./type_defs.md#getresourceoauth2tokenresponsetypedef)
- [GetWorkloadAccessTokenForJWTResponseTypeDef](./type_defs.md#getworkloadaccesstokenforjwtresponsetypedef)
- [GetWorkloadAccessTokenForUserIdResponseTypeDef](./type_defs.md#getworkloadaccesstokenforuseridresponsetypedef)
- [GetWorkloadAccessTokenResponseTypeDef](./type_defs.md#getworkloadaccesstokenresponsetypedef)
- [InvokeAgentRuntimeResponseTypeDef](./type_defs.md#invokeagentruntimeresponsetypedef)
- [ListActorsOutputTypeDef](./type_defs.md#listactorsoutputtypedef)
- [ListBrowserSessionsResponseTypeDef](./type_defs.md#listbrowsersessionsresponsetypedef)
- [ListCodeInterpreterSessionsResponseTypeDef](./type_defs.md#listcodeinterpretersessionsresponsetypedef)
- [StartCodeInterpreterSessionResponseTypeDef](./type_defs.md#startcodeinterpretersessionresponsetypedef)
- [StopBrowserSessionResponseTypeDef](./type_defs.md#stopbrowsersessionresponsetypedef)
- [StopCodeInterpreterSessionResponseTypeDef](./type_defs.md#stopcodeinterpretersessionresponsetypedef)
- [StartBrowserSessionRequestTypeDef](./type_defs.md#startbrowsersessionrequesttypedef)
- [ListActorsInputPaginateTypeDef](./type_defs.md#listactorsinputpaginatetypedef)
- [ListMemoryRecordsInputPaginateTypeDef](./type_defs.md#listmemoryrecordsinputpaginatetypedef)
- [ListSessionsInputPaginateTypeDef](./type_defs.md#listsessionsinputpaginatetypedef)
- [ListSessionsOutputTypeDef](./type_defs.md#listsessionsoutputtypedef)
- [MemoryRecordSummaryTypeDef](./type_defs.md#memoryrecordsummarytypedef)
- [MemoryRecordTypeDef](./type_defs.md#memoryrecordtypedef)
- [RetrieveMemoryRecordsInputPaginateTypeDef](./type_defs.md#retrievememoryrecordsinputpaginatetypedef)
- [RetrieveMemoryRecordsInputTypeDef](./type_defs.md#retrievememoryrecordsinputtypedef)
- [ValidationExceptionTypeDef](./type_defs.md#validationexceptiontypedef)
- [UpdateBrowserStreamRequestTypeDef](./type_defs.md#updatebrowserstreamrequesttypedef)
- [ToolArgumentsTypeDef](./type_defs.md#toolargumentstypedef)
- [ListEventsInputPaginateTypeDef](./type_defs.md#listeventsinputpaginatetypedef)
- [ListEventsInputTypeDef](./type_defs.md#listeventsinputtypedef)
- [GetBrowserSessionResponseTypeDef](./type_defs.md#getbrowsersessionresponsetypedef)
- [StartBrowserSessionResponseTypeDef](./type_defs.md#startbrowsersessionresponsetypedef)
- [UpdateBrowserStreamResponseTypeDef](./type_defs.md#updatebrowserstreamresponsetypedef)
- [CodeInterpreterResultTypeDef](./type_defs.md#codeinterpreterresulttypedef)
- [PayloadTypeOutputTypeDef](./type_defs.md#payloadtypeoutputtypedef)
- [PayloadTypeTypeDef](./type_defs.md#payloadtypetypedef)
- [ListMemoryRecordsOutputTypeDef](./type_defs.md#listmemoryrecordsoutputtypedef)
- [RetrieveMemoryRecordsOutputTypeDef](./type_defs.md#retrievememoryrecordsoutputtypedef)
- [GetMemoryRecordOutputTypeDef](./type_defs.md#getmemoryrecordoutputtypedef)
- [InvokeCodeInterpreterRequestTypeDef](./type_defs.md#invokecodeinterpreterrequesttypedef)
- [CodeInterpreterStreamOutputTypeDef](./type_defs.md#codeinterpreterstreamoutputtypedef)
- [EventTypeDef](./type_defs.md#eventtypedef)
- [PayloadTypeUnionTypeDef](./type_defs.md#payloadtypeuniontypedef)
- [InvokeCodeInterpreterResponseTypeDef](./type_defs.md#invokecodeinterpreterresponsetypedef)
- [CreateEventOutputTypeDef](./type_defs.md#createeventoutputtypedef)
- [GetEventOutputTypeDef](./type_defs.md#geteventoutputtypedef)
- [ListEventsOutputTypeDef](./type_defs.md#listeventsoutputtypedef)
- [CreateEventInputTypeDef](./type_defs.md#createeventinputtypedef)

