```
mkdir -p mta_archives ; mbt build -p=cf -t=mta_archives --mtar=justjava.mtar
```

# Deploy Command:
```
cf deploy mta_archives/justjava.mtar -f
```

# Subsequent Build+Deploy Commands:
```
mbt build -p=cf -t=mta_archives --mtar=justjava.mtar ; cf deploy mta_archives/justjava.mtar -f
```

# Undeploy Command:
```
cf undeploy justjava -f --delete-services
```
