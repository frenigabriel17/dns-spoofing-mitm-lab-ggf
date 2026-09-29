# dns-spoofing-mitm-lab-ggf
Cybersecurity lab demonstrating ARP spoofing, DNS spoofing, and HTTP traffic redirection using Kali Linux, Bettercap, and Apache, to test security and how the process works behind the curtains.


# DNS Spoofing & MITM Laboratory

## Overview

This project documents a controlled cybersecurity laboratory demonstrating DNS spoofing and Man-in-the-Middle concepts.

The laboratory uses Kali Linux, Bettercap, Apache2, and an Iphone device in a controlled network environment.

The objective is to understand how ARP spoofing, DNS resolution, HTTP traffic, and TLS interact during a network interception scenario.

> **Disclaimer:** This laboratory was performed only on devices and network infrastructure under my control for educational purposes.

---

## Objectives

* Understand ARP spoofing.
* Understand Man-in-the-Middle attacks.
* Understand DNS spoofing.
* Configure an Apache web server.
* Redirect controlled HTTP traffic to a local server.
* Analyze the limitations imposed by HTTPS and TLS.
* Practice Linux networking and troubleshooting.
* Document a cybersecurity laboratory using Git and GitHub.

---

## Lab Environment

| Component     | Role                     |
| ------------- | ------------------------ |
| Kali Linux    | Security testing machine |
| Iphone phone | Controlled test device   |
| Bettercap     | MITM and DNS spoofing    |
| Apache2       | Local web server         |
| Wi-Fi router  | Laboratory network       |

---

## Network Topology

```text
                 Wi-Fi Router
                      |
          +-----------+-----------+
          |                       |
    Android Phone             Kali Linux
       Test Device             Security Lab
                                    |
                                Bettercap
                                    |
                                 Apache2
```

---

## Technologies

* Kali Linux
* Bettercap
* Apache2
* DNS
* ARP
* HTTP
* HTTPS / TLS
* TCP/IP
* Git
* GitHub

---

## Methodology

The laboratory will demonstrate the following process:

1. Identify devices in the laboratory network.
2. Identify the Iphone test device.
3. Configure an ARP-based MITM scenario.
4. Intercept network traffic.
5. Configure DNS spoofing for a controlled HTTP test.
6. Redirect the test domain to the local Apache server.
7. Display a custom laboratory webpage.
8. Analyze the limitations of the technique.

---

## Results

Screenshots and evidence from the laboratory will be added here as the experiment is completed.

---

## HTTPS Considerations

DNS spoofing changes the IP address returned during DNS resolution.

It does not automatically bypass TLS certificate validation.

When HTTPS is used, the browser validates the certificate presented by the destination server. Redirecting an HTTPS domain to an unrelated server will therefore normally result in a certificate validation error.

This laboratory focuses on understanding DNS manipulation, MITM concepts, HTTP redirection, and the security provided by TLS.

---

## Lessons Learned

This laboratory is intended to provide practical experience with:

* Linux networking
* DNS
* ARP
* HTTP
* HTTPS
* MITM concepts
* Apache administration
* Bettercap
* Network troubleshooting
* Technical documentation
* Git and GitHub

---

## Ethical Considerations

This project is intended exclusively for authorized cybersecurity education and laboratory environments.

The techniques demonstrated should only be used against systems and networks for which the tester has explicit authorization.
