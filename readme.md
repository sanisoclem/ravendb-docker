Stand up an unsecure 3-node ravendb cluster using `docker-compose` that is only accessible from localhost.


```powershell
$ docker-compose up -d

# requires admin
$ Add-Content c:\windows\system32\drivers\etc\hosts "127.0.0.1 raven1`r`n127.0.0.1 raven2`r`n127.0.0.1 raven3`r`n"

# teardown
$ docker-compose down
```

NOTE: if using it with NServiceBus, just use two nodes as it is currently not supported.