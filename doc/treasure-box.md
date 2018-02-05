# Treasure Box

> Some important RPC calls you want to be aware of

## Create a new address

```
$> ./EmollientCoind getnewaddress
NVWc6Q7ui31zt3PNUKwu73eRna6U9ZoNQY
```

## Send 100 coins to this address

```
$> ./EmollientCoind sendtoaddress 100 NVWc6Q7ui31zt3PNUKwu73eRna6U9ZoNQY
```

## Show the current balance

```
$> ./EmollientCoind getbalance
100.0
```

**Note:** `getbalance` does not include the coins that haven't matured yet (ie. the coins that have been mined/minted less than 500 blocks ago). In order to get them, you will have to ...

## Show all received transactions

```
$> ./EmollientCoind listsinceblock
```

## Show all matured unspend outputs

```
$> ./EmollientCoind listunspent
```
