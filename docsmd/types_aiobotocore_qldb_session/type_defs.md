# Type definitions

> [Index](../README.md) > [QLDBSession](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [QLDBSession](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb-session.html#qldbsession)
    type annotations stubs module [types-aiobotocore-qldb-session](https://pypi.org/project/types-aiobotocore-qldb-session/).

## BlobTypeDef

```python
# BlobTypeDef Union usage example

from types_aiobotocore_qldb_session.type_defs import BlobTypeDef


def get_value() -> BlobTypeDef:
    return ...


# BlobTypeDef definition

BlobTypeDef = Union[
    str,
    bytes,
    IO[Any],
    StreamingBody,
]
```


## ValueHolderUnionTypeDef

```python
# ValueHolderUnionTypeDef Union usage example

from types_aiobotocore_qldb_session.type_defs import ValueHolderUnionTypeDef


def get_value() -> ValueHolderUnionTypeDef:
    return ...


# ValueHolderUnionTypeDef definition

ValueHolderUnionTypeDef = Union[
    ValueHolderTypeDef,  # (1)
    ValueHolderOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ValueHolderTypeDef](./type_defs.md#valueholdertypedef) 
2. See [:material-code-braces: ValueHolderOutputTypeDef](./type_defs.md#valueholderoutputtypedef) 



## TimingInformationTypeDef

```python
# TimingInformationTypeDef TypedDict usage example

from types_aiobotocore_qldb_session.type_defs import TimingInformationTypeDef


def get_value() -> TimingInformationTypeDef:
    return {
        "ProcessingTimeMilliseconds": ...,
    }


# TimingInformationTypeDef definition

class TimingInformationTypeDef(TypedDict):
    ProcessingTimeMilliseconds: NotRequired[int],
```

## IOUsageTypeDef

```python
# IOUsageTypeDef TypedDict usage example

from types_aiobotocore_qldb_session.type_defs import IOUsageTypeDef


def get_value() -> IOUsageTypeDef:
    return {
        "ReadIOs": ...,
    }


# IOUsageTypeDef definition

class IOUsageTypeDef(TypedDict):
    ReadIOs: NotRequired[int],
    WriteIOs: NotRequired[int],
```

## FetchPageRequestTypeDef

```python
# FetchPageRequestTypeDef TypedDict usage example

from types_aiobotocore_qldb_session.type_defs import FetchPageRequestTypeDef


def get_value() -> FetchPageRequestTypeDef:
    return {
        "TransactionId": ...,
    }


# FetchPageRequestTypeDef definition

class FetchPageRequestTypeDef(TypedDict):
    TransactionId: str,
    NextPageToken: str,
```

## ValueHolderOutputTypeDef

```python
# ValueHolderOutputTypeDef TypedDict usage example

from types_aiobotocore_qldb_session.type_defs import ValueHolderOutputTypeDef


def get_value() -> ValueHolderOutputTypeDef:
    return {
        "IonBinary": ...,
    }


# ValueHolderOutputTypeDef definition

class ValueHolderOutputTypeDef(TypedDict):
    IonBinary: NotRequired[bytes],
    IonText: NotRequired[str],
```

## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_qldb_session.type_defs import ResponseMetadataTypeDef


def get_value() -> ResponseMetadataTypeDef:
    return {
        "RequestId": ...,
    }


# ResponseMetadataTypeDef definition

class ResponseMetadataTypeDef(TypedDict):
    RequestId: str,
    HTTPStatusCode: int,
    HTTPHeaders: Dict[str, str],
    RetryAttempts: int,
    HostId: NotRequired[str],
```

## StartSessionRequestTypeDef

```python
# StartSessionRequestTypeDef TypedDict usage example

from types_aiobotocore_qldb_session.type_defs import StartSessionRequestTypeDef


def get_value() -> StartSessionRequestTypeDef:
    return {
        "LedgerName": ...,
    }


# StartSessionRequestTypeDef definition

class StartSessionRequestTypeDef(TypedDict):
    LedgerName: str,
```

## AbortTransactionResultTypeDef

```python
# AbortTransactionResultTypeDef TypedDict usage example

from types_aiobotocore_qldb_session.type_defs import AbortTransactionResultTypeDef


def get_value() -> AbortTransactionResultTypeDef:
    return {
        "TimingInformation": ...,
    }


# AbortTransactionResultTypeDef definition

class AbortTransactionResultTypeDef(TypedDict):
    TimingInformation: NotRequired[TimingInformationTypeDef],  # (1)
```

1. See [:material-code-braces: TimingInformationTypeDef](./type_defs.md#timinginformationtypedef) 
## EndSessionResultTypeDef

```python
# EndSessionResultTypeDef TypedDict usage example

from types_aiobotocore_qldb_session.type_defs import EndSessionResultTypeDef


def get_value() -> EndSessionResultTypeDef:
    return {
        "TimingInformation": ...,
    }


# EndSessionResultTypeDef definition

class EndSessionResultTypeDef(TypedDict):
    TimingInformation: NotRequired[TimingInformationTypeDef],  # (1)
```

1. See [:material-code-braces: TimingInformationTypeDef](./type_defs.md#timinginformationtypedef) 
## StartSessionResultTypeDef

```python
# StartSessionResultTypeDef TypedDict usage example

from types_aiobotocore_qldb_session.type_defs import StartSessionResultTypeDef


def get_value() -> StartSessionResultTypeDef:
    return {
        "SessionToken": ...,
    }


# StartSessionResultTypeDef definition

class StartSessionResultTypeDef(TypedDict):
    SessionToken: NotRequired[str],
    TimingInformation: NotRequired[TimingInformationTypeDef],  # (1)
```

1. See [:material-code-braces: TimingInformationTypeDef](./type_defs.md#timinginformationtypedef) 
## StartTransactionResultTypeDef

```python
# StartTransactionResultTypeDef TypedDict usage example

from types_aiobotocore_qldb_session.type_defs import StartTransactionResultTypeDef


def get_value() -> StartTransactionResultTypeDef:
    return {
        "TransactionId": ...,
    }


# StartTransactionResultTypeDef definition

class StartTransactionResultTypeDef(TypedDict):
    TransactionId: NotRequired[str],
    TimingInformation: NotRequired[TimingInformationTypeDef],  # (1)
```

1. See [:material-code-braces: TimingInformationTypeDef](./type_defs.md#timinginformationtypedef) 
## CommitTransactionRequestTypeDef

```python
# CommitTransactionRequestTypeDef TypedDict usage example

from types_aiobotocore_qldb_session.type_defs import CommitTransactionRequestTypeDef


def get_value() -> CommitTransactionRequestTypeDef:
    return {
        "TransactionId": ...,
    }


# CommitTransactionRequestTypeDef definition

class CommitTransactionRequestTypeDef(TypedDict):
    TransactionId: str,
    CommitDigest: BlobTypeDef,
```

## ValueHolderTypeDef

```python
# ValueHolderTypeDef TypedDict usage example

from types_aiobotocore_qldb_session.type_defs import ValueHolderTypeDef


def get_value() -> ValueHolderTypeDef:
    return {
        "IonBinary": ...,
    }


# ValueHolderTypeDef definition

class ValueHolderTypeDef(TypedDict):
    IonBinary: NotRequired[BlobTypeDef],
    IonText: NotRequired[str],
```

## CommitTransactionResultTypeDef

```python
# CommitTransactionResultTypeDef TypedDict usage example

from types_aiobotocore_qldb_session.type_defs import CommitTransactionResultTypeDef


def get_value() -> CommitTransactionResultTypeDef:
    return {
        "TransactionId": ...,
    }


# CommitTransactionResultTypeDef definition

class CommitTransactionResultTypeDef(TypedDict):
    TransactionId: NotRequired[str],
    CommitDigest: NotRequired[bytes],
    TimingInformation: NotRequired[TimingInformationTypeDef],  # (1)
    ConsumedIOs: NotRequired[IOUsageTypeDef],  # (2)
```

1. See [:material-code-braces: TimingInformationTypeDef](./type_defs.md#timinginformationtypedef) 
2. See [:material-code-braces: IOUsageTypeDef](./type_defs.md#iousagetypedef) 
## PageTypeDef

```python
# PageTypeDef TypedDict usage example

from types_aiobotocore_qldb_session.type_defs import PageTypeDef


def get_value() -> PageTypeDef:
    return {
        "Values": ...,
    }


# PageTypeDef definition

class PageTypeDef(TypedDict):
    Values: NotRequired[List[ValueHolderOutputTypeDef]],  # (1)
    NextPageToken: NotRequired[str],
```

1. See [:material-code-braces: ValueHolderOutputTypeDef](./type_defs.md#valueholderoutputtypedef) 
## ExecuteStatementResultTypeDef

```python
# ExecuteStatementResultTypeDef TypedDict usage example

from types_aiobotocore_qldb_session.type_defs import ExecuteStatementResultTypeDef


def get_value() -> ExecuteStatementResultTypeDef:
    return {
        "FirstPage": ...,
    }


# ExecuteStatementResultTypeDef definition

class ExecuteStatementResultTypeDef(TypedDict):
    FirstPage: NotRequired[PageTypeDef],  # (1)
    TimingInformation: NotRequired[TimingInformationTypeDef],  # (2)
    ConsumedIOs: NotRequired[IOUsageTypeDef],  # (3)
```

1. See [:material-code-braces: PageTypeDef](./type_defs.md#pagetypedef) 
2. See [:material-code-braces: TimingInformationTypeDef](./type_defs.md#timinginformationtypedef) 
3. See [:material-code-braces: IOUsageTypeDef](./type_defs.md#iousagetypedef) 
## FetchPageResultTypeDef

```python
# FetchPageResultTypeDef TypedDict usage example

from types_aiobotocore_qldb_session.type_defs import FetchPageResultTypeDef


def get_value() -> FetchPageResultTypeDef:
    return {
        "Page": ...,
    }


# FetchPageResultTypeDef definition

class FetchPageResultTypeDef(TypedDict):
    Page: NotRequired[PageTypeDef],  # (1)
    TimingInformation: NotRequired[TimingInformationTypeDef],  # (2)
    ConsumedIOs: NotRequired[IOUsageTypeDef],  # (3)
```

1. See [:material-code-braces: PageTypeDef](./type_defs.md#pagetypedef) 
2. See [:material-code-braces: TimingInformationTypeDef](./type_defs.md#timinginformationtypedef) 
3. See [:material-code-braces: IOUsageTypeDef](./type_defs.md#iousagetypedef) 
## ExecuteStatementRequestTypeDef

```python
# ExecuteStatementRequestTypeDef TypedDict usage example

from types_aiobotocore_qldb_session.type_defs import ExecuteStatementRequestTypeDef


def get_value() -> ExecuteStatementRequestTypeDef:
    return {
        "TransactionId": ...,
    }


# ExecuteStatementRequestTypeDef definition

class ExecuteStatementRequestTypeDef(TypedDict):
    TransactionId: str,
    Statement: str,
    Parameters: NotRequired[Sequence[ValueHolderUnionTypeDef]],  # (1)
```

1. See [:material-code-braces: ValueHolderTypeDef](./type_defs.md#valueholdertypedef) [:material-code-braces: ValueHolderOutputTypeDef](./type_defs.md#valueholderoutputtypedef) 
## SendCommandResultTypeDef

```python
# SendCommandResultTypeDef TypedDict usage example

from types_aiobotocore_qldb_session.type_defs import SendCommandResultTypeDef


def get_value() -> SendCommandResultTypeDef:
    return {
        "StartSession": ...,
    }


# SendCommandResultTypeDef definition

class SendCommandResultTypeDef(TypedDict):
    StartSession: StartSessionResultTypeDef,  # (1)
    StartTransaction: StartTransactionResultTypeDef,  # (2)
    EndSession: EndSessionResultTypeDef,  # (3)
    CommitTransaction: CommitTransactionResultTypeDef,  # (4)
    AbortTransaction: AbortTransactionResultTypeDef,  # (5)
    ExecuteStatement: ExecuteStatementResultTypeDef,  # (6)
    FetchPage: FetchPageResultTypeDef,  # (7)
    ResponseMetadata: ResponseMetadataTypeDef,  # (8)
```

1. See [:material-code-braces: StartSessionResultTypeDef](./type_defs.md#startsessionresulttypedef) 
2. See [:material-code-braces: StartTransactionResultTypeDef](./type_defs.md#starttransactionresulttypedef) 
3. See [:material-code-braces: EndSessionResultTypeDef](./type_defs.md#endsessionresulttypedef) 
4. See [:material-code-braces: CommitTransactionResultTypeDef](./type_defs.md#committransactionresulttypedef) 
5. See [:material-code-braces: AbortTransactionResultTypeDef](./type_defs.md#aborttransactionresulttypedef) 
6. See [:material-code-braces: ExecuteStatementResultTypeDef](./type_defs.md#executestatementresulttypedef) 
7. See [:material-code-braces: FetchPageResultTypeDef](./type_defs.md#fetchpageresulttypedef) 
8. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SendCommandRequestTypeDef

```python
# SendCommandRequestTypeDef TypedDict usage example

from types_aiobotocore_qldb_session.type_defs import SendCommandRequestTypeDef


def get_value() -> SendCommandRequestTypeDef:
    return {
        "SessionToken": ...,
    }


# SendCommandRequestTypeDef definition

class SendCommandRequestTypeDef(TypedDict):
    SessionToken: NotRequired[str],
    StartSession: NotRequired[StartSessionRequestTypeDef],  # (1)
    StartTransaction: NotRequired[Mapping[str, Any]],
    EndSession: NotRequired[Mapping[str, Any]],
    CommitTransaction: NotRequired[CommitTransactionRequestTypeDef],  # (2)
    AbortTransaction: NotRequired[Mapping[str, Any]],
    ExecuteStatement: NotRequired[ExecuteStatementRequestTypeDef],  # (3)
    FetchPage: NotRequired[FetchPageRequestTypeDef],  # (4)
```

1. See [:material-code-braces: StartSessionRequestTypeDef](./type_defs.md#startsessionrequesttypedef) 
2. See [:material-code-braces: CommitTransactionRequestTypeDef](./type_defs.md#committransactionrequesttypedef) 
3. See [:material-code-braces: ExecuteStatementRequestTypeDef](./type_defs.md#executestatementrequesttypedef) 
4. See [:material-code-braces: FetchPageRequestTypeDef](./type_defs.md#fetchpagerequesttypedef) 
