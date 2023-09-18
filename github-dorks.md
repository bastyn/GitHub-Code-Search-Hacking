# Dorks

## API keys

```text
/[a|A][p|P][i|I][_]?[k|K][e|E][y|Y].*['|\"][0-9a-zA-Z]{32,45}['|\"]/
/[a|A][p|P][i|I][_]?[k|K][e|E][y|Y][\s\t\'\"]*[=:>]+[\s\t\'\"]*[a-zA-Z0-9!@#$&()-\`\\\/_\|.+,\"]{8,60}/
/[a|A][p|P][i|I][\s\t\'\"]*[=:>]+[\s\t\'\"]*[a-zA-Z0-9!@#$&()-\`\\\/_\|.+,\"]{8,60}/
/[k|K][e|E][y|Y][\s\t\'\"]*[=:>]+[\s\t\'\"]*[a-zA-Z0-9!@#$&()-\`\\\/_\|.+,\"]{8,60}/
```

### Google API keys

```text
/AIza[0-9A-Za-z\\-_]{35}/
```

### SendGrid API keys

```text
/SG\.[a-zA-Z0-9_-]{22}\.[a-zA-Z0-9_-]{43}/
```

### Slack hooks

```text
/https:\/\/hooks\.slack\.com\/services\/T[a-zA-Z0-9_]+\/B[a-zA-Z0-9_]+\/[a-zA-Z0-9_]+/
```

## Secrets

```text
/[s|S][e|E][c|C][r|R][e|E][t|T].*['|\"][0-9a-zA-Z]{32,45}['|\"]/
```

## Passwords

```text
/[p|P][w|W][d|D][\s\t\'\"]*[=:>]+[\s\t\'\"]*[a-zA-Z0-9!@#$&()-\`\\\/_\|.+,\"]{8,60}/
/[p|P][a|A][s|S][s|S][w|W][o|O][r|R][d|D][\s\t\'\"]*[=:>]+[\s\t\'\"]*[a-zA-Z0-9!@#$&()-\`\\\/_\|.+,\"]{8,60}/
/[p|P][a|A][s|S][s|S][\s\t\'\"]*[=:>]+[\s\t\'\"]*[a-zA-Z0-9!@#$&()-\`\\\/_\|.+,\"]{8,60}/
```

## Values

```text
/[v|V][a|A][l|L][u|U][e|E].*['|\"][0-9a-zA-Z]{32,45}['|\"]/
```

## Tokens

```text
/[t|T][o|O][k|K][e|E][n|N][\s\t\'\"]*[=:>]+[\s\t\'\"]*[a-zA-Z0-9!@#$&()-\`\\\/_\|.+,\"]{8,60}/
```

### JWTs

```text
/eyJ[A-Za-z0-9\-_=]+\.[A-Za-z0-9\-_=]+\.?[A-Za-z0-9\-_.+\/=]*?/
```

### GitHub tokens

```text
/[g|G][h|H][p|P|o|O|u|U|s|S|r|R]_[A-Za-z0-9_]{36}/
```

## General connection strings

```text
/:\/\/[^{}\s]+:([^{}\s]+)@/
```

## SSH private keys

```text
/BEGIN[A-Z\s]+PRIVATE KEY/
/-----BEGIN [A-Z\s]+ PRIVATE KEY-----/
```

### Putty private keys

```text
/PuTTY-User-Key-File-2/
```

## SQL credentials

### Oracle

```text
/sqlplus(.*?)[A-Za-z0-9]+\/[A-Za-z0-9]+@[a-zA-Z0-9!@#$&()-\`.+,\"]+/
```

### MySQL

```text
/mysql -u [a-zA-Z0-9!@#$&()-`.+,"]+ -p[a-zA-Z0-9!@#$&()-`.+,"]+/ 
```

### SQL Server

```text
/SQLCMD [\/-]S [a-zA-Z0-9!@#$&()-`.+,\:"]+ -U [a-zA-Z0-9!@#$&()-`.+,"]+ -P [a-zA-Z0-9!@#$&()-`.+,"]+/
```

## Azure

### SharedAccessToken

```text
/AccountKey=[a-zA-Z0-9+\/=]{88}/
/SharedAccessKey=[a-zA-Z0-9!\/\\+=]{30,50}/
/InstrumentationKey=[a-zA-Z0-9\\-]{30,50}/
```

### windows.net

```text
/[k|K][e|E][y|Y]+.*.windows.net/
/[p|P][a|A][s|S][s|S][w|W][o|O][r|R][d|D]+.*.windows.net/
/[t|T][o|O][k|K][e|E][n|N]+.*.windows.net/
/.windows.net.*[k|K][e|E][y|Y]+/
/.windows.net.*[p|P][a|A][s|S][s|S][w|W][o|O][r|R][d|D]+/
/.windows.net.*[t|T][o|O][k|K][e|E][n|N]+/
```

## AWS

```text
/[a|A][w|W][s|S][\s\t\'\"]*[=:>]+[\s\t\'\"]*[a-zA-Z0-9!@#$&()-\`\\\/_\|.+,\"]{8,60}/
```
