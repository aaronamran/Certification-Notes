---
icon: '2'
---

# Network Communication and Addressing

### MAC Addresses

* A unique identifier assigned to a device's NIC to allow the device to be recognised on the local network
* OSI model: Data link layer (layer 2)
* Ensures data reaches the correct physical device
* Each MAC address is 48 bits long as a hexadecimal. 6 pairs of hexadecimal digits separated by colons or hyphens (example 00:1A:2B:3C:4D:5E)
* First 24 bits represent the OUI (Organisationally Unique Identifier) assigned to the manufacturer, while the remaining 24 bits are specific to the individual device, which ensures every MAC address is globally unique
*   Windows command to return the MAC address of every NIC on the host:

    ```
    getmac
    ```
*
