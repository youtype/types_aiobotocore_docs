# Type definitions

> [Index](../README.md) > [QLDBSession](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [QLDBSession](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb-session.html#QLDBSession)
    type annotations stubs module [types-aiobotocore-qldb-session](https://pypi.org/project/types-aiobotocore-qldb-session/).

## BlobTypeDef

```python
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
# TimingInformationTypeDef definition

class TimingInformationTypeDef(TypedDict):
    ProcessingTimeMilliseconds: NotRequired[int],
```

## IOUsageTypeDef

```python
# IOUsageTypeDef definition

class IOUsageTypeDef(TypedDict):
    ReadIOs: NotRequired[int],
    WriteIOs: NotRequired[int],
```

## FetchPageRequestTypeDef

```python
# FetchPageRequestTypeDef definition

class FetchPageRequestTypeDef(TypedDict):
    TransactionId: str,
    NextPageToken: str,
```

## ValueHolderOutputTypeDef

```python
# ValueHolderOutputTypeDef definition

class ValueHolderOutputTypeDef(TypedDict):
    IonBinary: NotRequired[bytes],
    IonText: NotRequired[str],
```

## ResponseMetadataTypeDef

```python
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
# StartSessionRequestTypeDef definition

class StartSessionRequestTypeDef(TypedDict):
    LedgerName: str,
```

## AbortTransactionResultTypeDef

```python
# AbortTransactionResultTypeDef definition

class AbortTransactionResultTypeDef(TypedDict):
    TimingInformation: NotRequired[TimingInformationTypeDef],  # (1)
```

1. See [:material-code-braces: TimingInformationTypeDef](./type_defs.md#timinginformationtypedef) 
## EndSessionResultTypeDef

```python
# EndSessionResultTypeDef definition

class EndSessionResultTypeDef(TypedDict):
    TimingInformation: NotRequired[TimingInformationTypeDef],  # (1)
```

1. See [:material-code-braces: TimingInformationTypeDef](./type_defs.md#timinginformationtypedef) 
## StartSessionResultTypeDef

```python
# StartSessionResultTypeDef definition

class StartSessionResultTypeDef(TypedDict):
    SessionToken: NotRequired[str],
    TimingInformation: NotRequired[TimingInformationTypeDef],  # (1)
```

1. See [:material-code-braces: TimingInformationTypeDef](./type_defs.md#timinginformationtypedef) 
## StartTransactionResultTypeDef

```python
# StartTransactionResultTypeDef definition

class StartTransactionResultTypeDef(TypedDict):
    TransactionId: NotRequired[str],
    TimingInformation: NotRequired[TimingInformationTypeDef],  # (1)
```

1. See [:material-code-braces: TimingInformationTypeDef](./type_defs.md#timinginformationtypedef) 
## CommitTransactionRequestTypeDef

```python
# CommitTransactionRequestTypeDef definition

class CommitTransactionRequestTypeDef(TypedDict):
    TransactionId: str,
    CommitDigest: BlobTypeDef,
```

## ValueHolderTypeDef

```python
# ValueHolderTypeDef definition

class ValueHolderTypeDef(TypedDict):
    IonBinary: NotRequired[BlobTypeDef],
    IonText: NotRequired[str],
```

## CommitTransactionResultTypeDef

```python
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
# PageTypeDef definition

class PageTypeDef(TypedDict):
    Values: NotRequired[List[ValueHolderOutputTypeDef]],  # (1)
    NextPageToken: NotRequired[str],
```

1. See [:material-code-braces: ValueHolderOutputTypeDef](./type_defs.md#valueholderoutputtypedef) 
## ExecuteStatementResultTypeDef

```python
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
# ExecuteStatementRequestTypeDef definition

class ExecuteStatementRequestTypeDef(TypedDict):
    TransactionId: str,
    Statement: str,
    Parameters: NotRequired[Sequence[ValueHolderUnionTypeDef]],  # (1)
```

1. See [:material-code-braces: ValueHolderTypeDef](./type_defs.md#valueholdertypedef) [:material-code-braces: ValueHolderOutputTypeDef](./type_defs.md#valueholderoutputtypedef) 
## SendCommandResultTypeDef

```python
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
## SendCommandRequestRequestTypeDef

```python
# SendCommandRequestRequestTypeDef definition

class SendCommandRequestRequestTypeDef(TypedDict):
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
