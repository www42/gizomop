
Traditionell startet und stoppt man eine virtuelle Python Umgebung mit Scripts, z.B. bei einer venv Umgebung und PowerShell mit

```
 .\.venv\Scripts\Activate.ps1 -Verbose
 
 # python stuff

deactivate
```

Der ganze `python stuff` geschieht mit genau dem Python Interpreter, der der virtuellen Umgebung zugeordnet ist, und Python Pakete werden nur in der virtuellen Umgebung installiert.

Neuerdings startet VS Code automatisch virtuelle Python Umgebungen. Das finde ich intransparent, ausserdem wird im Prompt nicht - wie bisher üblich - mit `(.venv)` angezeigt, daß die virtuelle Umgebung aktiv ist.

Das automatische Aktivieren durch VS Code kann man deaktivieren mit 

```json
    "python.terminal.activateEnvironment": false,
```
