# Discovery Scan for an Entire Subnet using the Tenable platform

![green-radar-hud-radar-display-of-radar-vector-44508896](https://github.com/user-attachments/assets/3837549d-15cc-4b70-bf13-386b11da4c74)

Project demonstrating how to create a **Host Discovery Scan** with the Tenable/Nessus platform to identify active hosts within a specific subnet range of a **virtual network in Azure**.

_**Inception State:**_ No scan configured to discover subnets.

_**Completion State:**_ Subnet scan created, targets identified, scan launched, and discovery results obtained.

---

# Technology Utilized
- **Tenable** – Cloud-based vulnerability management and scanning platform
- **Azure Virtual Network** – Source of the subnet for scanning
- **Internal Network Scanner** – Configured in Tenable

![Screenshot 2025-06-07 111407](https://github.com/user-attachments/assets/8470b8ce-40b4-4b6c-839c-86b3887f4844)

---

## 1. Creating the Scan in Tenable✅

**First, we navigate to the scan creation page in Tenable:** ✅

![1-In Tenable we are going to create a scan](https://github.com/user-attachments/assets/cb48323e-e1d1-4f65-9c7a-a343b1289f2b)

**Select the “Host Discovery” scan template:** ✅

![2- Select Host Discovery Scan](https://github.com/user-attachments/assets/5b06a698-fb69-4320-ada9-56daca7066bb)

---

## 2. Identify Subnet Target in Azure

**In the Azure portal, navigate to the “Virtual Networks” section:** ✅

![3- In Azure go to virtual networks](https://github.com/user-attachments/assets/cb4e1b5a-7b1e-4270-b42b-a7d946d44ed9)

**Locate the specific subnet of your virtual network to scan:** ✅

![4- Copied the Subnet of the Virtual Network from my company](https://github.com/user-attachments/assets/1e03e043-e32b-4e0a-a99b-bf8aff73cde5)

---

## 3. Configuring the Scan in Tenable✅

**Back in Tenable, edit the scan and name it appropriately:** ✅

![5- Editing and Naming the Scan](https://github.com/user-attachments/assets/4ccd1310-3f77-4bb7-af06-c7f72e708781)

**Paste the subnet CIDR block (e.g., `10.0.0.0/21`) into the “Targets” section:** ✅

![6- Pasting the Subnet in the Target space](https://github.com/user-attachments/assets/cc241520-fd88-45bd-9e26-7823152c9121)

**Save and launch the scan:** ✅
 
![7- Saved and Launched Scan](https://github.com/user-attachments/assets/adfebc7f-613f-483c-ad49-f509527aa814)

---

## 4. Scan Progress and Results✅

**The scan starts running and progress can be seen in Tenable:** ✅

![8- Scan In Process](https://github.com/user-attachments/assets/f20f6fab-6dba-4eb5-9257-3d5bb96e4aef)

---

## 5. Scan Completion and Results✅

**Once the scan completes, Tenable marks it as “Completed”:** ✅

![9- Scan Completed](https://github.com/user-attachments/assets/065cfc64-7608-464a-97b4-c278c57f58fa)

**View the results to see the assets discovered in the subnet:** ✅

![10- Results - Assets that were actually discovered](https://github.com/user-attachments/assets/b32e2a61-7b8a-4d0e-930d-c3dd3cd9203a)

---

## 6. Tagging Discovered Assets✅

**In Tenable, go to the asset’s details page to tag it for better management and classification (I don't have permissions to add a tag):** ✅

![11- Tagging Process](https://github.com/user-attachments/assets/fc407ac0-263f-4a30-94c5-16ec368686d9)

**Purpose of Tagging in Subnet Discovery Scan
Tagging in vulnerability management and asset discovery platforms like Tenable serves a crucial role in organizing, categorizing, and managing scanned assets. Here’s why it’s important in the Subnet Discovery Scan you just completed:**

**✅ Organizational Clarity
When you scan large subnets or networks, you might find multiple hosts with different roles (e.g., production servers, testing VMs, personal workstations). Tags help you quickly identify and group these assets based on shared characteristics like hostname, IP address, environment (production, staging, dev), or asset type.**

**✅ Streamlined Vulnerability Management
Tagging allows you to filter and prioritize vulnerabilities based on asset importance. For example, a critical vulnerability on a production asset should be addressed faster than one on a test machine. Tagging makes this easier to track.**

**✅ Improved Reporting and Automation
By tagging assets, you can generate targeted reports for specific groups. If your manager wants a report only on critical production assets, tags help you filter that data quickly. You can also integrate tags with automated workflows in security orchestration tools.**

**✅ Contextual Awareness for Response Teams
Security teams can quickly understand the context of an asset (e.g., what environment it belongs to or what service it runs) by looking at the tags. This helps during incident response, patching, and risk assessments.**

**❌No Owner for Device? Rogue Asset!✅**

**Isolate: Disconnect the rogue device from your network to prevent any unauthorized access.✅**

**Investigate: Analyze the device to understand its purpose and security status using network scanning tools.✅**

**Decide: Follow your organization's security policies to either remove or secure and reintegrate the device.✅**

![R](https://github.com/user-attachments/assets/15a0c50e-9055-44de-9dee-949266ab6f79)
