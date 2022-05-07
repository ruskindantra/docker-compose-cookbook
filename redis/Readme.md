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
1. https://kb.objectrocket.com/redis/how-to-use-the-redis-watch-command-695

h2. Redis UIs
1. https://www.npmjs.com/package/redis-commander

h2. Connecting to Redis
1. Use local `redis-cli`
    1. Installed via HomeBrew using `brew install redis`
1. Connecting to ElastiCache
    1. Note cannot connect to ElastiCache unless using VPC, [ref](https://docs.aws.amazon.com/AmazonElastiCache/latest/mem-ug/accessing-elasticache.html)
    1. Use port forwarding [ref](https://aws.amazon.com/blogs/aws/new-port-forwarding-using-aws-system-manager-sessions-manager/)
        1. Helpful GitHub [repo](https://github.com/aws-samples/aws-systems-manager-port-forwarding-for-amazon-elasticache)
    1. More on Port Forwarding [ref](https://www.ssh.com/academy/ssh/tunneling/example#what-is-ssh-port-forwarding,-aka-ssh-tunneling?)
1. Connecting to Redis Cluster Mode enabled
    1. `redis-cli -h XXXX -c` as `-c` is for Cluster Mode
1. Using Redis UI
1. NB: Sometimes ports can be blocked depending on where you connect from, be aware of any proxies/firewall settings

h2. Other notes
1. Running Redis in ElastiCache
    1. https://docs.aws.amazon.com/AmazonElastiCache/latest/red-ug/accessing-elasticache.html#access-from-outside-aws
    1. https://docs.aws.amazon.com/AmazonElastiCache/latest/red-ug/GettingStarted.ConnectToCacheNode.html
1. Running Redis via HomeBrew
    1. https://redis.io/docs/getting-started/installation/install-redis-on-mac-os/
    1. `brew services start redis`
    1. `brew services info redis`
    1. `brew services stop redis`