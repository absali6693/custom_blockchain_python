# Simple Blockchain in Pythont

### To register a node using crul :

```javascript
curl -X POST -H "Content-Type: application/json" -d '{
"nodes": ["127.0.0.1:5001"] 
}' "http://localhost:5000/nodes/register"
```

### To make a new transaction: 

```javascript
curl -X POST -H "Content-Type: application/json" -d '{
"sender": "sender-address",
"recipient": "receivers-address",
"amount": 5
}' "http://localhost:5000/transactions/new"
```

### To mine a block use:

#### Get method
```javascript
http://localhost:5000/mine
```
### To get the chain:
```javascript
http://localhost:5000/chain
```

### What's comming next:

-   File saperation.
-   cron based resolution of the chain
