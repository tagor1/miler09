## Methods Table

Miningpoolhub supports some API methods to fetch information in JSON format. This list reflects the current state of the API. All methods used are called via:

```
https://[<coin_name>.]miningpoolhub.com/index.php?page=api&action=<method>&api_key=<user_api_key>[&<argument>=<value>]
```

This table lists all methods and their arguments available.

`Token`: Requires a valid API Key (`api_key` in the URL); `Admin`: `Y`, requires admin, `B`, with or without admin, `N`, no admin required

| API Action | Arguments | Desctipion | Token |
| ------------- |:-------------:| :-----|:-------------:|
| `getminingandprofitsstatistics` | none | Get mining profits statistics | N |
| `getautoswitchingandprofitsstatistics` | none | Get current auto switching info | N |
| `getuserallbalances` | none | Get all currency's balances | Y |
| `getblockcount` | none | Get current block height in blockchain | Y |
| `getblocksfound` | none | Get last N blocks found as configured in admin panel | Y |
| `getblockstats` | none | Get pool block stats | Y |
| `getcurrentworkers` | none | Get amount of current active workers | Y |
| `getdashboarddata` | `id` | Fetch all dashboard related information | Y |
| `getdifficulty` | none | Get current difficulty in blockchain | Y |
| `getestimatedtime` | none | Get estimated time to next block based on pool hashrate (seconds) | Y |
| `gethourlyhashrates` | none | Currently broken | Y |
| `getnavbardata` | none | Get the data displayed on the navbar | Y |
| `getpoolhashrate` | none | Get current pool hashrate | Y |
| `getpoolinfo` | none | Get the information on pool settings | Y |
| `getpoolsharerate` | none | Get current pool share rate (shares/s) | Y |
| `getpoolstatus` | none | Fetch overall pool status, only user token is required | Y |
| `gettimesincelastblock` | none | Get time since last block found (seconds) | Y |
| `gettopcontributors` | none | Fetch top contributors data | Y |
| `getuserbalance` | `id` | Fetch a users balance | Y |
| `getuserhashrate` | `id` | Fetch a users hash rate | Y |
| `getusersharerate` | `id` | Fetch a users share rate | Y |
| `getuserstatus` | `id` | Fetch a users overall status | Y |
| `getusertransactions` | `id` | Get a users transactions | Y |
| `getuserworkers` | `id` | Fetch a users worker status | Y |
| `public` | none | Fetch public pool statistics, no authentication required | N |