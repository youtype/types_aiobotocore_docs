# Examples

> [Index](../README.md) > [PrometheusService](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [PrometheusService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService)
    type annotations stubs module [types-aiobotocore-amp](https://pypi.org/project/types-aiobotocore-amp/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[amp]` package installed.

Write your `PrometheusService` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aiobotocore.session import get_session


    session = get_session()

    async with session.create_client("amp") as client:  # (1)
        result = await client.create_alert_manager_definition()  # (2)
    ```

    1. client: [PrometheusServiceClient](./client.md)
    2. result: [:material-code-braces: CreateAlertManagerDefinitionResponseTypeDef](./type_defs.md#createalertmanagerdefinitionresponsetypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aiobotocore.session import get_session


    session = get_session()

    async with session.create_client("amp") as client:  # (1)
        paginator = client.get_paginator("list_rule_groups_namespaces")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [PrometheusServiceClient](./client.md)
    2. paginator: [ListRuleGroupsNamespacesPaginator](./paginators.md#listrulegroupsnamespacespaginator)
    3. item: [:material-code-braces: ListRuleGroupsNamespacesResponseTypeDef](./type_defs.md#listrulegroupsnamespacesresponsetypedef) 



=== "Waiters"

    ```python title="Waiter usage example"
    from aiobotocore.session import get_session


    session = get_session()

    async with session.create_client("amp") as client:  # (1)
        waiter = client.get_waiter("workspace_active")  # (2)
        await waiter.wait()
    ```

    1. client: [PrometheusServiceClient](./client.md)
    2. waiter: [WorkspaceActiveWaiter](./waiters.md#workspaceactivewaiter)


### Explicit type annotations

With `types-aiobotocore-lite[amp]`
or a standalone `types_aiobotocore_amp` package, you have to explicitly specify
`client: PrometheusServiceClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aiobotocore.session import get_session

    from types_aiobotocore_amp.client import PrometheusServiceClient
    from types_aiobotocore_amp.type_defs import CreateAlertManagerDefinitionResponseTypeDef
    from types_aiobotocore_amp.type_defs import CreateAlertManagerDefinitionRequestRequestTypeDef


    session = get_session()

    async with session.create_client("amp") as client:
        client: PrometheusServiceClient
        kwargs: CreateAlertManagerDefinitionRequestRequestTypeDef = {...}
        result: CreateAlertManagerDefinitionResponseTypeDef = await client.create_alert_manager_definition(**kwargs)
    ```



=== "Paginators"

    ```python title="Paginator usage example"
    from aiobotocore.session import get_session

    from types_aiobotocore_amp.client import PrometheusServiceClient
    from types_aiobotocore_amp.paginator import ListRuleGroupsNamespacesPaginator
    from types_aiobotocore_amp.type_defs import ListRuleGroupsNamespacesResponseTypeDef


    session = get_session()

    async with session.create_client("amp") as client:
        client: PrometheusServiceClient
        paginator: ListRuleGroupsNamespacesPaginator = client.get_paginator("list_rule_groups_namespaces")
        async for item in paginator.paginate(...):
            item: ListRuleGroupsNamespacesResponseTypeDef
            print(item)
    ```



=== "Waiters"

    ```python title="Waiter usage example"
    from aiobotocore.session import get_session

    from types_aiobotocore_amp.client import PrometheusServiceClient
    from types_aiobotocore_amp.waiter import WorkspaceActiveWaiter


    session = get_session()

    async with session.create_client("amp") as client:
        client: PrometheusServiceClient
        waiter: WorkspaceActiveWaiter = client.get_waiter("workspace_active")
        await waiter.wait()
    ```
