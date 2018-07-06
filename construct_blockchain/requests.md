```
$ curl -X POST -H "Content-Type: application/json" -d '{
"sender": "d4ee26eee15148ee92c6cd394edd974e",
"recipient": "someone-other-address",
"amount": 5
}' "http://localhost:5000/transactions/new"
{
  "message": "Transaction will be added to Block 2"
}

```

```
$ curl -X GET -H "Content-Type: application/json" "http://localhost:5000/chain"
{
  "chain": [
    {
      "index": 1,
      "previous_hash": "1",
      "proof": 100,
      "timestamp": 1530890966.9954557,
      "transactions": []
    }
  ],
  "length": 1
}

```
