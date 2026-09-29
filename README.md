# Ancora-Education-Ucertify-Lab3
# Setting Up a Honeypot

A honeypot is a security system designed to detect malicious activity on a network by luring attackers with fake data or services. It is used to identify, deflect, or study malicious activity on a network. Setting up a honeypot requires careful planning and configuration to ensure it is secure and effective.(uCertify,2026)

> **Original Lab Source**
> This lab was available through:
> [https://ancoraeducation.ucertify.com/app/?func=navigate_items&item_sequence=3]

## Important Lab Instructions
Lab/Machine Environment: You are provided with the Kali virtual machine.

## Objective of the Lab
This lab session demonstrates the steps involved in setting up a honeypot. Upon completion of this lab, you will be able to: 
>Understand the concept of a honeypot and its importance in network security.
>
>Configure the honeypot to detect malicious activity.

## Instructions
## Part A: Determining the inet IP
Launch the terminal window and execute the command to view the inet IP of the eth0 router.

### STEP 1
From the left sidebar, click the Terminal icon to open its window.

### STEP 2
Execute the following command to display the network interface:
```bash
ifconfig
```
## PART B: Setting Up a Honeypot
Execute the commands to set up a honeypot with port 443 and the false message as Caught You!!.

### STEP 1
Execute the following commands to manage the directory (Note: Execute one command at a time.):
```bash
cd pentbox-1.8/
```
```bash
./pentbox.rb
```

### STEP 2
Type 2 to select the Network tools option and press Enter.

### STEP 3
Type 3 to select the Honeypot option and press Enter.

### STEP 4
Type 2 and press Enter for manual configuration.

### STEP 5
Type 443 and press Enter to open the port.

### STEP 6
Type the false message as Caught You!! and press Enter.

### STEP 7
Type y and press Enter to save the log.

### STEP 8
Press Enter to save the log file in the default location.

### STEP 9
Type n and press Enter to not activate the beep sound.
# **Note**
Here, we are opening a port and inserting a fake message. We are also providing the ability to save the record and the record’s name. As a result, you will see that the honeypot is enabled on the required port. For every attempt of intrusion that is made, it is alerted, and a log is created where the attacker’s IP and port are recorded.

## PART C: Detecting the Intrusion
Launch Firefox ESR, navigate to the inet site, and then restore the Terminal window to stop the attack..

### STEP 1
Open Firefox ESR, in the address bar, type https://<ip address>, and then press Enter.
>### **CAUTION**

### STEP 2
You will observe that the page will not load and a Secure Connection Failed message appears on the screen.

### STEP 3
Restore the Terminal window, and you will notice the INTRUSION ATTEMPT DETECTED! message appears on the screen.

### STEP 4
Press Ctrl+C to stop.

## LAB SUMMARY
This lab session provides you with a straightforward and practical understanding of how to set up a honeypot and how to configure it to detect malicious activity. Here's a summary of what you have learned: How to configure the honeypot to detect malicious activity. How to set up the appropriate security measures to protect the honeypot. Now, you are equipped with the knowledge and skills to set up a honeypot effectively, protect it from malicious activity, and analyze any data collected.(uCertify,2026)

## Disclaimer

This repository is for **educational and personal learning purposes only**.  

The original lab content belongs to **uCertify / Ancora Education** and remains their copyrighted material.  
This repository is not affiliated with, endorsed by, or sponsored by uCertify or Ancora Education.  

No copyright infringement is intended.  
Use of any tools or techniques mentioned here should only be performed in authorized, legal environments.
