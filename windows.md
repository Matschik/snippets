# Windows

## Processus
### Kill process
A exécuter en tant qu'administrateur
```
# Find PID number
$ netstat -ano | findstr :<yourPortNumber>

# Kill process by PID
$ taskkill /PID <typeyourPIDhere> /F
```
