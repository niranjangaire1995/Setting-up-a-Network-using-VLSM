# Challenges Faced and Solutions  

## 1. IP Collision Error on Router Interfaces  
**Issue:**  
- When assigning IP addresses, instead of distributing them across two routers for interconnection, I mistakenly assigned both IPs to two different interfaces on the same router.  
- This caused an **IP collision error**, preventing proper routing.  

**Solution:**  
- Used the `show ip interface brief` command to analyze the IP assignments.  
- Reassigned the IP addresses correctly—one per router interface instead of assigning both to the same router.  
- Verified successful inter-router communication by pinging the neighboring router.  

---

## 2. Unable to Ping Across Different Networks  
**Issue:**  
- A PC in one city could not communicate with PCs or switches in other cities.  
- The root cause was **missing OSPF configuration** on each router, meaning they weren’t sharing routing information.  

**Solution:**  
- Implemented OSPF on all routers using the command:  
  ```plaintext
  router ospf 1  
  network 172.30.0.0 0.0.255.255 area 0
  ### **3. Default Gateway Not Assigned to Switches**

**Issue:**  
Switches didn’t have a default gateway, causing them to be unable to communicate beyond their local subnet.

**Solution:**  
Assigned default gateways on all switches using:  
```plaintext
Switch(config)# ip default-gateway 172.30.x.1  

