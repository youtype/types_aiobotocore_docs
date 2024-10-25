# AgreementServiceClient

> [Index](../README.md) > [AgreementService](./README.md) > AgreementServiceClient

!!! note ""

    Auto-generated documentation for [AgreementService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-agreement.html#AgreementService)
    type annotations stubs module [types-aiobotocore-marketplace-agreement](https://pypi.org/project/types-aiobotocore-marketplace-agreement/).

## AgreementServiceClient

Type annotations and code completion for `#!python session.create_client("marketplace-agreement")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-agreement.html#AgreementService.Client)

```python
# AgreementServiceClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_marketplace_agreement.client import AgreementServiceClient

session = get_session()
async with session.create_client("marketplace-agreement") as client:
    client: AgreementServiceClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("marketplace-agreement").exceptions` structure.

```python
# AgreementServiceClient.exceptions usage example

async with session.create_client("marketplace-agreement") as client:
    try:
        do_something(client)
    except (
            client.AccessDeniedException,
        client.ClientError,
        client.InternalServerException,
        client.ResourceNotFoundException,
        client.ThrottlingException,
        client.ValidationException,
    ) as e:
        print(e)
```

```python
# AgreementServiceClient usage type checking example

from types_aiobotocore_marketplace_agreement.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate

Check if an operation can be paginated.

Type annotations and code completion for `#!python session.create_client("marketplace-agreement").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-agreement.html#AgreementService.Client.can_paginate)

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

Type annotations and code completion for `#!python session.create_client("marketplace-agreement").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-agreement.html#AgreementService.Client.close)

```python
# close method definition

await def close(
    self,
) -> None:
    ...
```


### describe\_agreement

Provides details about an agreement, such as the proposer, acceptor, start
date, and end
date.

Type annotations and code completion for `#!python session.create_client("marketplace-agreement").describe_agreement` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-agreement.html#AgreementService.Client.describe_agreement)

```python
# describe_agreement method definition

await def describe_agreement(
    self,
    *,
    agreementId: str,
) -> DescribeAgreementOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeAgreementOutputTypeDef](./type_defs.md#describeagreementoutputtypedef) 


```python
# describe_agreement method usage example with argument unpacking

kwargs: DescribeAgreementInputRequestTypeDef = {  # (1)
    "agreementId": ...,
}

parent.describe_agreement(**kwargs)
```

1. See [:material-code-braces: DescribeAgreementInputRequestTypeDef](./type_defs.md#describeagreementinputrequesttypedef) 

### generate\_presigned\_url

Generate a presigned url given a client, its method, and arguments.

Type annotations and code completion for `#!python session.create_client("marketplace-agreement").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-agreement.html#AgreementService.Client.generate_presigned_url)

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


### get\_agreement\_terms

Obtains details about the terms in an agreement that you participated in as
proposer or
acceptor.

Type annotations and code completion for `#!python session.create_client("marketplace-agreement").get_agreement_terms` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-agreement.html#AgreementService.Client.get_agreement_terms)

```python
# get_agreement_terms method definition

await def get_agreement_terms(
    self,
    *,
    agreementId: str,
    maxResults: int = ...,
    nextToken: str = ...,
) -> GetAgreementTermsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetAgreementTermsOutputTypeDef](./type_defs.md#getagreementtermsoutputtypedef) 


```python
# get_agreement_terms method usage example with argument unpacking

kwargs: GetAgreementTermsInputRequestTypeDef = {  # (1)
    "agreementId": ...,
}

parent.get_agreement_terms(**kwargs)
```

1. See [:material-code-braces: GetAgreementTermsInputRequestTypeDef](./type_defs.md#getagreementtermsinputrequesttypedef) 

### search\_agreements

Searches across all agreements that a proposer or an acceptor has in AWS
Marketplace.

Type annotations and code completion for `#!python session.create_client("marketplace-agreement").search_agreements` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-agreement.html#AgreementService.Client.search_agreements)

```python
# search_agreements method definition

await def search_agreements(
    self,
    *,
    catalog: str = ...,
    filters: Sequence[FilterTypeDef] = ...,  # (1)
    maxResults: int = ...,
    nextToken: str = ...,
    sort: SortTypeDef = ...,  # (2)
) -> SearchAgreementsOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: SortTypeDef](./type_defs.md#sorttypedef) 
3. See [:material-code-braces: SearchAgreementsOutputTypeDef](./type_defs.md#searchagreementsoutputtypedef) 


```python
# search_agreements method usage example with argument unpacking

kwargs: SearchAgreementsInputRequestTypeDef = {  # (1)
    "catalog": ...,
}

parent.search_agreements(**kwargs)
```

1. See [:material-code-braces: SearchAgreementsInputRequestTypeDef](./type_defs.md#searchagreementsinputrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("marketplace-agreement").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-agreement.html#AgreementService.Client.__aenter__)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> "AgreementServiceClient":
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("marketplace-agreement").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-agreement.html#AgreementService.Client.__aexit__)

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





