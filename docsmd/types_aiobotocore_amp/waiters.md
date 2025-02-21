# Waiters

> [Index](../README.md) > [PrometheusService](./README.md) > Waiters

!!! note ""

    Auto-generated documentation for [PrometheusService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#prometheusservice)
    type annotations stubs module [types-aiobotocore-amp](https://pypi.org/project/types-aiobotocore-amp/).

## ScraperActiveWaiter

Type annotations and code completion for `#!python session.create_client("amp").get_waiter("scraper_active")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp/waiter/ScraperActive.html#PrometheusService.Waiter.ScraperActive)

```python
# ScraperActiveWaiter usage example

from aiobotocore.session import Session

from types_aiobotocore_amp.waiter import ScraperActiveWaiter

session = get_session()
async with session.create_client("amp") as client:  # (1)
    waiter: ScraperActiveWaiter = client.get_waiter("scraper_active")  # (2)
    await waiter.wait()
```

1. client: [PrometheusServiceClient](./client.md)
2. waiter: [ScraperActiveWaiter](./waiters.md#scraperactivewaiter)


### wait

Type annotations and code completion for `#!python ScraperActiveWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    scraperId: str,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: DescribeScraperRequestWaitTypeDef = {  # (1)
    "scraperId": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: DescribeScraperRequestWaitTypeDef](./type_defs.md#describescraperrequestwaittypedef) 
## ScraperDeletedWaiter

Type annotations and code completion for `#!python session.create_client("amp").get_waiter("scraper_deleted")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp/waiter/ScraperDeleted.html#PrometheusService.Waiter.ScraperDeleted)

```python
# ScraperDeletedWaiter usage example

from aiobotocore.session import Session

from types_aiobotocore_amp.waiter import ScraperDeletedWaiter

session = get_session()
async with session.create_client("amp") as client:  # (1)
    waiter: ScraperDeletedWaiter = client.get_waiter("scraper_deleted")  # (2)
    await waiter.wait()
```

1. client: [PrometheusServiceClient](./client.md)
2. waiter: [ScraperDeletedWaiter](./waiters.md#scraperdeletedwaiter)


### wait

Type annotations and code completion for `#!python ScraperDeletedWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    scraperId: str,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: DescribeScraperRequestWaitExtraTypeDef = {  # (1)
    "scraperId": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: DescribeScraperRequestWaitExtraTypeDef](./type_defs.md#describescraperrequestwaitextratypedef) 
## WorkspaceActiveWaiter

Type annotations and code completion for `#!python session.create_client("amp").get_waiter("workspace_active")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp/waiter/WorkspaceActive.html#PrometheusService.Waiter.WorkspaceActive)

```python
# WorkspaceActiveWaiter usage example

from aiobotocore.session import Session

from types_aiobotocore_amp.waiter import WorkspaceActiveWaiter

session = get_session()
async with session.create_client("amp") as client:  # (1)
    waiter: WorkspaceActiveWaiter = client.get_waiter("workspace_active")  # (2)
    await waiter.wait()
```

1. client: [PrometheusServiceClient](./client.md)
2. waiter: [WorkspaceActiveWaiter](./waiters.md#workspaceactivewaiter)


### wait

Type annotations and code completion for `#!python WorkspaceActiveWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    workspaceId: str,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: DescribeWorkspaceRequestWaitTypeDef = {  # (1)
    "workspaceId": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: DescribeWorkspaceRequestWaitTypeDef](./type_defs.md#describeworkspacerequestwaittypedef) 
## WorkspaceDeletedWaiter

Type annotations and code completion for `#!python session.create_client("amp").get_waiter("workspace_deleted")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp/waiter/WorkspaceDeleted.html#PrometheusService.Waiter.WorkspaceDeleted)

```python
# WorkspaceDeletedWaiter usage example

from aiobotocore.session import Session

from types_aiobotocore_amp.waiter import WorkspaceDeletedWaiter

session = get_session()
async with session.create_client("amp") as client:  # (1)
    waiter: WorkspaceDeletedWaiter = client.get_waiter("workspace_deleted")  # (2)
    await waiter.wait()
```

1. client: [PrometheusServiceClient](./client.md)
2. waiter: [WorkspaceDeletedWaiter](./waiters.md#workspacedeletedwaiter)


### wait

Type annotations and code completion for `#!python WorkspaceDeletedWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    workspaceId: str,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: DescribeWorkspaceRequestWaitExtraTypeDef = {  # (1)
    "workspaceId": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: DescribeWorkspaceRequestWaitExtraTypeDef](./type_defs.md#describeworkspacerequestwaitextratypedef) 
