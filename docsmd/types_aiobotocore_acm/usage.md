# Examples

> [Index](../README.md) > [ACM](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [ACM](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM)
    type annotations stubs module [types-aiobotocore-acm](https://pypi.org/project/types-aiobotocore-acm/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[acm]` package installed.

Write your `ACM` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aiobotocore.session import get_session


    session = get_session()

    async with session.create_client("acm") as client:  # (1)
        result = await client.describe_certificate()  # (2)
    ```

    1. client: [ACMClient](./client.md)
    2. result: [:material-code-braces: DescribeCertificateResponseTypeDef](./type_defs.md#describecertificateresponsetypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aiobotocore.session import get_session


    session = get_session()

    async with session.create_client("acm") as client:  # (1)
        paginator = client.get_paginator("list_certificates")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [ACMClient](./client.md)
    2. paginator: [ListCertificatesPaginator](./paginators.md#listcertificatespaginator)
    3. item: [:material-code-braces: ListCertificatesResponseTypeDef](./type_defs.md#listcertificatesresponsetypedef) 



=== "Waiters"

    ```python title="Waiter usage example"
    from aiobotocore.session import get_session


    session = get_session()

    async with session.create_client("acm") as client:  # (1)
        waiter = client.get_waiter("certificate_validated")  # (2)
        await waiter.wait()
    ```

    1. client: [ACMClient](./client.md)
    2. waiter: [CertificateValidatedWaiter](./waiters.md#certificatevalidatedwaiter)


### Explicit type annotations

With `types-aiobotocore-lite[acm]`
or a standalone `types_aiobotocore_acm` package, you have to explicitly specify
`client: ACMClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aiobotocore.session import get_session

    from types_aiobotocore_acm.client import ACMClient
    from types_aiobotocore_acm.type_defs import DescribeCertificateResponseTypeDef
    from types_aiobotocore_acm.type_defs import DescribeCertificateRequestRequestTypeDef


    session = get_session()

    async with session.create_client("acm") as client:
        client: ACMClient
        kwargs: DescribeCertificateRequestRequestTypeDef = {...}
        result: DescribeCertificateResponseTypeDef = await client.describe_certificate(**kwargs)
    ```



=== "Paginators"

    ```python title="Paginator usage example"
    from aiobotocore.session import get_session

    from types_aiobotocore_acm.client import ACMClient
    from types_aiobotocore_acm.paginator import ListCertificatesPaginator
    from types_aiobotocore_acm.type_defs import ListCertificatesResponseTypeDef


    session = get_session()

    async with session.create_client("acm") as client:
        client: ACMClient
        paginator: ListCertificatesPaginator = client.get_paginator("list_certificates")
        async for item in paginator.paginate(...):
            item: ListCertificatesResponseTypeDef
            print(item)
    ```



=== "Waiters"

    ```python title="Waiter usage example"
    from aiobotocore.session import get_session

    from types_aiobotocore_acm.client import ACMClient
    from types_aiobotocore_acm.waiter import CertificateValidatedWaiter


    session = get_session()

    async with session.create_client("acm") as client:
        client: ACMClient
        waiter: CertificateValidatedWaiter = client.get_waiter("certificate_validated")
        await waiter.wait()
    ```
