# Akka Docs Offline

Backup akka docs for offline usage.
- Upstream is also trying to provide offline docs: https://github.com/akka/akka/issues/22728
- Download zip: https://github.com/xieyuheng/akka-docs-offline/archive/master.zip

Backup akka: (2.5.23)
``` sh
httrack -n https://doc.akka.io/docs/akka/current/index.html -r6
```

Backup akka-http: (10.1.9)
```
httrack -n https://doc.akka.io/docs/akka-http/current/ -r100
```

Clean up:
```
sh delete-cookie-banner.sh
```
