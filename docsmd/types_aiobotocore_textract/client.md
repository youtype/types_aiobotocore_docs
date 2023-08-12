# TextractClient

> [Index](../README.md) > [Textract](./README.md) > TextractClient

!!! note ""

    Auto-generated documentation for [Textract](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/textract.html#Textract)
    type annotations stubs module [types-aiobotocore-textract](https://pypi.org/project/types-aiobotocore-textract/).

## TextractClient

Type annotations and code completion for `#!python session.create_client("textract")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/textract.html#Textract.Client)

```python
TextractClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_textract.client import TextractClient

session = get_session()
async with session.create_client("textract") as client:
    client: TextractClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("textract").exceptions` structure.

```python
TextractClient.exceptions usage example

async with session.create_client("textract") as client:
    try:
        do_something(client)
    except (
            client.AccessDeniedException,
        client.BadDocumentException,
        client.ClientError,
        client.DocumentTooLargeException,
        client.HumanLoopQuotaExceededException,
        client.IdempotentParameterMismatchException,
        client.InternalServerError,
        client.InvalidJobIdException,
        client.InvalidKMSKeyException,
        client.InvalidParameterException,
        client.InvalidS3ObjectException,
        client.LimitExceededException,
        client.ProvisionedThroughputExceededException,
        client.ThrottlingException,
        client.UnsupportedDocumentException,
    ) as e:
        print(e)
```

```python
TextractClient usage type checking example

from types_aiobotocore_textract.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### analyze\_document

Analyzes an input document for relationships between detected items.

Type annotations and code completion for `#!python session.create_client("textract").analyze_document` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/textract.html#Textract.Client.analyze_document)

```python
# analyze_document method definition

await def analyze_document(
    self,
    *,
    Document: DocumentTypeDef,  # (1)
    FeatureTypes: Sequence[FeatureTypeType],  # (2)
    HumanLoopConfig: HumanLoopConfigTypeDef = ...,  # (3)
    QueriesConfig: QueriesConfigTypeDef = ...,  # (4)
) -> AnalyzeDocumentResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-braces: DocumentTypeDef](./type_defs.md#documenttypedef) 
2. See [:material-code-brackets: FeatureTypeType](./literals.md#featuretypetype) 
3. See [:material-code-braces: HumanLoopConfigTypeDef](./type_defs.md#humanloopconfigtypedef) 
4. See [:material-code-braces: QueriesConfigTypeDef](./type_defs.md#queriesconfigtypedef) 
5. See [:material-code-braces: AnalyzeDocumentResponseTypeDef](./type_defs.md#analyzedocumentresponsetypedef) 


```python
# analyze_document method usage example with argument unpacking

kwargs: AnalyzeDocumentRequestRequestTypeDef = {  # (1)
    "Document": ...,
    "FeatureTypes": ...,
}

parent.analyze_document(**kwargs)
```

1. See [:material-code-braces: AnalyzeDocumentRequestRequestTypeDef](./type_defs.md#analyzedocumentrequestrequesttypedef) 

### analyze\_expense

`AnalyzeExpense` synchronously analyzes an input document for financially
related relationships between text.

Type annotations and code completion for `#!python session.create_client("textract").analyze_expense` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/textract.html#Textract.Client.analyze_expense)

```python
# analyze_expense method definition

await def analyze_expense(
    self,
    *,
    Document: DocumentTypeDef,  # (1)
) -> AnalyzeExpenseResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: DocumentTypeDef](./type_defs.md#documenttypedef) 
2. See [:material-code-braces: AnalyzeExpenseResponseTypeDef](./type_defs.md#analyzeexpenseresponsetypedef) 


```python
# analyze_expense method usage example with argument unpacking

kwargs: AnalyzeExpenseRequestRequestTypeDef = {  # (1)
    "Document": ...,
}

parent.analyze_expense(**kwargs)
```

1. See [:material-code-braces: AnalyzeExpenseRequestRequestTypeDef](./type_defs.md#analyzeexpenserequestrequesttypedef) 

### analyze\_id

Analyzes identity documents for relevant information.

Type annotations and code completion for `#!python session.create_client("textract").analyze_id` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/textract.html#Textract.Client.analyze_id)

```python
# analyze_id method definition

await def analyze_id(
    self,
    *,
    DocumentPages: Sequence[DocumentTypeDef],  # (1)
) -> AnalyzeIDResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: DocumentTypeDef](./type_defs.md#documenttypedef) 
2. See [:material-code-braces: AnalyzeIDResponseTypeDef](./type_defs.md#analyzeidresponsetypedef) 


```python
# analyze_id method usage example with argument unpacking

kwargs: AnalyzeIDRequestRequestTypeDef = {  # (1)
    "DocumentPages": ...,
}

parent.analyze_id(**kwargs)
```

1. See [:material-code-braces: AnalyzeIDRequestRequestTypeDef](./type_defs.md#analyzeidrequestrequesttypedef) 

### can\_paginate

Check if an operation can be paginated.

Type annotations and code completion for `#!python session.create_client("textract").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/textract.html#Textract.Client.can_paginate)

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

Type annotations and code completion for `#!python session.create_client("textract").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/textract.html#Textract.Client.close)

```python
# close method definition

await def close(
    self,
) -> None:
    ...
```


### detect\_document\_text

Detects text in the input document.

Type annotations and code completion for `#!python session.create_client("textract").detect_document_text` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/textract.html#Textract.Client.detect_document_text)

```python
# detect_document_text method definition

await def detect_document_text(
    self,
    *,
    Document: DocumentTypeDef,  # (1)
) -> DetectDocumentTextResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: DocumentTypeDef](./type_defs.md#documenttypedef) 
2. See [:material-code-braces: DetectDocumentTextResponseTypeDef](./type_defs.md#detectdocumenttextresponsetypedef) 


```python
# detect_document_text method usage example with argument unpacking

kwargs: DetectDocumentTextRequestRequestTypeDef = {  # (1)
    "Document": ...,
}

parent.detect_document_text(**kwargs)
```

1. See [:material-code-braces: DetectDocumentTextRequestRequestTypeDef](./type_defs.md#detectdocumenttextrequestrequesttypedef) 

### generate\_presigned\_url

Generate a presigned url given a client, its method, and arguments.

Type annotations and code completion for `#!python session.create_client("textract").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/textract.html#Textract.Client.generate_presigned_url)

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


### get\_document\_analysis

Gets the results for an Amazon Textract asynchronous operation that analyzes
text in a document.

Type annotations and code completion for `#!python session.create_client("textract").get_document_analysis` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/textract.html#Textract.Client.get_document_analysis)

```python
# get_document_analysis method definition

await def get_document_analysis(
    self,
    *,
    JobId: str,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> GetDocumentAnalysisResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetDocumentAnalysisResponseTypeDef](./type_defs.md#getdocumentanalysisresponsetypedef) 


```python
# get_document_analysis method usage example with argument unpacking

kwargs: GetDocumentAnalysisRequestRequestTypeDef = {  # (1)
    "JobId": ...,
}

parent.get_document_analysis(**kwargs)
```

1. See [:material-code-braces: GetDocumentAnalysisRequestRequestTypeDef](./type_defs.md#getdocumentanalysisrequestrequesttypedef) 

### get\_document\_text\_detection

Gets the results for an Amazon Textract asynchronous operation that detects text
in a document.

Type annotations and code completion for `#!python session.create_client("textract").get_document_text_detection` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/textract.html#Textract.Client.get_document_text_detection)

```python
# get_document_text_detection method definition

await def get_document_text_detection(
    self,
    *,
    JobId: str,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> GetDocumentTextDetectionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetDocumentTextDetectionResponseTypeDef](./type_defs.md#getdocumenttextdetectionresponsetypedef) 


```python
# get_document_text_detection method usage example with argument unpacking

kwargs: GetDocumentTextDetectionRequestRequestTypeDef = {  # (1)
    "JobId": ...,
}

parent.get_document_text_detection(**kwargs)
```

1. See [:material-code-braces: GetDocumentTextDetectionRequestRequestTypeDef](./type_defs.md#getdocumenttextdetectionrequestrequesttypedef) 

### get\_expense\_analysis

Gets the results for an Amazon Textract asynchronous operation that analyzes
invoices and receipts.

Type annotations and code completion for `#!python session.create_client("textract").get_expense_analysis` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/textract.html#Textract.Client.get_expense_analysis)

```python
# get_expense_analysis method definition

await def get_expense_analysis(
    self,
    *,
    JobId: str,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> GetExpenseAnalysisResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetExpenseAnalysisResponseTypeDef](./type_defs.md#getexpenseanalysisresponsetypedef) 


```python
# get_expense_analysis method usage example with argument unpacking

kwargs: GetExpenseAnalysisRequestRequestTypeDef = {  # (1)
    "JobId": ...,
}

parent.get_expense_analysis(**kwargs)
```

1. See [:material-code-braces: GetExpenseAnalysisRequestRequestTypeDef](./type_defs.md#getexpenseanalysisrequestrequesttypedef) 

### get\_lending\_analysis

Gets the results for an Amazon Textract asynchronous operation that analyzes
text in a lending document.

Type annotations and code completion for `#!python session.create_client("textract").get_lending_analysis` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/textract.html#Textract.Client.get_lending_analysis)

```python
# get_lending_analysis method definition

await def get_lending_analysis(
    self,
    *,
    JobId: str,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> GetLendingAnalysisResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetLendingAnalysisResponseTypeDef](./type_defs.md#getlendinganalysisresponsetypedef) 


```python
# get_lending_analysis method usage example with argument unpacking

kwargs: GetLendingAnalysisRequestRequestTypeDef = {  # (1)
    "JobId": ...,
}

parent.get_lending_analysis(**kwargs)
```

1. See [:material-code-braces: GetLendingAnalysisRequestRequestTypeDef](./type_defs.md#getlendinganalysisrequestrequesttypedef) 

### get\_lending\_analysis\_summary

Gets summarized results for the `StartLendingAnalysis` operation, which analyzes
text in a lending document.

Type annotations and code completion for `#!python session.create_client("textract").get_lending_analysis_summary` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/textract.html#Textract.Client.get_lending_analysis_summary)

```python
# get_lending_analysis_summary method definition

await def get_lending_analysis_summary(
    self,
    *,
    JobId: str,
) -> GetLendingAnalysisSummaryResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetLendingAnalysisSummaryResponseTypeDef](./type_defs.md#getlendinganalysissummaryresponsetypedef) 


```python
# get_lending_analysis_summary method usage example with argument unpacking

kwargs: GetLendingAnalysisSummaryRequestRequestTypeDef = {  # (1)
    "JobId": ...,
}

parent.get_lending_analysis_summary(**kwargs)
```

1. See [:material-code-braces: GetLendingAnalysisSummaryRequestRequestTypeDef](./type_defs.md#getlendinganalysissummaryrequestrequesttypedef) 

### start\_document\_analysis

Starts the asynchronous analysis of an input document for relationships between
detected items such as key-value pairs, tables, and selection elements.

Type annotations and code completion for `#!python session.create_client("textract").start_document_analysis` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/textract.html#Textract.Client.start_document_analysis)

```python
# start_document_analysis method definition

await def start_document_analysis(
    self,
    *,
    DocumentLocation: DocumentLocationTypeDef,  # (1)
    FeatureTypes: Sequence[FeatureTypeType],  # (2)
    ClientRequestToken: str = ...,
    JobTag: str = ...,
    NotificationChannel: NotificationChannelTypeDef = ...,  # (3)
    OutputConfig: OutputConfigTypeDef = ...,  # (4)
    KMSKeyId: str = ...,
    QueriesConfig: QueriesConfigTypeDef = ...,  # (5)
) -> StartDocumentAnalysisResponseTypeDef:  # (6)
    ...
```

1. See [:material-code-braces: DocumentLocationTypeDef](./type_defs.md#documentlocationtypedef) 
2. See [:material-code-brackets: FeatureTypeType](./literals.md#featuretypetype) 
3. See [:material-code-braces: NotificationChannelTypeDef](./type_defs.md#notificationchanneltypedef) 
4. See [:material-code-braces: OutputConfigTypeDef](./type_defs.md#outputconfigtypedef) 
5. See [:material-code-braces: QueriesConfigTypeDef](./type_defs.md#queriesconfigtypedef) 
6. See [:material-code-braces: StartDocumentAnalysisResponseTypeDef](./type_defs.md#startdocumentanalysisresponsetypedef) 


```python
# start_document_analysis method usage example with argument unpacking

kwargs: StartDocumentAnalysisRequestRequestTypeDef = {  # (1)
    "DocumentLocation": ...,
    "FeatureTypes": ...,
}

parent.start_document_analysis(**kwargs)
```

1. See [:material-code-braces: StartDocumentAnalysisRequestRequestTypeDef](./type_defs.md#startdocumentanalysisrequestrequesttypedef) 

### start\_document\_text\_detection

Starts the asynchronous detection of text in a document.

Type annotations and code completion for `#!python session.create_client("textract").start_document_text_detection` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/textract.html#Textract.Client.start_document_text_detection)

```python
# start_document_text_detection method definition

await def start_document_text_detection(
    self,
    *,
    DocumentLocation: DocumentLocationTypeDef,  # (1)
    ClientRequestToken: str = ...,
    JobTag: str = ...,
    NotificationChannel: NotificationChannelTypeDef = ...,  # (2)
    OutputConfig: OutputConfigTypeDef = ...,  # (3)
    KMSKeyId: str = ...,
) -> StartDocumentTextDetectionResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: DocumentLocationTypeDef](./type_defs.md#documentlocationtypedef) 
2. See [:material-code-braces: NotificationChannelTypeDef](./type_defs.md#notificationchanneltypedef) 
3. See [:material-code-braces: OutputConfigTypeDef](./type_defs.md#outputconfigtypedef) 
4. See [:material-code-braces: StartDocumentTextDetectionResponseTypeDef](./type_defs.md#startdocumenttextdetectionresponsetypedef) 


```python
# start_document_text_detection method usage example with argument unpacking

kwargs: StartDocumentTextDetectionRequestRequestTypeDef = {  # (1)
    "DocumentLocation": ...,
}

parent.start_document_text_detection(**kwargs)
```

1. See [:material-code-braces: StartDocumentTextDetectionRequestRequestTypeDef](./type_defs.md#startdocumenttextdetectionrequestrequesttypedef) 

### start\_expense\_analysis

Starts the asynchronous analysis of invoices or receipts for data like contact
information, items purchased, and vendor names.

Type annotations and code completion for `#!python session.create_client("textract").start_expense_analysis` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/textract.html#Textract.Client.start_expense_analysis)

```python
# start_expense_analysis method definition

await def start_expense_analysis(
    self,
    *,
    DocumentLocation: DocumentLocationTypeDef,  # (1)
    ClientRequestToken: str = ...,
    JobTag: str = ...,
    NotificationChannel: NotificationChannelTypeDef = ...,  # (2)
    OutputConfig: OutputConfigTypeDef = ...,  # (3)
    KMSKeyId: str = ...,
) -> StartExpenseAnalysisResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: DocumentLocationTypeDef](./type_defs.md#documentlocationtypedef) 
2. See [:material-code-braces: NotificationChannelTypeDef](./type_defs.md#notificationchanneltypedef) 
3. See [:material-code-braces: OutputConfigTypeDef](./type_defs.md#outputconfigtypedef) 
4. See [:material-code-braces: StartExpenseAnalysisResponseTypeDef](./type_defs.md#startexpenseanalysisresponsetypedef) 


```python
# start_expense_analysis method usage example with argument unpacking

kwargs: StartExpenseAnalysisRequestRequestTypeDef = {  # (1)
    "DocumentLocation": ...,
}

parent.start_expense_analysis(**kwargs)
```

1. See [:material-code-braces: StartExpenseAnalysisRequestRequestTypeDef](./type_defs.md#startexpenseanalysisrequestrequesttypedef) 

### start\_lending\_analysis

Starts the classification and analysis of an input document.

Type annotations and code completion for `#!python session.create_client("textract").start_lending_analysis` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/textract.html#Textract.Client.start_lending_analysis)

```python
# start_lending_analysis method definition

await def start_lending_analysis(
    self,
    *,
    DocumentLocation: DocumentLocationTypeDef,  # (1)
    ClientRequestToken: str = ...,
    JobTag: str = ...,
    NotificationChannel: NotificationChannelTypeDef = ...,  # (2)
    OutputConfig: OutputConfigTypeDef = ...,  # (3)
    KMSKeyId: str = ...,
) -> StartLendingAnalysisResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: DocumentLocationTypeDef](./type_defs.md#documentlocationtypedef) 
2. See [:material-code-braces: NotificationChannelTypeDef](./type_defs.md#notificationchanneltypedef) 
3. See [:material-code-braces: OutputConfigTypeDef](./type_defs.md#outputconfigtypedef) 
4. See [:material-code-braces: StartLendingAnalysisResponseTypeDef](./type_defs.md#startlendinganalysisresponsetypedef) 


```python
# start_lending_analysis method usage example with argument unpacking

kwargs: StartLendingAnalysisRequestRequestTypeDef = {  # (1)
    "DocumentLocation": ...,
}

parent.start_lending_analysis(**kwargs)
```

1. See [:material-code-braces: StartLendingAnalysisRequestRequestTypeDef](./type_defs.md#startlendinganalysisrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("textract").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/textract.html#Textract.Client.__aenter__)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> TextractClient:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("textract").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/textract.html#Textract.Client.__aexit__)

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





