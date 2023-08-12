# ManagedBlockchainQuery module

> [Index](../README.md) > ManagedBlockchainQuery


!!! note ""

    Auto-generated documentation for [ManagedBlockchainQuery](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain-query.html#ManagedBlockchainQuery)
    type annotations stubs module [types-aiobotocore-managedblockchain-query](https://pypi.org/project/types-aiobotocore-managedblockchain-query/).

## How to install



### From PyPI with pip

Install `types-aiobotocore` for `ManagedBlockchainQuery` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[managedblockchain-query]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[managedblockchain-query]'


# standalone installation
python -m pip install types-aiobotocore-managedblockchain-query
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-managedblockchain-query
```

## Usage

Code samples can be found in [Examples](./usage.md).

## ManagedBlockchainQueryClient

Type annotations and code completion for  `#!python session.create_client("managedblockchain-query")` as [ManagedBlockchainQueryClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain-query.html#ManagedBlockchainQuery.Client)

```python
# ManagedBlockchainQueryClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_managedblockchain_query.client import ManagedBlockchainQueryClient


session = get_session()
async with session.create_client("managedblockchain-query") as client:
    client: ManagedBlockchainQueryClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("managedblockchain-query").get_paginator("...")`.

```python
# ListTokenBalancesPaginator usage example

from types_aiobotocore_managedblockchain_query.paginator import ListTokenBalancesPaginator

def get_list_token_balances_paginator() -> ListTokenBalancesPaginator:
    return client.get_paginator("list_token_balances"))
```

- [ListTokenBalancesPaginator](./paginators.md#listtokenbalancespaginator)
- [ListTransactionEventsPaginator](./paginators.md#listtransactioneventspaginator)
- [ListTransactionsPaginator](./paginators.md#listtransactionspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# ErrorTypeType usage example

from types_aiobotocore_managedblockchain_query.literals import ErrorTypeType

def get_value() -> ErrorTypeType:
    return "RESOURCE_NOT_FOUND_EXCEPTION"
```

- [ErrorTypeType](./literals.md#errortypetype)
- [ListTokenBalancesPaginatorName](./literals.md#listtokenbalancespaginatorname)
- [ListTransactionEventsPaginatorName](./literals.md#listtransactioneventspaginatorname)
- [ListTransactionsPaginatorName](./literals.md#listtransactionspaginatorname)
- [ListTransactionsSortByType](./literals.md#listtransactionssortbytype)
- [QueryNetworkType](./literals.md#querynetworktype)
- [QueryTransactionEventTypeType](./literals.md#querytransactioneventtypetype)
- [QueryTransactionStatusType](./literals.md#querytransactionstatustype)
- [SortOrderType](./literals.md#sortordertype)
- [ManagedBlockchainQueryServiceName](./literals.md#managedblockchainqueryservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [OwnerIdentifierTypeDef](./type_defs.md#owneridentifiertypedef)
- [TokenIdentifierTypeDef](./type_defs.md#tokenidentifiertypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [TimestampTypeDef](./type_defs.md#timestamptypedef)
- [GetTransactionInputRequestTypeDef](./type_defs.md#gettransactioninputrequesttypedef)
- [TransactionTypeDef](./type_defs.md#transactiontypedef)
- [OwnerFilterTypeDef](./type_defs.md#ownerfiltertypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [TokenFilterTypeDef](./type_defs.md#tokenfiltertypedef)
- [ListTransactionEventsInputRequestTypeDef](./type_defs.md#listtransactioneventsinputrequesttypedef)
- [TransactionEventTypeDef](./type_defs.md#transactioneventtypedef)
- [ListTransactionsSortTypeDef](./type_defs.md#listtransactionssorttypedef)
- [TransactionOutputItemTypeDef](./type_defs.md#transactionoutputitemtypedef)
- [BlockchainInstantTypeDef](./type_defs.md#blockchaininstanttypedef)
- [GetTransactionOutputTypeDef](./type_defs.md#gettransactionoutputtypedef)
- [ListTransactionEventsInputListTransactionEventsPaginateTypeDef](./type_defs.md#listtransactioneventsinputlisttransactioneventspaginatetypedef)
- [ListTokenBalancesInputListTokenBalancesPaginateTypeDef](./type_defs.md#listtokenbalancesinputlisttokenbalancespaginatetypedef)
- [ListTokenBalancesInputRequestTypeDef](./type_defs.md#listtokenbalancesinputrequesttypedef)
- [ListTransactionEventsOutputTypeDef](./type_defs.md#listtransactioneventsoutputtypedef)
- [ListTransactionsOutputTypeDef](./type_defs.md#listtransactionsoutputtypedef)
- [BatchGetTokenBalanceErrorItemTypeDef](./type_defs.md#batchgettokenbalanceerroritemtypedef)
- [BatchGetTokenBalanceInputItemTypeDef](./type_defs.md#batchgettokenbalanceinputitemtypedef)
- [BatchGetTokenBalanceOutputItemTypeDef](./type_defs.md#batchgettokenbalanceoutputitemtypedef)
- [GetTokenBalanceInputRequestTypeDef](./type_defs.md#gettokenbalanceinputrequesttypedef)
- [GetTokenBalanceOutputTypeDef](./type_defs.md#gettokenbalanceoutputtypedef)
- [ListTransactionsInputListTransactionsPaginateTypeDef](./type_defs.md#listtransactionsinputlisttransactionspaginatetypedef)
- [ListTransactionsInputRequestTypeDef](./type_defs.md#listtransactionsinputrequesttypedef)
- [TokenBalanceTypeDef](./type_defs.md#tokenbalancetypedef)
- [BatchGetTokenBalanceInputRequestTypeDef](./type_defs.md#batchgettokenbalanceinputrequesttypedef)
- [BatchGetTokenBalanceOutputTypeDef](./type_defs.md#batchgettokenbalanceoutputtypedef)
- [ListTokenBalancesOutputTypeDef](./type_defs.md#listtokenbalancesoutputtypedef)

