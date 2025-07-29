<p align="center">
<img src="https://i.imgur.com/Hxx4wak.png" height="50%" width="50%" alt="Traffic Examination"/>
</p>

# VPN (Virtual Private Network) Setup and Analysis
This covers Virtual Private Networks (VPNs) and how they help secure remote access to a network. <br />

## 🧰 Environments & Technologies Used

- VPN (Proton VPN/Windscribe)
- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop

---

## 💻 Operating System

- Windows 10 (21H2)

---

## 🔧 High-Level Process

- Identify Local IP Address
- Deploy a Virtual Machine in Microsoft Azure
- Verify Public IP from VM
- Connect to a VPN via the VM
- Confirm New IP Address via VPN

---

## 🔍 Steps & Observations

<p>
<img src="https://i.imgur.com/EJuAMFn.png" height="60%" width="60%" alt="Disk Sanitization Steps"/>
</p>
<p>
To confirm the network identity of your own computer (outside of any virtual machines or VPNs):

Open any web browser (Chrome, Edge, Firefox, etc.).

Go to: https://whatismyipaddress.com

The site will display your public IP address, location, and Internet Service Provider (ISP).

This is helpful for understanding the baseline network location of your local device—before introducing VPNs or cloud-based virtual machines.

</p>
<br />

<p>
<img src="https://i.imgur.com/BNWKykA.png" height="60%" width="60%" alt="Disk Sanitization Steps"/>
</p>
<p>

- Click Create a resource > Virtual Machine and select Windows 10.
- Choose a geographic region to host the VM.
- Review your settings and click Create to launch the VM.
- Connect using RDP with the VM’s public IP and your credentials.
</p>
<br />

<p>
<img src="https://i.imgur.com/c9cbxwM.png"60%" width="60%" alt="Disk Sanitization Steps"/>
</p>
<p>
  
- Launch a browser from within the VM.  
- Visit [whatismyipaddress.com](https://whatismyipaddress.com).  
- Note the IP, location, and ISP for the VM (pre-VPN).
  
</p>
<br />

<p>
<img src="https://i.imgur.com/J7k9nsu.png" height="40%" width="40%" alt="Disk Sanitization Steps"/>
</p>
<p>

- Download and install a free VPN (e.g., ProtonVPN or Windscribe).  
- Select a region (different from the VM’s region) and connect.

</p>
<br />

<p>
<img src="https://i.imgur.com/aksjhdJ.png" height="60%" width="60%" alt="Disk Sanitization Steps"/>
</p>
<p>

- Open a browser in the VM.  
- Visit [whatismyipaddress.com](https://whatismyipaddress.com).  
- A new public IP and location should appear—matching the VPN region.

</p>
<br />

## 📝 Summary

Set up cloud-based Windows 10 virtual machines with VPNs to simulate different geographic locations and demonstrate IP/geolocation changes for privacy, testing, and networking use cases.
