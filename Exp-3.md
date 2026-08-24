# Password Capturing Using Wireshark

## Experiment No. 3

## Aim

To capture and analyze login credentials transmitted through network traffic using the Wireshark network capture analyzer.

> ⚠️ **Note:** This experiment should only be performed in an authorized lab environment, on systems you own, or on a deliberately vulnerable test website.

---

# Introduction

Wireshark can capture not only passwords but also different types of information transmitted over a network, such as:

- Usernames
- Email addresses
- Personal information
- Other network data

As long as network traffic can be captured, transmitted data may be visible depending on the protocol being used.

Sniffing can include passwords transmitted through protocols such as:

- HTTP
- FTP
- Telnet

Captured data can be used for troubleshooting network problems, but it can also be misused to gain unauthorized access to sensitive information.

In this experiment, we use the Wireshark network capture analyzer to observe the network traffic generated during a login operation and inspect the captured HTTP form data.

---

# Requirements

- Wireshark
- Internet connection
- Web browser
- Active network interface
- Authorized test website

---

# Procedure

## Step 1: Open Wireshark

First, open the Wireshark tool on Windows or Linux.

Select the active network interface.

In this experiment, the **Wi-Fi** interface was selected for capturing network traffic.

Start the packet capture.

### Output

<img width="793" height="597" alt="1" src="https://github.com/user-attachments/assets/7ff19f5a-326d-4658-ac8b-e0763b2f110f" />
---

## Step 2: Open the Test Website

After starting packet capture, open the authorized test website in a web browser.

Navigate to the login page.

Enter the login credentials provided by the test environment and click the **Login** button.

### Output

<img width="995" height="928" alt="4" src="https://github.com/user-attachments/assets/2c9ffbd9-c5f7-40ca-8ce1-921b8ca9e07e" />
---

## Step 3: Analyze the Captured Packets

After completing the login process, return to Wireshark.

Wireshark captures many different types of network packets.

To specifically analyze HTTP traffic, use a display filter.
<img width="1892" height="562" alt="5" src="https://github.com/user-attachments/assets/ea39f1f9-1f5a-47f5-aa1e-13f1c4148dd0" />


---

## Step 4: Apply the HTTP Filter

In the Wireshark display filter bar, enter:
<img width="685" height="303" alt="6" src="https://github.com/user-attachments/assets/a8e020f6-de2c-45d3-a81b-98652a3420bc" />


```text
http
