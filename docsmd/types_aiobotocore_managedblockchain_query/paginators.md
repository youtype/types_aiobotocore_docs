# Paginators

> [Index](../README.md) > [ManagedBlockchainQuery](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [ManagedBlockchainQuery](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain-query.html#managedblockchainquery)
    type annotations stubs module [types-aiobotocore-managedblockchain-query](https://pypi.org/project/types-aiobotocore-managedblockchain-query/).

## ListAssetContractsPaginator

Type annotations and code completion for `#!python session.create_client("managedblockchain-query").get_paginator("list_asset_contracts")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain-query/paginator/ListAssetContracts.html#ManagedBlockchainQuery.Paginator.ListAssetContracts)

```python
# ListAssetContractsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_managedblockchain_query.paginator import ListAssetContractsPaginator

session = get_session()
async with session.create_client("managedblockchain-query") as client:  # (1)
    paginator: ListAssetContractsPaginator = client.get_paginator("list_asset_contracts")  # (2)
    async for item in paginator.paginate(...):
        item: ListAssetContractsOutputTypeDef
        print(item)  # (3)
```

1. client: [ManagedBlockchainQueryClient](./client.md)
2. paginator: [ListAssetContractsPaginator](./paginators.md#listassetcontractspaginator)
3. item: [:material-code-braces: ListAssetContractsOutputTypeDef](./type_defs.md#listassetcontractsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListAssetContractsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    contractFilter: ContractFilterTypeDef,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListAssetContractsOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: ContractFilterTypeDef](./type_defs.md#contractfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListAssetContractsOutputTypeDef](./type_defs.md#listassetcontractsoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListAssetContractsInputPaginateTypeDef = {  # (1)
    "contractFilter": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAssetContractsInputPaginateTypeDef](./type_defs.md#listassetcontractsinputpaginatetypedef) 
## ListFilteredTransactionEventsPaginator

Type annotations and code completion for `#!python session.create_client("managedblockchain-query").get_paginator("list_filtered_transaction_events")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain-query/paginator/ListFilteredTransactionEvents.html#ManagedBlockchainQuery.Paginator.ListFilteredTransactionEvents)

```python
# ListFilteredTransactionEventsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_managedblockchain_query.paginator import ListFilteredTransactionEventsPaginator

session = get_session()
async with session.create_client("managedblockchain-query") as client:  # (1)
    paginator: ListFilteredTransactionEventsPaginator = client.get_paginator("list_filtered_transaction_events")  # (2)
    async for item in paginator.paginate(...):
        item: ListFilteredTransactionEventsOutputTypeDef
        print(item)  # (3)
```

1. client: [ManagedBlockchainQueryClient](./client.md)
2. paginator: [ListFilteredTransactionEventsPaginator](./paginators.md#listfilteredtransactioneventspaginator)
3. item: [:material-code-braces: ListFilteredTransactionEventsOutputTypeDef](./type_defs.md#listfilteredtransactioneventsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListFilteredTransactionEventsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    network: str,
    addressIdentifierFilter: AddressIdentifierFilterTypeDef,  # (1)
    timeFilter: TimeFilterTypeDef = ...,  # (2)
    voutFilter: VoutFilterTypeDef = ...,  # (3)
    confirmationStatusFilter: ConfirmationStatusFilterTypeDef = ...,  # (4)
    sort: ListFilteredTransactionEventsSortTypeDef = ...,  # (5)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (6)
) -> AioPageIterator[ListFilteredTransactionEventsOutputTypeDef]:  # (7)
    ...
```

1. See [:material-code-braces: AddressIdentifierFilterTypeDef](./type_defs.md#addressidentifierfiltertypedef) 
2. See [:material-code-braces: TimeFilterTypeDef](./type_defs.md#timefiltertypedef) 
3. See [:material-code-braces: VoutFilterTypeDef](./type_defs.md#voutfiltertypedef) 
4. See [:material-code-braces: ConfirmationStatusFilterTypeDef](./type_defs.md#confirmationstatusfiltertypedef) 
5. See [:material-code-braces: ListFilteredTransactionEventsSortTypeDef](./type_defs.md#listfilteredtransactioneventssorttypedef) 
6. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
7. See [:material-code-braces: ListFilteredTransactionEventsOutputTypeDef](./type_defs.md#listfilteredtransactioneventsoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListFilteredTransactionEventsInputPaginateTypeDef = {  # (1)
    "network": ...,
    "addressIdentifierFilter": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListFilteredTransactionEventsInputPaginateTypeDef](./type_defs.md#listfilteredtransactioneventsinputpaginatetypedef) 
## ListTokenBalancesPaginator

Type annotations and code completion for `#!python session.create_client("managedblockchain-query").get_paginator("list_token_balances")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain-query/paginator/ListTokenBalances.html#ManagedBlockchainQuery.Paginator.ListTokenBalances)

```python
# ListTokenBalancesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_managedblockchain_query.paginator import ListTokenBalancesPaginator

session = get_session()
async with session.create_client("managedblockchain-query") as client:  # (1)
    paginator: ListTokenBalancesPaginator = client.get_paginator("list_token_balances")  # (2)
    async for item in paginator.paginate(...):
        item: ListTokenBalancesOutputTypeDef
        print(item)  # (3)
```

1. client: [ManagedBlockchainQueryClient](./client.md)
2. paginator: [ListTokenBalancesPaginator](./paginators.md#listtokenbalancespaginator)
3. item: [:material-code-braces: ListTokenBalancesOutputTypeDef](./type_defs.md#listtokenbalancesoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListTokenBalancesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    tokenFilter: TokenFilterTypeDef,  # (1)
    ownerFilter: OwnerFilterTypeDef = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AioPageIterator[ListTokenBalancesOutputTypeDef]:  # (4)
    ...
```

1. See [:material-code-braces: TokenFilterTypeDef](./type_defs.md#tokenfiltertypedef) 
2. See [:material-code-braces: OwnerFilterTypeDef](./type_defs.md#ownerfiltertypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: ListTokenBalancesOutputTypeDef](./type_defs.md#listtokenbalancesoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListTokenBalancesInputPaginateTypeDef = {  # (1)
    "tokenFilter": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTokenBalancesInputPaginateTypeDef](./type_defs.md#listtokenbalancesinputpaginatetypedef) 
## ListTransactionEventsPaginator

Type annotations and code completion for `#!python session.create_client("managedblockchain-query").get_paginator("list_transaction_events")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain-query/paginator/ListTransactionEvents.html#ManagedBlockchainQuery.Paginator.ListTransactionEvents)

```python
# ListTransactionEventsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_managedblockchain_query.paginator import ListTransactionEventsPaginator

session = get_session()
async with session.create_client("managedblockchain-query") as client:  # (1)
    paginator: ListTransactionEventsPaginator = client.get_paginator("list_transaction_events")  # (2)
    async for item in paginator.paginate(...):
        item: ListTransactionEventsOutputTypeDef
        print(item)  # (3)
```

1. client: [ManagedBlockchainQueryClient](./client.md)
2. paginator: [ListTransactionEventsPaginator](./paginators.md#listtransactioneventspaginator)
3. item: [:material-code-braces: ListTransactionEventsOutputTypeDef](./type_defs.md#listtransactioneventsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListTransactionEventsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    network: QueryNetworkType,  # (1)
    transactionHash: str = ...,
    transactionId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListTransactionEventsOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: QueryNetworkType](./literals.md#querynetworktype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListTransactionEventsOutputTypeDef](./type_defs.md#listtransactioneventsoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListTransactionEventsInputPaginateTypeDef = {  # (1)
    "network": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTransactionEventsInputPaginateTypeDef](./type_defs.md#listtransactioneventsinputpaginatetypedef) 
## ListTransactionsPaginator

Type annotations and code completion for `#!python session.create_client("managedblockchain-query").get_paginator("list_transactions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain-query/paginator/ListTransactions.html#ManagedBlockchainQuery.Paginator.ListTransactions)

```python
# ListTransactionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_managedblockchain_query.paginator import ListTransactionsPaginator

session = get_session()
async with session.create_client("managedblockchain-query") as client:  # (1)
    paginator: ListTransactionsPaginator = client.get_paginator("list_transactions")  # (2)
    async for item in paginator.paginate(...):
        item: ListTransactionsOutputTypeDef
        print(item)  # (3)
```

1. client: [ManagedBlockchainQueryClient](./client.md)
2. paginator: [ListTransactionsPaginator](./paginators.md#listtransactionspaginator)
3. item: [:material-code-braces: ListTransactionsOutputTypeDef](./type_defs.md#listtransactionsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListTransactionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    address: str,
    network: QueryNetworkType,  # (1)
    fromBlockchainInstant: BlockchainInstantUnionTypeDef = ...,  # (2)
    toBlockchainInstant: BlockchainInstantUnionTypeDef = ...,  # (2)
    sort: ListTransactionsSortTypeDef = ...,  # (4)
    confirmationStatusFilter: ConfirmationStatusFilterTypeDef = ...,  # (5)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (6)
) -> AioPageIterator[ListTransactionsOutputTypeDef]:  # (7)
    ...
```

1. See [:material-code-brackets: QueryNetworkType](./literals.md#querynetworktype) 
2. See [:material-code-braces: BlockchainInstantTypeDef](./type_defs.md#blockchaininstanttypedef) [:material-code-braces: BlockchainInstantOutputTypeDef](./type_defs.md#blockchaininstantoutputtypedef) 
3. See [:material-code-braces: BlockchainInstantTypeDef](./type_defs.md#blockchaininstanttypedef) [:material-code-braces: BlockchainInstantOutputTypeDef](./type_defs.md#blockchaininstantoutputtypedef) 
4. See [:material-code-braces: ListTransactionsSortTypeDef](./type_defs.md#listtransactionssorttypedef) 
5. See [:material-code-braces: ConfirmationStatusFilterTypeDef](./type_defs.md#confirmationstatusfiltertypedef) 
6. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
7. See [:material-code-braces: ListTransactionsOutputTypeDef](./type_defs.md#listtransactionsoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListTransactionsInputPaginateTypeDef = {  # (1)
    "address": ...,
    "network": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTransactionsInputPaginateTypeDef](./type_defs.md#listtransactionsinputpaginatetypedef) 
