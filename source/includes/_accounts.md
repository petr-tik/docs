# Accounts

Accounts represent a store of funds, and have a list of transactions.

## (GET) List accounts

Returns a list of accounts owned by the currently authorised user.

```shell
$ http "https://api.getmondo.co.uk/accounts" \
    "Authorization: Bearer $access_token"
```

```json
{
    "accounts": [
        {
            "id": "acc_00009237aqC8c5umZmrRdh",
            "description": "Peter Pan's Account",
            "created": "2015-11-13T12:17:42Z"
        }
    ]
}
```
