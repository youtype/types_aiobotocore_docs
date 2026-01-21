# Paginators

> [Index](../README.md) > [CleanRoomsService](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [CleanRoomsService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#cleanroomsservice)
    type annotations stubs module [types-aiobotocore-cleanrooms](https://pypi.org/project/types-aiobotocore-cleanrooms/).

## ListAnalysisTemplatesPaginator

Type annotations and code completion for `#!python session.create_client("cleanrooms").get_paginator("list_analysis_templates")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms/paginator/ListAnalysisTemplates.html#CleanRoomsService.Paginator.ListAnalysisTemplates)

```python
# ListAnalysisTemplatesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_cleanrooms.paginator import ListAnalysisTemplatesPaginator

session = get_session()
async with session.create_client("cleanrooms") as client:  # (1)
    paginator: ListAnalysisTemplatesPaginator = client.get_paginator("list_analysis_templates")  # (2)
    async for item in paginator.paginate(...):
        item: ListAnalysisTemplatesOutputTypeDef
        print(item)  # (3)
```

1. client: [CleanRoomsServiceClient](./client.md)
2. paginator: [ListAnalysisTemplatesPaginator](./paginators.md#listanalysistemplatespaginator)
3. item: `AioPageIterator[ListAnalysisTemplatesOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListAnalysisTemplatesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    membershipIdentifier: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListAnalysisTemplatesOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListAnalysisTemplatesOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListAnalysisTemplatesInputPaginateTypeDef = {  # (1)
    "membershipIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAnalysisTemplatesInputPaginateTypeDef](./type_defs.md#listanalysistemplatesinputpaginatetypedef)
## ListCollaborationAnalysisTemplatesPaginator

Type annotations and code completion for `#!python session.create_client("cleanrooms").get_paginator("list_collaboration_analysis_templates")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms/paginator/ListCollaborationAnalysisTemplates.html#CleanRoomsService.Paginator.ListCollaborationAnalysisTemplates)

```python
# ListCollaborationAnalysisTemplatesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_cleanrooms.paginator import ListCollaborationAnalysisTemplatesPaginator

session = get_session()
async with session.create_client("cleanrooms") as client:  # (1)
    paginator: ListCollaborationAnalysisTemplatesPaginator = client.get_paginator("list_collaboration_analysis_templates")  # (2)
    async for item in paginator.paginate(...):
        item: ListCollaborationAnalysisTemplatesOutputTypeDef
        print(item)  # (3)
```

1. client: [CleanRoomsServiceClient](./client.md)
2. paginator: [ListCollaborationAnalysisTemplatesPaginator](./paginators.md#listcollaborationanalysistemplatespaginator)
3. item: `AioPageIterator[ListCollaborationAnalysisTemplatesOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListCollaborationAnalysisTemplatesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    collaborationIdentifier: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListCollaborationAnalysisTemplatesOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListCollaborationAnalysisTemplatesOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListCollaborationAnalysisTemplatesInputPaginateTypeDef = {  # (1)
    "collaborationIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListCollaborationAnalysisTemplatesInputPaginateTypeDef](./type_defs.md#listcollaborationanalysistemplatesinputpaginatetypedef)
## ListCollaborationChangeRequestsPaginator

Type annotations and code completion for `#!python session.create_client("cleanrooms").get_paginator("list_collaboration_change_requests")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms/paginator/ListCollaborationChangeRequests.html#CleanRoomsService.Paginator.ListCollaborationChangeRequests)

```python
# ListCollaborationChangeRequestsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_cleanrooms.paginator import ListCollaborationChangeRequestsPaginator

session = get_session()
async with session.create_client("cleanrooms") as client:  # (1)
    paginator: ListCollaborationChangeRequestsPaginator = client.get_paginator("list_collaboration_change_requests")  # (2)
    async for item in paginator.paginate(...):
        item: ListCollaborationChangeRequestsOutputTypeDef
        print(item)  # (3)
```

1. client: [CleanRoomsServiceClient](./client.md)
2. paginator: [ListCollaborationChangeRequestsPaginator](./paginators.md#listcollaborationchangerequestspaginator)
3. item: `AioPageIterator[ListCollaborationChangeRequestsOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListCollaborationChangeRequestsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    collaborationIdentifier: str,
    status: ChangeRequestStatusType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListCollaborationChangeRequestsOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: ChangeRequestStatusType](./literals.md#changerequeststatustype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListCollaborationChangeRequestsOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListCollaborationChangeRequestsInputPaginateTypeDef = {  # (1)
    "collaborationIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListCollaborationChangeRequestsInputPaginateTypeDef](./type_defs.md#listcollaborationchangerequestsinputpaginatetypedef)
## ListCollaborationConfiguredAudienceModelAssociationsPaginator

Type annotations and code completion for `#!python session.create_client("cleanrooms").get_paginator("list_collaboration_configured_audience_model_associations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms/paginator/ListCollaborationConfiguredAudienceModelAssociations.html#CleanRoomsService.Paginator.ListCollaborationConfiguredAudienceModelAssociations)

```python
# ListCollaborationConfiguredAudienceModelAssociationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_cleanrooms.paginator import ListCollaborationConfiguredAudienceModelAssociationsPaginator

session = get_session()
async with session.create_client("cleanrooms") as client:  # (1)
    paginator: ListCollaborationConfiguredAudienceModelAssociationsPaginator = client.get_paginator("list_collaboration_configured_audience_model_associations")  # (2)
    async for item in paginator.paginate(...):
        item: ListCollaborationConfiguredAudienceModelAssociationsOutputTypeDef
        print(item)  # (3)
```

1. client: [CleanRoomsServiceClient](./client.md)
2. paginator: [ListCollaborationConfiguredAudienceModelAssociationsPaginator](./paginators.md#listcollaborationconfiguredaudiencemodelassociationspaginator)
3. item: `AioPageIterator[ListCollaborationConfiguredAudienceModelAssociationsOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListCollaborationConfiguredAudienceModelAssociationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    collaborationIdentifier: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListCollaborationConfiguredAudienceModelAssociationsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListCollaborationConfiguredAudienceModelAssociationsOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListCollaborationConfiguredAudienceModelAssociationsInputPaginateTypeDef = {  # (1)
    "collaborationIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListCollaborationConfiguredAudienceModelAssociationsInputPaginateTypeDef](./type_defs.md#listcollaborationconfiguredaudiencemodelassociationsinputpaginatetypedef)
## ListCollaborationIdNamespaceAssociationsPaginator

Type annotations and code completion for `#!python session.create_client("cleanrooms").get_paginator("list_collaboration_id_namespace_associations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms/paginator/ListCollaborationIdNamespaceAssociations.html#CleanRoomsService.Paginator.ListCollaborationIdNamespaceAssociations)

```python
# ListCollaborationIdNamespaceAssociationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_cleanrooms.paginator import ListCollaborationIdNamespaceAssociationsPaginator

session = get_session()
async with session.create_client("cleanrooms") as client:  # (1)
    paginator: ListCollaborationIdNamespaceAssociationsPaginator = client.get_paginator("list_collaboration_id_namespace_associations")  # (2)
    async for item in paginator.paginate(...):
        item: ListCollaborationIdNamespaceAssociationsOutputTypeDef
        print(item)  # (3)
```

1. client: [CleanRoomsServiceClient](./client.md)
2. paginator: [ListCollaborationIdNamespaceAssociationsPaginator](./paginators.md#listcollaborationidnamespaceassociationspaginator)
3. item: `AioPageIterator[ListCollaborationIdNamespaceAssociationsOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListCollaborationIdNamespaceAssociationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    collaborationIdentifier: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListCollaborationIdNamespaceAssociationsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListCollaborationIdNamespaceAssociationsOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListCollaborationIdNamespaceAssociationsInputPaginateTypeDef = {  # (1)
    "collaborationIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListCollaborationIdNamespaceAssociationsInputPaginateTypeDef](./type_defs.md#listcollaborationidnamespaceassociationsinputpaginatetypedef)
## ListCollaborationPrivacyBudgetTemplatesPaginator

Type annotations and code completion for `#!python session.create_client("cleanrooms").get_paginator("list_collaboration_privacy_budget_templates")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms/paginator/ListCollaborationPrivacyBudgetTemplates.html#CleanRoomsService.Paginator.ListCollaborationPrivacyBudgetTemplates)

```python
# ListCollaborationPrivacyBudgetTemplatesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_cleanrooms.paginator import ListCollaborationPrivacyBudgetTemplatesPaginator

session = get_session()
async with session.create_client("cleanrooms") as client:  # (1)
    paginator: ListCollaborationPrivacyBudgetTemplatesPaginator = client.get_paginator("list_collaboration_privacy_budget_templates")  # (2)
    async for item in paginator.paginate(...):
        item: ListCollaborationPrivacyBudgetTemplatesOutputTypeDef
        print(item)  # (3)
```

1. client: [CleanRoomsServiceClient](./client.md)
2. paginator: [ListCollaborationPrivacyBudgetTemplatesPaginator](./paginators.md#listcollaborationprivacybudgettemplatespaginator)
3. item: `AioPageIterator[ListCollaborationPrivacyBudgetTemplatesOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListCollaborationPrivacyBudgetTemplatesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    collaborationIdentifier: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListCollaborationPrivacyBudgetTemplatesOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListCollaborationPrivacyBudgetTemplatesOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListCollaborationPrivacyBudgetTemplatesInputPaginateTypeDef = {  # (1)
    "collaborationIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListCollaborationPrivacyBudgetTemplatesInputPaginateTypeDef](./type_defs.md#listcollaborationprivacybudgettemplatesinputpaginatetypedef)
## ListCollaborationPrivacyBudgetsPaginator

Type annotations and code completion for `#!python session.create_client("cleanrooms").get_paginator("list_collaboration_privacy_budgets")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms/paginator/ListCollaborationPrivacyBudgets.html#CleanRoomsService.Paginator.ListCollaborationPrivacyBudgets)

```python
# ListCollaborationPrivacyBudgetsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_cleanrooms.paginator import ListCollaborationPrivacyBudgetsPaginator

session = get_session()
async with session.create_client("cleanrooms") as client:  # (1)
    paginator: ListCollaborationPrivacyBudgetsPaginator = client.get_paginator("list_collaboration_privacy_budgets")  # (2)
    async for item in paginator.paginate(...):
        item: ListCollaborationPrivacyBudgetsOutputTypeDef
        print(item)  # (3)
```

1. client: [CleanRoomsServiceClient](./client.md)
2. paginator: [ListCollaborationPrivacyBudgetsPaginator](./paginators.md#listcollaborationprivacybudgetspaginator)
3. item: `AioPageIterator[ListCollaborationPrivacyBudgetsOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListCollaborationPrivacyBudgetsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    collaborationIdentifier: str,
    privacyBudgetType: PrivacyBudgetTypeType,  # (1)
    accessBudgetResourceArn: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListCollaborationPrivacyBudgetsOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: PrivacyBudgetTypeType](./literals.md#privacybudgettypetype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListCollaborationPrivacyBudgetsOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListCollaborationPrivacyBudgetsInputPaginateTypeDef = {  # (1)
    "collaborationIdentifier": ...,
    "privacyBudgetType": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListCollaborationPrivacyBudgetsInputPaginateTypeDef](./type_defs.md#listcollaborationprivacybudgetsinputpaginatetypedef)
## ListCollaborationsPaginator

Type annotations and code completion for `#!python session.create_client("cleanrooms").get_paginator("list_collaborations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms/paginator/ListCollaborations.html#CleanRoomsService.Paginator.ListCollaborations)

```python
# ListCollaborationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_cleanrooms.paginator import ListCollaborationsPaginator

session = get_session()
async with session.create_client("cleanrooms") as client:  # (1)
    paginator: ListCollaborationsPaginator = client.get_paginator("list_collaborations")  # (2)
    async for item in paginator.paginate(...):
        item: ListCollaborationsOutputTypeDef
        print(item)  # (3)
```

1. client: [CleanRoomsServiceClient](./client.md)
2. paginator: [ListCollaborationsPaginator](./paginators.md#listcollaborationspaginator)
3. item: `AioPageIterator[ListCollaborationsOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListCollaborationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    memberStatus: FilterableMemberStatusType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListCollaborationsOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: FilterableMemberStatusType](./literals.md#filterablememberstatustype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListCollaborationsOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListCollaborationsInputPaginateTypeDef = {  # (1)
    "memberStatus": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListCollaborationsInputPaginateTypeDef](./type_defs.md#listcollaborationsinputpaginatetypedef)
## ListConfiguredAudienceModelAssociationsPaginator

Type annotations and code completion for `#!python session.create_client("cleanrooms").get_paginator("list_configured_audience_model_associations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms/paginator/ListConfiguredAudienceModelAssociations.html#CleanRoomsService.Paginator.ListConfiguredAudienceModelAssociations)

```python
# ListConfiguredAudienceModelAssociationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_cleanrooms.paginator import ListConfiguredAudienceModelAssociationsPaginator

session = get_session()
async with session.create_client("cleanrooms") as client:  # (1)
    paginator: ListConfiguredAudienceModelAssociationsPaginator = client.get_paginator("list_configured_audience_model_associations")  # (2)
    async for item in paginator.paginate(...):
        item: ListConfiguredAudienceModelAssociationsOutputTypeDef
        print(item)  # (3)
```

1. client: [CleanRoomsServiceClient](./client.md)
2. paginator: [ListConfiguredAudienceModelAssociationsPaginator](./paginators.md#listconfiguredaudiencemodelassociationspaginator)
3. item: `AioPageIterator[ListConfiguredAudienceModelAssociationsOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListConfiguredAudienceModelAssociationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    membershipIdentifier: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListConfiguredAudienceModelAssociationsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListConfiguredAudienceModelAssociationsOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListConfiguredAudienceModelAssociationsInputPaginateTypeDef = {  # (1)
    "membershipIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListConfiguredAudienceModelAssociationsInputPaginateTypeDef](./type_defs.md#listconfiguredaudiencemodelassociationsinputpaginatetypedef)
## ListConfiguredTableAssociationsPaginator

Type annotations and code completion for `#!python session.create_client("cleanrooms").get_paginator("list_configured_table_associations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms/paginator/ListConfiguredTableAssociations.html#CleanRoomsService.Paginator.ListConfiguredTableAssociations)

```python
# ListConfiguredTableAssociationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_cleanrooms.paginator import ListConfiguredTableAssociationsPaginator

session = get_session()
async with session.create_client("cleanrooms") as client:  # (1)
    paginator: ListConfiguredTableAssociationsPaginator = client.get_paginator("list_configured_table_associations")  # (2)
    async for item in paginator.paginate(...):
        item: ListConfiguredTableAssociationsOutputTypeDef
        print(item)  # (3)
```

1. client: [CleanRoomsServiceClient](./client.md)
2. paginator: [ListConfiguredTableAssociationsPaginator](./paginators.md#listconfiguredtableassociationspaginator)
3. item: `AioPageIterator[ListConfiguredTableAssociationsOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListConfiguredTableAssociationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    membershipIdentifier: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListConfiguredTableAssociationsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListConfiguredTableAssociationsOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListConfiguredTableAssociationsInputPaginateTypeDef = {  # (1)
    "membershipIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListConfiguredTableAssociationsInputPaginateTypeDef](./type_defs.md#listconfiguredtableassociationsinputpaginatetypedef)
## ListConfiguredTablesPaginator

Type annotations and code completion for `#!python session.create_client("cleanrooms").get_paginator("list_configured_tables")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms/paginator/ListConfiguredTables.html#CleanRoomsService.Paginator.ListConfiguredTables)

```python
# ListConfiguredTablesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_cleanrooms.paginator import ListConfiguredTablesPaginator

session = get_session()
async with session.create_client("cleanrooms") as client:  # (1)
    paginator: ListConfiguredTablesPaginator = client.get_paginator("list_configured_tables")  # (2)
    async for item in paginator.paginate(...):
        item: ListConfiguredTablesOutputTypeDef
        print(item)  # (3)
```

1. client: [CleanRoomsServiceClient](./client.md)
2. paginator: [ListConfiguredTablesPaginator](./paginators.md#listconfiguredtablespaginator)
3. item: `AioPageIterator[ListConfiguredTablesOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListConfiguredTablesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListConfiguredTablesOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListConfiguredTablesOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListConfiguredTablesInputPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListConfiguredTablesInputPaginateTypeDef](./type_defs.md#listconfiguredtablesinputpaginatetypedef)
## ListIdMappingTablesPaginator

Type annotations and code completion for `#!python session.create_client("cleanrooms").get_paginator("list_id_mapping_tables")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms/paginator/ListIdMappingTables.html#CleanRoomsService.Paginator.ListIdMappingTables)

```python
# ListIdMappingTablesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_cleanrooms.paginator import ListIdMappingTablesPaginator

session = get_session()
async with session.create_client("cleanrooms") as client:  # (1)
    paginator: ListIdMappingTablesPaginator = client.get_paginator("list_id_mapping_tables")  # (2)
    async for item in paginator.paginate(...):
        item: ListIdMappingTablesOutputTypeDef
        print(item)  # (3)
```

1. client: [CleanRoomsServiceClient](./client.md)
2. paginator: [ListIdMappingTablesPaginator](./paginators.md#listidmappingtablespaginator)
3. item: `AioPageIterator[ListIdMappingTablesOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListIdMappingTablesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    membershipIdentifier: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListIdMappingTablesOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListIdMappingTablesOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListIdMappingTablesInputPaginateTypeDef = {  # (1)
    "membershipIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListIdMappingTablesInputPaginateTypeDef](./type_defs.md#listidmappingtablesinputpaginatetypedef)
## ListIdNamespaceAssociationsPaginator

Type annotations and code completion for `#!python session.create_client("cleanrooms").get_paginator("list_id_namespace_associations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms/paginator/ListIdNamespaceAssociations.html#CleanRoomsService.Paginator.ListIdNamespaceAssociations)

```python
# ListIdNamespaceAssociationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_cleanrooms.paginator import ListIdNamespaceAssociationsPaginator

session = get_session()
async with session.create_client("cleanrooms") as client:  # (1)
    paginator: ListIdNamespaceAssociationsPaginator = client.get_paginator("list_id_namespace_associations")  # (2)
    async for item in paginator.paginate(...):
        item: ListIdNamespaceAssociationsOutputTypeDef
        print(item)  # (3)
```

1. client: [CleanRoomsServiceClient](./client.md)
2. paginator: [ListIdNamespaceAssociationsPaginator](./paginators.md#listidnamespaceassociationspaginator)
3. item: `AioPageIterator[ListIdNamespaceAssociationsOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListIdNamespaceAssociationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    membershipIdentifier: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListIdNamespaceAssociationsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListIdNamespaceAssociationsOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListIdNamespaceAssociationsInputPaginateTypeDef = {  # (1)
    "membershipIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListIdNamespaceAssociationsInputPaginateTypeDef](./type_defs.md#listidnamespaceassociationsinputpaginatetypedef)
## ListMembersPaginator

Type annotations and code completion for `#!python session.create_client("cleanrooms").get_paginator("list_members")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms/paginator/ListMembers.html#CleanRoomsService.Paginator.ListMembers)

```python
# ListMembersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_cleanrooms.paginator import ListMembersPaginator

session = get_session()
async with session.create_client("cleanrooms") as client:  # (1)
    paginator: ListMembersPaginator = client.get_paginator("list_members")  # (2)
    async for item in paginator.paginate(...):
        item: ListMembersOutputTypeDef
        print(item)  # (3)
```

1. client: [CleanRoomsServiceClient](./client.md)
2. paginator: [ListMembersPaginator](./paginators.md#listmemberspaginator)
3. item: `AioPageIterator[ListMembersOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListMembersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    collaborationIdentifier: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListMembersOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListMembersOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListMembersInputPaginateTypeDef = {  # (1)
    "collaborationIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListMembersInputPaginateTypeDef](./type_defs.md#listmembersinputpaginatetypedef)
## ListMembershipsPaginator

Type annotations and code completion for `#!python session.create_client("cleanrooms").get_paginator("list_memberships")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms/paginator/ListMemberships.html#CleanRoomsService.Paginator.ListMemberships)

```python
# ListMembershipsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_cleanrooms.paginator import ListMembershipsPaginator

session = get_session()
async with session.create_client("cleanrooms") as client:  # (1)
    paginator: ListMembershipsPaginator = client.get_paginator("list_memberships")  # (2)
    async for item in paginator.paginate(...):
        item: ListMembershipsOutputTypeDef
        print(item)  # (3)
```

1. client: [CleanRoomsServiceClient](./client.md)
2. paginator: [ListMembershipsPaginator](./paginators.md#listmembershipspaginator)
3. item: `AioPageIterator[ListMembershipsOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListMembershipsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    status: MembershipStatusType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListMembershipsOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: MembershipStatusType](./literals.md#membershipstatustype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListMembershipsOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListMembershipsInputPaginateTypeDef = {  # (1)
    "status": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListMembershipsInputPaginateTypeDef](./type_defs.md#listmembershipsinputpaginatetypedef)
## ListPrivacyBudgetTemplatesPaginator

Type annotations and code completion for `#!python session.create_client("cleanrooms").get_paginator("list_privacy_budget_templates")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms/paginator/ListPrivacyBudgetTemplates.html#CleanRoomsService.Paginator.ListPrivacyBudgetTemplates)

```python
# ListPrivacyBudgetTemplatesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_cleanrooms.paginator import ListPrivacyBudgetTemplatesPaginator

session = get_session()
async with session.create_client("cleanrooms") as client:  # (1)
    paginator: ListPrivacyBudgetTemplatesPaginator = client.get_paginator("list_privacy_budget_templates")  # (2)
    async for item in paginator.paginate(...):
        item: ListPrivacyBudgetTemplatesOutputTypeDef
        print(item)  # (3)
```

1. client: [CleanRoomsServiceClient](./client.md)
2. paginator: [ListPrivacyBudgetTemplatesPaginator](./paginators.md#listprivacybudgettemplatespaginator)
3. item: `AioPageIterator[ListPrivacyBudgetTemplatesOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListPrivacyBudgetTemplatesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    membershipIdentifier: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListPrivacyBudgetTemplatesOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListPrivacyBudgetTemplatesOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListPrivacyBudgetTemplatesInputPaginateTypeDef = {  # (1)
    "membershipIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListPrivacyBudgetTemplatesInputPaginateTypeDef](./type_defs.md#listprivacybudgettemplatesinputpaginatetypedef)
## ListPrivacyBudgetsPaginator

Type annotations and code completion for `#!python session.create_client("cleanrooms").get_paginator("list_privacy_budgets")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms/paginator/ListPrivacyBudgets.html#CleanRoomsService.Paginator.ListPrivacyBudgets)

```python
# ListPrivacyBudgetsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_cleanrooms.paginator import ListPrivacyBudgetsPaginator

session = get_session()
async with session.create_client("cleanrooms") as client:  # (1)
    paginator: ListPrivacyBudgetsPaginator = client.get_paginator("list_privacy_budgets")  # (2)
    async for item in paginator.paginate(...):
        item: ListPrivacyBudgetsOutputTypeDef
        print(item)  # (3)
```

1. client: [CleanRoomsServiceClient](./client.md)
2. paginator: [ListPrivacyBudgetsPaginator](./paginators.md#listprivacybudgetspaginator)
3. item: `AioPageIterator[ListPrivacyBudgetsOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListPrivacyBudgetsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    membershipIdentifier: str,
    privacyBudgetType: PrivacyBudgetTypeType,  # (1)
    accessBudgetResourceArn: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListPrivacyBudgetsOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: PrivacyBudgetTypeType](./literals.md#privacybudgettypetype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListPrivacyBudgetsOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListPrivacyBudgetsInputPaginateTypeDef = {  # (1)
    "membershipIdentifier": ...,
    "privacyBudgetType": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListPrivacyBudgetsInputPaginateTypeDef](./type_defs.md#listprivacybudgetsinputpaginatetypedef)
## ListProtectedJobsPaginator

Type annotations and code completion for `#!python session.create_client("cleanrooms").get_paginator("list_protected_jobs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms/paginator/ListProtectedJobs.html#CleanRoomsService.Paginator.ListProtectedJobs)

```python
# ListProtectedJobsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_cleanrooms.paginator import ListProtectedJobsPaginator

session = get_session()
async with session.create_client("cleanrooms") as client:  # (1)
    paginator: ListProtectedJobsPaginator = client.get_paginator("list_protected_jobs")  # (2)
    async for item in paginator.paginate(...):
        item: ListProtectedJobsOutputTypeDef
        print(item)  # (3)
```

1. client: [CleanRoomsServiceClient](./client.md)
2. paginator: [ListProtectedJobsPaginator](./paginators.md#listprotectedjobspaginator)
3. item: `AioPageIterator[ListProtectedJobsOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListProtectedJobsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    membershipIdentifier: str,
    status: ProtectedJobStatusType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListProtectedJobsOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: ProtectedJobStatusType](./literals.md#protectedjobstatustype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListProtectedJobsOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListProtectedJobsInputPaginateTypeDef = {  # (1)
    "membershipIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListProtectedJobsInputPaginateTypeDef](./type_defs.md#listprotectedjobsinputpaginatetypedef)
## ListProtectedQueriesPaginator

Type annotations and code completion for `#!python session.create_client("cleanrooms").get_paginator("list_protected_queries")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms/paginator/ListProtectedQueries.html#CleanRoomsService.Paginator.ListProtectedQueries)

```python
# ListProtectedQueriesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_cleanrooms.paginator import ListProtectedQueriesPaginator

session = get_session()
async with session.create_client("cleanrooms") as client:  # (1)
    paginator: ListProtectedQueriesPaginator = client.get_paginator("list_protected_queries")  # (2)
    async for item in paginator.paginate(...):
        item: ListProtectedQueriesOutputTypeDef
        print(item)  # (3)
```

1. client: [CleanRoomsServiceClient](./client.md)
2. paginator: [ListProtectedQueriesPaginator](./paginators.md#listprotectedqueriespaginator)
3. item: `AioPageIterator[ListProtectedQueriesOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListProtectedQueriesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    membershipIdentifier: str,
    status: ProtectedQueryStatusType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListProtectedQueriesOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: ProtectedQueryStatusType](./literals.md#protectedquerystatustype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListProtectedQueriesOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListProtectedQueriesInputPaginateTypeDef = {  # (1)
    "membershipIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListProtectedQueriesInputPaginateTypeDef](./type_defs.md#listprotectedqueriesinputpaginatetypedef)
## ListSchemasPaginator

Type annotations and code completion for `#!python session.create_client("cleanrooms").get_paginator("list_schemas")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms/paginator/ListSchemas.html#CleanRoomsService.Paginator.ListSchemas)

```python
# ListSchemasPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_cleanrooms.paginator import ListSchemasPaginator

session = get_session()
async with session.create_client("cleanrooms") as client:  # (1)
    paginator: ListSchemasPaginator = client.get_paginator("list_schemas")  # (2)
    async for item in paginator.paginate(...):
        item: ListSchemasOutputTypeDef
        print(item)  # (3)
```

1. client: [CleanRoomsServiceClient](./client.md)
2. paginator: [ListSchemasPaginator](./paginators.md#listschemaspaginator)
3. item: `AioPageIterator[ListSchemasOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListSchemasPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    collaborationIdentifier: str,
    schemaType: SchemaTypeType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListSchemasOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: SchemaTypeType](./literals.md#schematypetype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListSchemasOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListSchemasInputPaginateTypeDef = {  # (1)
    "collaborationIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSchemasInputPaginateTypeDef](./type_defs.md#listschemasinputpaginatetypedef)
