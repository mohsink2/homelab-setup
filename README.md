![vbox](https://github.com/user-attachments/assets/cd261640-d3b3-4e1e-8441-7d8ee2aabd2e)

# Virtual Box - Installation and Setup
An easy guide to create a home lab with active directory

## Lab Resources
* [Downloads](https://drive.google.com/drive/folders/1gu1KOeCBM6A5ZJi_9alO-m8mPiecPs_t?usp=sharing)

## Software and Technologies Used
* Windows Server 2022 Iso
* Windows 10 Iso
* Oracle VirtualBox

## Steps for Installation and Setup
* Download and Install Oracle VirtualBox
* Create a Windows Server 2022 Virtual Machine
* Create a Windows 10 Virtual Machine

## 1. Download and Setup VirtualBox
### Step 1: Download VirtualBox
* Go to the official [VirtualBox website](https://www.virtualbox.org/)
* Click on the **"Download VirtualBox"** button.
* Select the version for your operating system (Windows, macOS, Linux, etc.).
* Download the installer file.

### Step 2: Run the Installer
* Locate the downloaded installer file (usually in your "Downloads" folder).
* Double-click the file to start the installation process.

### Step 3: Begin Installation (Windows Example)
* The VirtualBox Setup Wizard will open. Click Next.
* Choose the components to install (default settings are usually fine). Click Next.
* Select where to install VirtualBox (default location is recommended). Click Next.
* You may see a warning about network interfaces. Click Yes to proceed.
* Click Install to begin the installation.

### Step 4: Complete Installation
* Wait for the installation to finish. This may take a few minutes.
* Once done, click Finish to launch VirtualBox.

## 2. Creating a Windows Server 2022 Virtual Machine
### Step 1: Prepare the Windows Server 2022 ISO
* Download the Windows Server 2022 ISO file from the official Microsoft website or the [Lab Resources](https://drive.google.com/drive/folders/1gu1KOeCBM6A5ZJi_9alO-m8mPiecPs_t?usp=sharing).
* Save the ISO file to a location on your computer (e.g., C:\ISOs\Windows_Server_2022.iso).

### Step 2: Create the Virtual Machine
* Open Oracle VirtualBox.
* Click the New button to create a new virtual machine.
* In the Name and operating system window:
  * Upload the ISO
  * Name: Windows Server 2022
  * Edition: Windows Server 2022 Standard Evaluation (Desktop Experience)
  * Type: Microsoft Windows
  * Version: Windows 2022 (64-bit)
* Click Next

### Step 3: Allocate Memory (RAM)
* Set the memory size to 4096 MB (4 GB).
* Click Next.

### Step 4: Create a Virtual Hard Disk
* Select Create a virtual hard disk now.
* Click Create.
* Choose VDI (VirtualBox Disk Image) as the hard disk file type. Click Next.
* Select Dynamically allocated (this saves space on your physical drive). Click Next.
* Set the hard disk size to 50 GB. Click Create.

### Step 5: Configure the Virtual Machine
* Select the newly created virtual machine (Windows Server 2022) in the VirtualBox Manager.
* Click Settings.
* Go to the System tab:
  * Set Processor(s) to 1.
* Go to the Network tab:
  * Click on "Adapter 2"
  * Check Enable Network Adaptor
  * Under Attached to: Select Internal Network
  * Name it: "intnet"
* Click OK to save settings.

### Step 6: Install Windows Server 2022
* Start the virtual machine by clicking Start.
* Follow the on-screen instructions to install Windows Server 2022:
  * Select your language, time, and keyboard preferences.
  * Click Install Now.
  * Follow the prompts to complete the installation.

## 3. Creating a Windows 10 Virtual Machine
### Step 1: Prepare the Windows 10 ISO
* Download the Windows 10 ISO file from the official Microsoft website or the [Lab Resources](https://drive.google.com/drive/folders/1gu1KOeCBM6A5ZJi_9alO-m8mPiecPs_t?usp=sharing).
* Save the ISO file to a location on your computer (e.g., C:\ISOs\Windows_10.iso).

### Step 2: Create the Virtual Machine
* Open Oracle VirtualBox.
* Click the New button to create a new virtual machine.
* In the Name and operating system window:
  * Upload the ISO
  * Name: Windows 10
  * Type: Microsoft Windows
  * Version: Windows 10 (64-bit).
* Click Next.

### Step 3: Allocate Memory (RAM)
* Set the memory size to 2048 MB (2 GB).
* Click Next.

### Step 4: Create a Virtual Hard Disk
* Select Create a virtual hard disk now.
* Click Create.
* Choose VDI (VirtualBox Disk Image) as the hard disk file type. Click Next.
* Select Dynamically allocated (this saves space on your physical drive). Click Next.
* Set the hard disk size to 50 GB. Click Create.

### Step 5: Configure the Virtual Machine
* Select the newly created virtual machine (Windows 10) in the VirtualBox Manager.
* Click Settings.
* Go to the System tab:
  * Set Processor(s) to 1.
* Go to the Network tab:
  * Under Attached to: Select Internal Network
  * Name it: "intnet"
* Click OK to save settings.

### Step 6: Install Windows 10
* Start the virtual machine by clicking Start.
* Follow the on-screen instructions to install Windows 10:
  * Select your language, time, and keyboard preferences.
  * Click Install Now.
  * Skip the product key.
  * Choose the "Windows 10 Pro" edition of Windows 10.
  * Follow the prompts to complete the installation.
