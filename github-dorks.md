# Scope
```
repo:<your-repo> <dork>
org:<your-org> <dork>
```

# Show files that are most likely production environment
```
<dork> NOT path:*tst* NOT path:*test* NOT path:*dev* NOT path:*development* NOT path:*local* NOT path:*acc* NOT path:*acceptance*
```

# API keys 
```
/[a|A][p|P][i|I][_]?[k|K][e|E][y|Y].*['|\"][0-9a-zA-Z]{32,45}['|\"]/
```

## Google 
```
/AIza[0-9A-Za-z\\-_]{35}/
```

# Secrets
```
/[s|S][e|E][c|C][r|R][e|E][t|T].*['|\"][0-9a-zA-Z]{32,45}['|\"]/
```

# Passwords
```
/[p|P][a|A][s|S][s|S][w|W][o|O][r|R][d|D].*['|\"][0-9a-zA-Z]{8,45}['|\"]/
```

# Value
```
/[v|V][a|A][l|L][u|U][e|E].*['|\"][0-9a-zA-Z]{32,45}['|\"]/
```

# Private keys
```
/-----BEGIN [A-Z\s]+ PRIVATE KEY-----/
```

# SQL credentials

## Oracle
```
/sqlplus(.*?)[A-Za-z0-9]+\/[A-Za-z0-9]+@[a-zA-Z0-9!@#$&()-`.+,"]+/
```

## MySQL
```
/mysql -u [a-zA-Z0-9!@#$&()-`.+,"]+ -p[a-zA-Z0-9!@#$&()-`.+,"]+/ 
```

## SQL Server
```
/SQLCMD [\/-]S [a-zA-Z0-9!@#$&()-`.+,\:"]+ -U [a-zA-Z0-9!@#$&()-`.+,"]+ -P [a-zA-Z0-9!@#$&()-`.+,"]+/
```

# Azure

## SharedAccessToken
```
/SharedAccessKey=[a-zA-Z0-9!\/@#$&()-`.+,"]+;/
/SharedAccessKey=[a-zA-Z0-9!\/@#$&()-`.+,"]+;/
/InstrumentationKey=[a-zA-Z0-9-]+;/
/AccountKey=[a-zA-Z0-9!\/@#$&()-`.+,"]+;/
/SharedAccessKey=[a-zA-Z0-9!\/@#$&()-`.+,"]+;/
/InstrumentationKey=[a-zA-Z0-9-]+;/
```