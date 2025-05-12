# VLSM Network Design

## **NET ID to Start with**: 172.30.0.0/16

---

### **1. San Francisco Router (Largest Hosts Requirement: 5996)**

- **Hosts Required**: 5996  
- **Subnet Mask**: 255.255.0.0 = 11111111.11111111.00000000.00000000  
- **Formula**: 2^n - 2 ≥ 5996  
  → **n = 13**

- **Burrowing Bits**:
    ```
    11111111.11111111.000|00000.00000000
    ```
    → **New Subnet Mask**: 255.255.224.0  
    → **CIDR**: /19  
    → **Magic Number**: 256 - 224 = 32

- **Next NETID**: 172.30.32.0

---

### **2. Miami Router (Hosts Required: 1080)**

- **Hosts Required**: 1080  
- **Subnet Mask**: 255.255.224.0 = 11111111.11111111.11100000.00000000  
- **Formula**: 2^n - 2 ≥ 1080  
  → **n = 11**

- **Burrowing Bits**:
    ```
    11111111.11111111.11111|000.00000000
    ```
    → **New Subnet Mask**: 255.255.248.0  
    → **CIDR**: /21  
    → **Magic Number**: 256 - 248 = 8

- **Next NETID**: 172.30.40.0

---

### **3. Chicago Router (Hosts Required: 210)**

- **Hosts Required**: 210  
- **Subnet Mask**: 255.255.248.0 = 11111111.11111111.11111000.00000000  
- **Formula**: 2^n - 2 ≥ 210  
  → **n = 8**

- **Burrowing Bits**:
    ```
    11111111.11111111.11111111.|00000000
    ```
    → **New Subnet Mask**: 255.255.255.0  
    → **CIDR**: /24  
    → **Magic Number**: 256 - 255 = 1

- **Next NETID**: 172.30.41.0

---

### **4. New York Router (Hosts Required: 75)**

- **Hosts Required**: 75  
- **Formula**: 2^n - 2 ≥ 75  
  → **n = 7**

- **Burrowing Bits**:
    ```
    11111111.11111111.11111111.1|0000000
    ```
    → **New Subnet Mask**: 255.255.255.128  
    → **CIDR**: /25  
    → **Magic Number**: 256 - 128 = 128

- **Next NETID**: 172.30.41.128

---

### **5. Router Connections (Each Router Needs 4 IPs)**

- **Formula**: 2^n ≥ 4  
  → **n = 2**

- **Burrowing Bits**:
    ```
    11111111.11111111.11111111.111111|00
    ```
    → **Subnet Mask**: 255.255.255.252  
    → **CIDR**: /30  
    → **Magic Number**: 256 - 252 = 4

- **Next NETID**: 172.30.41.132

---

## **Listing All NETIDs with Subnet Masks and CIDR Notation:**

### **1. San Francisco Router (NETID: 172.30.0.0/19)**

- **Hosts Required**: 5996  
- **Subnet Mask**: 255.255.224.0  
- **CIDR**: /19  
- **Default Gateway**: 172.30.0.1/19  
- **First Host IP**: 172.30.0.2/19  
- **Last Usable IP**: 172.30.31.254/19  
- **Broadcast Address**: 172.30.31.255/19

---

### **2. Miami Router (NETID: 172.30.32.0/21)**

- **Hosts Required**: 1080  
- **Subnet Mask**: 255.255.248.0  
- **CIDR**: /21  
- **Default Gateway**: 172.30.32.1/21  
- **First Host IP**: 172.30.32.2/21  
- **Last Usable IP**: 172.30.39.254/21  
- **Broadcast Address**: 172.30.39.255/21

---

### **3. Chicago Router (NETID: 172.30.40.0/24)**

- **Hosts Required**: 210  
- **Subnet Mask**: 255.255.255.0  
- **CIDR**: /24  
- **Default Gateway**: 172.30.40.1/24  
- **First Host IP**: 172.30.40.2/24  
- **Last Usable IP**: 172.30.40.254/24  
- **Broadcast Address**: 172.30.40.255/24

---

### **4. New York Router (NETID: 172.30.41.0/25)**

- **Hosts Required**: 75  
- **Subnet Mask**: 255.255.255.128  
- **CIDR**: /25  
- **Default Gateway**: 172.30.41.1/25  
- **First Host IP**: 172.30.41.2/25  
- **Last Usable IP**: 172.30.41.126/25  
- **Broadcast Address**: 172.30.41.127/25

---

## **Router Connections:**

### **1. Connection Between Routers (NETID: 172.30.41.128/30)**

- **San Francisco to Chicago**: Port G0/0: 172.30.41.129/30  
- **San Francisco to New York**: Port G0/1: 172.30.41.130/30  
- **Broadcast Address**: 172.30.41.131/30

---

### **2. Miami to New York and Miami to Chicago (NETID: 172.30.41.132/30)**

- **Miami to New York**: 172.30.41.133/30  
- **Miami to Chicago**: 172.30.41.134/30  
- **Broadcast Address**: 172.30.41.135/30

---

### **3. New York to San Francisco and New York to Miami (NETID: 172.30.41.136/30)**

- **New York to San Francisco**: 172.30.41.137  
- **New York to Miami**: 172.30.41.138  
- **Broadcast Address**: 172.30.41.139

---

### **4. Chicago to San Francisco and Chicago to Miami (NETID: 172.30.41.140/30)**

- **Chicago to San Francisco**: 172.30.41.141  
- **Chicago to Miami**: 172.30.41.142  
- **Broadcast Address**: 172.30.41.143

---
