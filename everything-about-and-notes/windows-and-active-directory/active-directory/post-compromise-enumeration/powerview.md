# Powerview

**Permissions: User / Administrator / SYSTEM**

## Intro

Once we get access to a machine, we can run this powerful tool to enumerate.

## Powerview

```powershell
Get-NetDomain  //Give information about the domain.

Get-NetDomainController  //Give information about the DC.

Get-DomainPolicy  //Gets the domain policy.

(Get-DomainPolicy)."system access"  // Gets the password policy of the domain.

Get-NetUser  // Get users information like descriptions, samaccountname and more. You can use select to filter.

Get-NetUser | select <field-to-filter>

Get-UserProperty  // Show all user properties that a user might have

Get-UserProperty -Property <pwdlastset> <logoncount> <badpwdcount>

Get-NetComputer -Fulldata // enumerate all the computers in the domain

Get-NetGroup -GroupName "Domain Admins" // List domain groups

Get-NetGroupMember -GroupName "Domain admins" // enum all domain admins

Invoke-ShareFinder  // Enums all the shares (smb)

Get-NetGPO  // Get all group policies
```

