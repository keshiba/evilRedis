What is Redis?
--------------
To answer that question, go to - [redis/redis repository](https://github.com/redis/redis)


What is evilRedis?
------------------
evilRedis is the devil re-incarnation .... umm, blah blah.

Why evilRedis?
---------------
1. Was bored
2. Needed to re-learn C
3. I knew much about redis and thought that it would be the apt playground to learn c again
4. Was exploiting buffer overflows and writing shellcodes recently (harmless CTFs of course)
5. All of that just came together I guess

#### It was an accident! Honestly...

How it works?
-------------


### Horn #1 - Taming `echo`

Pass in your shell command using redis's `echo` command along with a trigger keyword.
```
# Normal echo behavior
> echo whoami
whoami

# Shell execution is triggered with the keyword "evilRedisCmd:"
> echo evilRedisCmd:whoami
keshiba\n
```
When evilRedis finds the trigger keyword, it will try to execute the command that follows in the shell and returns the output.
Fun right?


Stay tuned for more...

Until then,
Enjoy!
