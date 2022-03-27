# Examples

> [Index](../README.md) > [AlexaForBusiness](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [AlexaForBusiness](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness)
    type annotations stubs module [types-aiobotocore-alexaforbusiness](https://pypi.org/project/types-aiobotocore-alexaforbusiness/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[alexaforbusiness]` package installed.

Write your `AlexaForBusiness` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aiobotocore.session import get_session


    session = get_session()

    async with session.create_client("alexaforbusiness") as client:  # (1)
        result = await client.create_address_book()  # (2)
    ```

    1. client: [AlexaForBusinessClient](./client.md)
    2. result: [:material-code-braces: CreateAddressBookResponseTypeDef](./type_defs.md#createaddressbookresponsetypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aiobotocore.session import get_session


    session = get_session()

    async with session.create_client("alexaforbusiness") as client:  # (1)
        paginator = client.get_paginator("list_business_report_schedules")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [AlexaForBusinessClient](./client.md)
    2. paginator: [ListBusinessReportSchedulesPaginator](./paginators.md#listbusinessreportschedulespaginator)
    3. item: [:material-code-braces: ListBusinessReportSchedulesResponseTypeDef](./type_defs.md#listbusinessreportschedulesresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[alexaforbusiness]`
or a standalone `types_aiobotocore_alexaforbusiness` package, you have to explicitly specify
`client: AlexaForBusinessClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aiobotocore.session import get_session

    from types_aiobotocore_alexaforbusiness.client import AlexaForBusinessClient
    from types_aiobotocore_alexaforbusiness.type_defs import CreateAddressBookResponseTypeDef
    from types_aiobotocore_alexaforbusiness.type_defs import CreateAddressBookRequestRequestTypeDef


    session = get_session()

    async with session.create_client("alexaforbusiness") as client:
        client: AlexaForBusinessClient
        kwargs: CreateAddressBookRequestRequestTypeDef = {...}
        result: CreateAddressBookResponseTypeDef = await client.create_address_book(**kwargs)
    ```



=== "Paginators"

    ```python title="Paginator usage example"
    from aiobotocore.session import get_session

    from types_aiobotocore_alexaforbusiness.client import AlexaForBusinessClient
    from types_aiobotocore_alexaforbusiness.paginator import ListBusinessReportSchedulesPaginator
    from types_aiobotocore_alexaforbusiness.type_defs import ListBusinessReportSchedulesResponseTypeDef


    session = get_session()

    async with session.create_client("alexaforbusiness") as client:
        client: AlexaForBusinessClient
        paginator: ListBusinessReportSchedulesPaginator = client.get_paginator("list_business_report_schedules")
        async for item in paginator.paginate(...):
            item: ListBusinessReportSchedulesResponseTypeDef
            print(item)
    ```


