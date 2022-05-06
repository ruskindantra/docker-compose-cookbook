h2. Redis Commands
[Redis cheatsheet](https://simplecheatsheet.com/tag/redis-cheat-sheet/)
1. Switch databases in redis [Link](https://stackoverflow.com/questions/13386053/how-do-i-change-between-redis-database)
    `select n` where n is a number between 0-15
1. Return all keys
    `keys *`
1. Simple set
    `set key_name value`
1. Simple get
    `get key_name`

h2. Understanding transactions
1. https://stackexchange.github.io/StackExchange.Redis/Transactions.html
1. https://redis.io/docs/manual/programmability/eval-intro/
1. https://www.w3resource.com/redis/redis-exec.php