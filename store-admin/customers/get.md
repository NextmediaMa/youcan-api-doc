# Get a Customer

Endpoint: `https://api.youcan.shop/customers/{id}`

Method: `GET`

## Subresources

To include a sub-resource, add GET param `include`.
`https://api.youcan.shop/customers/{id}?include=<SUBRESOURCE>`

### Available subresources

- `address`
- `orders`

<a name="response"></a>

## Responses

[200] OK

```json
{
    "id": "da4d2666-33d2-47de-881b-3dad8c4abf62",
    "first_name": "customer_first_name",
    "last_name": "customer_last_name",
    "full_name": "customer_full_name",
    "email": "customer_email",
    "avatar": "https://www.gravatar.com/avatar/f287649f7dd2d340b5e22704b3622ecd?s=100&d=http://api.youcan.shop/store-admin/images/generic_avatar.png",
    "phone": "+212706650843",
    "country": "Morocco",
    "region": "my_region",
    "city": "my_city",
    "notes": "my_",
    "location": "Fes, Morocco",
    "created_at": "2021-04-15T13:55:10+00:00",
    "updated_at": "2021-04-15T13:55:10+00:00",
    "deleted_at": null,
    "links": {
        "edit": "http://seller-area.youcan.shop/admin/customers/da4d2666-33d2-47de-881b-3dad8c4abf62/edit"
    },
    "address": [
        {
            "id": "43cc4816-57dc-4eb1-a828-d2850fe1b42b",
            "first_name": "customer_address_first_name",
            "last_name": "customer_address_last_name",
            "full_name": "customer_address_full_name",
            "first_line": "customer_address_first_line",
            "second_line": "customer_address_second_line",
            "company": "customer_address_company",
            "phone": "+212600000000",
            "country_code": "MA",
            "country_name": "Morocco",
            "state": "customer_state",
            "region": "my_region",
            "city": "my_city",
            "zip_code": "50000",
            "default": true,
            "created_at": 1618494926,
            "updated_at": 1618494926
        }
    ]
}
```

[404] Not Found

```json
{
    "status": 404,
    "code": 0,
    "detail": "Customer not found",
    "meta": []
}
```
