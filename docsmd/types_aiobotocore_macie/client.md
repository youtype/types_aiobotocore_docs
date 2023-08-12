# MacieClient

> [Index](../README.md) > [Macie](./README.md) > MacieClient

!!! note ""

    Auto-generated documentation for [Macie](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie.html#Macie)
    type annotations stubs module [types-aiobotocore-macie](https://pypi.org/project/types-aiobotocore-macie/).

## MacieClient

Type annotations and code completion for `#!python session.create_client("macie")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie.html#Macie.Client)

```python
MacieClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_macie.client import MacieClient

session = get_session()
async with session.create_client("macie") as client:
    client: MacieClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("macie").exceptions` structure.

```python
MacieClient.exceptions usage example

async with session.create_client("macie") as client:
    try:
        do_something(client)
    except (
            client.AccessDeniedException,
        client.ClientError,
        client.InternalException,
        client.InvalidInputException,
        client.LimitExceededException,
    ) as e:
        print(e)
```

```python
MacieClient usage type checking example

from types_aiobotocore_macie.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### associate\_member\_account

(Discontinued) Associates a specified Amazon Web Services account with Amazon
Macie Classic as a member account.

Type annotations and code completion for `#!python session.create_client("macie").associate_member_account` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie.html#Macie.Client.associate_member_account)

```python
# associate_member_account method definition

await def associate_member_account(
    self,
    *,
    memberAccountId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# associate_member_account method usage example with argument unpacking

kwargs: AssociateMemberAccountRequestRequestTypeDef = {  # (1)
    "memberAccountId": ...,
}

parent.associate_member_account(**kwargs)
```

1. See [:material-code-braces: AssociateMemberAccountRequestRequestTypeDef](./type_defs.md#associatememberaccountrequestrequesttypedef) 

### associate\_s3\_resources

(Discontinued) Associates specified S3 resources with Amazon Macie Classic for
monitoring and data classification.

Type annotations and code completion for `#!python session.create_client("macie").associate_s3_resources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie.html#Macie.Client.associate_s3_resources)

```python
# associate_s3_resources method definition

await def associate_s3_resources(
    self,
    *,
    s3Resources: Sequence[S3ResourceClassificationTypeDef],  # (1)
    memberAccountId: str = ...,
) -> AssociateS3ResourcesResultTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: S3ResourceClassificationTypeDef](./type_defs.md#s3resourceclassificationtypedef) 
2. See [:material-code-braces: AssociateS3ResourcesResultTypeDef](./type_defs.md#associates3resourcesresulttypedef) 


```python
# associate_s3_resources method usage example with argument unpacking

kwargs: AssociateS3ResourcesRequestRequestTypeDef = {  # (1)
    "s3Resources": ...,
}

parent.associate_s3_resources(**kwargs)
```

1. See [:material-code-braces: AssociateS3ResourcesRequestRequestTypeDef](./type_defs.md#associates3resourcesrequestrequesttypedef) 

### can\_paginate

Check if an operation can be paginated.

Type annotations and code completion for `#!python session.create_client("macie").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie.html#Macie.Client.can_paginate)

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

Type annotations and code completion for `#!python session.create_client("macie").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie.html#Macie.Client.close)

```python
# close method definition

await def close(
    self,
) -> None:
    ...
```


### disassociate\_member\_account

(Discontinued) Removes the specified member account from Amazon Macie Classic.

Type annotations and code completion for `#!python session.create_client("macie").disassociate_member_account` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie.html#Macie.Client.disassociate_member_account)

```python
# disassociate_member_account method definition

await def disassociate_member_account(
    self,
    *,
    memberAccountId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# disassociate_member_account method usage example with argument unpacking

kwargs: DisassociateMemberAccountRequestRequestTypeDef = {  # (1)
    "memberAccountId": ...,
}

parent.disassociate_member_account(**kwargs)
```

1. See [:material-code-braces: DisassociateMemberAccountRequestRequestTypeDef](./type_defs.md#disassociatememberaccountrequestrequesttypedef) 

### disassociate\_s3\_resources

(Discontinued) Removes specified S3 resources from being monitored by Amazon
Macie Classic.

Type annotations and code completion for `#!python session.create_client("macie").disassociate_s3_resources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie.html#Macie.Client.disassociate_s3_resources)

```python
# disassociate_s3_resources method definition

await def disassociate_s3_resources(
    self,
    *,
    associatedS3Resources: Sequence[S3ResourceTypeDef],  # (1)
    memberAccountId: str = ...,
) -> DisassociateS3ResourcesResultTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: S3ResourceTypeDef](./type_defs.md#s3resourcetypedef) 
2. See [:material-code-braces: DisassociateS3ResourcesResultTypeDef](./type_defs.md#disassociates3resourcesresulttypedef) 


```python
# disassociate_s3_resources method usage example with argument unpacking

kwargs: DisassociateS3ResourcesRequestRequestTypeDef = {  # (1)
    "associatedS3Resources": ...,
}

parent.disassociate_s3_resources(**kwargs)
```

1. See [:material-code-braces: DisassociateS3ResourcesRequestRequestTypeDef](./type_defs.md#disassociates3resourcesrequestrequesttypedef) 

### generate\_presigned\_url

Generate a presigned url given a client, its method, and arguments.

Type annotations and code completion for `#!python session.create_client("macie").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie.html#Macie.Client.generate_presigned_url)

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


### list\_member\_accounts

(Discontinued) Lists all Amazon Macie Classic member accounts for the current
Macie Classic administrator account.

Type annotations and code completion for `#!python session.create_client("macie").list_member_accounts` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie.html#Macie.Client.list_member_accounts)

```python
# list_member_accounts method definition

await def list_member_accounts(
    self,
    *,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListMemberAccountsResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListMemberAccountsResultTypeDef](./type_defs.md#listmemberaccountsresulttypedef) 


```python
# list_member_accounts method usage example with argument unpacking

kwargs: ListMemberAccountsRequestRequestTypeDef = {  # (1)
    "nextToken": ...,
}

parent.list_member_accounts(**kwargs)
```

1. See [:material-code-braces: ListMemberAccountsRequestRequestTypeDef](./type_defs.md#listmemberaccountsrequestrequesttypedef) 

### list\_s3\_resources

(Discontinued) Lists all the S3 resources associated with Amazon Macie Classic.

Type annotations and code completion for `#!python session.create_client("macie").list_s3_resources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie.html#Macie.Client.list_s3_resources)

```python
# list_s3_resources method definition

await def list_s3_resources(
    self,
    *,
    memberAccountId: str = ...,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListS3ResourcesResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListS3ResourcesResultTypeDef](./type_defs.md#lists3resourcesresulttypedef) 


```python
# list_s3_resources method usage example with argument unpacking

kwargs: ListS3ResourcesRequestRequestTypeDef = {  # (1)
    "memberAccountId": ...,
}

parent.list_s3_resources(**kwargs)
```

1. See [:material-code-braces: ListS3ResourcesRequestRequestTypeDef](./type_defs.md#lists3resourcesrequestrequesttypedef) 

### update\_s3\_resources

(Discontinued) Updates the classification types for the specified S3 resources.

Type annotations and code completion for `#!python session.create_client("macie").update_s3_resources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie.html#Macie.Client.update_s3_resources)

```python
# update_s3_resources method definition

await def update_s3_resources(
    self,
    *,
    s3ResourcesUpdate: Sequence[S3ResourceClassificationUpdateTypeDef],  # (1)
    memberAccountId: str = ...,
) -> UpdateS3ResourcesResultTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: S3ResourceClassificationUpdateTypeDef](./type_defs.md#s3resourceclassificationupdatetypedef) 
2. See [:material-code-braces: UpdateS3ResourcesResultTypeDef](./type_defs.md#updates3resourcesresulttypedef) 


```python
# update_s3_resources method usage example with argument unpacking

kwargs: UpdateS3ResourcesRequestRequestTypeDef = {  # (1)
    "s3ResourcesUpdate": ...,
}

parent.update_s3_resources(**kwargs)
```

1. See [:material-code-braces: UpdateS3ResourcesRequestRequestTypeDef](./type_defs.md#updates3resourcesrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("macie").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie.html#Macie.Client.__aenter__)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> MacieClient:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("macie").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie.html#Macie.Client.__aexit__)

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

Type annotations and code completion for `#!python session.create_client("macie").get_paginator` method with overloads.

- `client.get_paginator("list_member_accounts")` -> [ListMemberAccountsPaginator](./paginators.md#listmemberaccountspaginator)
- `client.get_paginator("list_s3_resources")` -> [ListS3ResourcesPaginator](./paginators.md#lists3resourcespaginator)



