## Methods Table

Miningpoolhub supports some API methods to fetch information in JSON format. This list reflects the current state of the API. All methods used are called via:

```
https://[coin_name.]miningpoolhub.com/index.php?page=api&action=<method>&api_key=<user_api_key>[&<argument>=<value>]
```

This table lists all methods and their arguments available.

`Token`: Requires a valid API Key (`api_key` in the URL); `Admin`: `Y`, requires admin, `B`, with or without admin, `N`, no admin required

| API Action | Arguments | Desctipion | Token | Admin |
| ------------- |:-------------:| :-----|:-------------:|:-------------:|
| `getminingandprofitsstatistics` | none | Get mining profits statistics | N | N |
| `getautoswitchingandprofitsstatistics` | none | Get current auto switching info | N | N |
| `getblockcount` | none | Get current block height in blockchain | Y | N |
| `getblocksfound` | none | Get last N blocks found as configured in admin panel | Y | N |
| `getblockstats` | none | Get pool block stats | Y | N |
| `getcurrentworkers` | none | Get amount of current active workers | Y | N |
| `getdashboarddata` | `id` | Fetch all dashboard related information | Y | N |
| `getdifficulty` | none | Get current difficulty in blockchain | Y | N |
| `getestimatedtime` | none | Get estimated time to next block based on pool hashrate (seconds) | Y | N |
| `gethourlyhashrates` | none | Currently broken | Y | N |
| `getnavbardata` | none | Get the data displayed on the navbar | Y | N |
| `getpoolhashrate` | none | Get current pool hashrate | Y | N |
| `getpoolinfo` | none | Get the information on pool settings | Y | N |
| `getpoolsharerate` | none | Get current pool share rate (shares/s) | Y | N |
| `getpoolstatus` | none | Fetch overall pool status, only user token is required | Y | N |
| `gettimesincelastblock` | none | Get time since last block found (seconds) | Y | N |
| `gettopcontributors` | none | Fetch top contributors data | Y | N |
| `getuserbalance` | `id` | Fetch a users balance | Y | Y |
| `getuserhashrate` | `id` | Fetch a users hash rate | Y | B |
| `getusersharerate` | `id` | Fetch a users share rate | Y | B |
| `getuserstatus` | `id` | Fetch a users overall status | Y | B |
| `getusertransactions` | `id` | Get a users transactions | Y | B |
| `getuserworkers` | `id` | Fetch a users worker status | Y | B |
| `public` | none | Fetch public pool statistics, no authentication required | N | N |