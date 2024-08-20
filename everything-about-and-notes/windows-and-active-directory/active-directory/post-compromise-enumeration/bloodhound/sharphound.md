# SharpHound

**Permissions: User / Administrator / SYSTEM**

## Intro

Is a tool used to grab data from the domain once you have a compromise machine.

### Download

* [https://github.com/BloodHoundAD/BloodHound/blob/master/Collectors/SharpHound.ps1](https://github.com/BloodHoundAD/BloodHound/blob/master/Collectors/SharpHound.ps1)

### Command

```powershell
Invoke-BloodHound -CollectionMethod All -Domain domain.local -ZipFileName file.zip
```
