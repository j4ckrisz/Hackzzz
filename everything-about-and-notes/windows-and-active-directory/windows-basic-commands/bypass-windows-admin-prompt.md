# Bypass Windows Admin Prompt

* Using the following batch script, the program you are trying to install will be installed as your current user. **(Without admin privileges)**

```batch
Set __COMPAT_LAYER=RunAsInvoker
Start "program_name".exe
```
