# ManagedBlockchainQueryClient

> [Index](../README.md) > [ManagedBlockchainQuery](./README.md) > ManagedBlockchainQueryClient

!!! note ""

    Auto-generated documentation for [ManagedBlockchainQuery](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain-query.html#ManagedBlockchainQuery)
    type annotations stubs module [types-aiobotocore-managedblockchain-query](https://pypi.org/project/types-aiobotocore-managedblockchain-query/).

## ManagedBlockchainQueryClient

Type annotations and code completion for `#!python session.create_client("managedblockchain-query")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain-query.html#ManagedBlockchainQuery.Client)

```python
ManagedBlockchainQueryClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_managedblockchain_query.client import ManagedBlockchainQueryClient

session = get_session()
async with session.create_client("managedblockchain-query") as client:
    client: ManagedBlockchainQueryClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("managedblockchain-query").exceptions` structure.

```python
ManagedBlockchainQueryClient.exceptions usage example

async with session.create_client("managedblockchain-query") as client:
    try:
        do_something(client)
    except (
            client.AccessDeniedException,
        client.ClientError,
        client.InternalServerException,
        client.ResourceNotFoundException,
        client.ServiceQuotaExceededException,
        client.ThrottlingException,
        client.ValidationException,
    ) as e:
        print(e)
```

```python
ManagedBlockchainQueryClient usage type checking example

from types_aiobotocore_managedblockchain_query.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### batch\_get\_token\_balance

Gets the token balance for a batch of tokens by using the `GetTokenBalance`
action for every token in the request.

Type annotations and code completion for `#!python session.create_client("managedblockchain-query").batch_get_token_balance` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain-query.html#ManagedBlockchainQuery.Client.batch_get_token_balance)

```python
# batch_get_token_balance method definition

await def batch_get_token_balance(
    self,
    *,
    getTokenBalanceInputs: Sequence[BatchGetTokenBalanceInputItemTypeDef] = ...,  # (1)
) -> BatchGetTokenBalanceOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: BatchGetTokenBalanceInputItemTypeDef](./type_defs.md#batchgettokenbalanceinputitemtypedef) 
2. See [:material-code-braces: BatchGetTokenBalanceOutputTypeDef](./type_defs.md#batchgettokenbalanceoutputtypedef) 


```python
# batch_get_token_balance method usage example with argument unpacking

kwargs: BatchGetTokenBalanceInputRequestTypeDef = {  # (1)
    "getTokenBalanceInputs": ...,
}

parent.batch_get_token_balance(**kwargs)
```

1. See [:material-code-braces: BatchGetTokenBalanceInputRequestTypeDef](./type_defs.md#batchgettokenbalanceinputrequesttypedef) 

### can\_paginate

Check if an operation can be paginated.

Type annotations and code completion for `#!python session.create_client("managedblockchain-query").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain-query.html#ManagedBlockchainQuery.Client.can_paginate)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### close

Closes underlying endpoint connections.

Type annotations and code completion for `#!python session.create_client("managedblockchain-query").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain-query.html#ManagedBlockchainQuery.Client.close)

```python
# close method definition

await def close(
    self,
) -> None:
    ...
```


### generate\_presigned\_url

Generate a presigned url given a client, its method, and arguments.

Type annotations and code completion for `#!python session.create_client("managedblockchain-query").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain-query.html#ManagedBlockchainQuery.Client.generate_presigned_url)

```python
# generate_presigned_url method definition

await def generate_presigned_url(
    self,
    ClientMethod: str,
    Params: Mapping[str, Any] = ...,
    ExpiresIn: int = 3600,
    HttpMethod: str = ...,
) -> str:
    ...
```


### get\_token\_balance

Gets the balance of a specific token, including native tokens, for a given
address (wallet or contract) on the blockchain.

Type annotations and code completion for `#!python session.create_client("managedblockchain-query").get_token_balance` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain-query.html#ManagedBlockchainQuery.Client.get_token_balance)

```python
# get_token_balance method definition

await def get_token_balance(
    self,
    *,
    tokenIdentifier: TokenIdentifierTypeDef,  # (1)
    ownerIdentifier: OwnerIdentifierTypeDef,  # (2)
    atBlockchainInstant: BlockchainInstantTypeDef = ...,  # (3)
) -> GetTokenBalanceOutputTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: TokenIdentifierTypeDef](./type_defs.md#tokenidentifiertypedef) 
2. See [:material-code-braces: OwnerIdentifierTypeDef](./type_defs.md#owneridentifiertypedef) 
3. See [:material-code-braces: BlockchainInstantTypeDef](./type_defs.md#blockchaininstanttypedef) 
4. See [:material-code-braces: GetTokenBalanceOutputTypeDef](./type_defs.md#gettokenbalanceoutputtypedef) 


```python
# get_token_balance method usage example with argument unpacking

kwargs: GetTokenBalanceInputRequestTypeDef = {  # (1)
    "tokenIdentifier": ...,
    "ownerIdentifier": ...,
}

parent.get_token_balance(**kwargs)
```

1. See [:material-code-braces: GetTokenBalanceInputRequestTypeDef](./type_defs.md#gettokenbalanceinputrequesttypedef) 

### get\_transaction

Get the details of a transaction.

Type annotations and code completion for `#!python session.create_client("managedblockchain-query").get_transaction` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain-query.html#ManagedBlockchainQuery.Client.get_transaction)

```python
# get_transaction method definition

await def get_transaction(
    self,
    *,
    transactionHash: str,
    network: QueryNetworkType,  # (1)
) -> GetTransactionOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: QueryNetworkType](./literals.md#querynetworktype) 
2. See [:material-code-braces: GetTransactionOutputTypeDef](./type_defs.md#gettransactionoutputtypedef) 


```python
# get_transaction method usage example with argument unpacking

kwargs: GetTransactionInputRequestTypeDef = {  # (1)
    "transactionHash": ...,
    "network": ...,
}

parent.get_transaction(**kwargs)
```

1. See [:material-code-braces: GetTransactionInputRequestTypeDef](./type_defs.md#gettransactioninputrequesttypedef) 

### list\_token\_balances

This action returns the following for a given a blockchain network: * Lists all
token balances owned by an address (either a contact address or a wallet
address).

Type annotations and code completion for `#!python session.create_client("managedblockchain-query").list_token_balances` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain-query.html#ManagedBlockchainQuery.Client.list_token_balances)

```python
# list_token_balances method definition

await def list_token_balances(
    self,
    *,
    tokenFilter: TokenFilterTypeDef,  # (1)
    ownerFilter: OwnerFilterTypeDef = ...,  # (2)
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListTokenBalancesOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: TokenFilterTypeDef](./type_defs.md#tokenfiltertypedef) 
2. See [:material-code-braces: OwnerFilterTypeDef](./type_defs.md#ownerfiltertypedef) 
3. See [:material-code-braces: ListTokenBalancesOutputTypeDef](./type_defs.md#listtokenbalancesoutputtypedef) 


```python
# list_token_balances method usage example with argument unpacking

kwargs: ListTokenBalancesInputRequestTypeDef = {  # (1)
    "tokenFilter": ...,
}

parent.list_token_balances(**kwargs)
```

1. See [:material-code-braces: ListTokenBalancesInputRequestTypeDef](./type_defs.md#listtokenbalancesinputrequesttypedef) 

### list\_transaction\_events

An array of `TransactionEvent` objects.

Type annotations and code completion for `#!python session.create_client("managedblockchain-query").list_transaction_events` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain-query.html#ManagedBlockchainQuery.Client.list_transaction_events)

```python
# list_transaction_events method definition

await def list_transaction_events(
    self,
    *,
    transactionHash: str,
    network: QueryNetworkType,  # (1)
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListTransactionEventsOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: QueryNetworkType](./literals.md#querynetworktype) 
2. See [:material-code-braces: ListTransactionEventsOutputTypeDef](./type_defs.md#listtransactioneventsoutputtypedef) 


```python
# list_transaction_events method usage example with argument unpacking

kwargs: ListTransactionEventsInputRequestTypeDef = {  # (1)
    "transactionHash": ...,
    "network": ...,
}

parent.list_transaction_events(**kwargs)
```

1. See [:material-code-braces: ListTransactionEventsInputRequestTypeDef](./type_defs.md#listtransactioneventsinputrequesttypedef) 

### list\_transactions

Lists all of the transactions on a given wallet address or to a specific
contract.

Type annotations and code completion for `#!python session.create_client("managedblockchain-query").list_transactions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain-query.html#ManagedBlockchainQuery.Client.list_transactions)

```python
# list_transactions method definition

await def list_transactions(
    self,
    *,
    address: str,
    network: QueryNetworkType,  # (1)
    fromBlockchainInstant: BlockchainInstantTypeDef = ...,  # (2)
    toBlockchainInstant: BlockchainInstantTypeDef = ...,  # (2)
    sort: ListTransactionsSortTypeDef = ...,  # (4)
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListTransactionsOutputTypeDef:  # (5)
    ...
```

1. See [:material-code-brackets: QueryNetworkType](./literals.md#querynetworktype) 
2. See [:material-code-braces: BlockchainInstantTypeDef](./type_defs.md#blockchaininstanttypedef) 
3. See [:material-code-braces: BlockchainInstantTypeDef](./type_defs.md#blockchaininstanttypedef) 
4. See [:material-code-braces: ListTransactionsSortTypeDef](./type_defs.md#listtransactionssorttypedef) 
5. See [:material-code-braces: ListTransactionsOutputTypeDef](./type_defs.md#listtransactionsoutputtypedef) 


```python
# list_transactions method usage example with argument unpacking

kwargs: ListTransactionsInputRequestTypeDef = {  # (1)
    "address": ...,
    "network": ...,
}

parent.list_transactions(**kwargs)
```

1. See [:material-code-braces: ListTransactionsInputRequestTypeDef](./type_defs.md#listtransactionsinputrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("managedblockchain-query").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain-query.html#ManagedBlockchainQuery.Client.__aenter__)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> ManagedBlockchainQueryClient:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("managedblockchain-query").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain-query.html#ManagedBlockchainQuery.Client.__aexit__)

```python
# __aexit__ method definition

await def __aexit__(
    self,
    exc_type: Any,
    exc_val: Any,
    exc_tb: Any,
) -> Any:
    ...
```




### get_paginator

Type annotations and code completion for `#!python session.create_client("managedblockchain-query").get_paginator` method with overloads.

- `client.get_paginator("list_token_balances")` -> [ListTokenBalancesPaginator](./paginators.md#listtokenbalancespaginator)
- `client.get_paginator("list_transaction_events")` -> [ListTransactionEventsPaginator](./paginators.md#listtransactioneventspaginator)
- `client.get_paginator("list_transactions")` -> [ListTransactionsPaginator](./paginators.md#listtransactionspaginator)



