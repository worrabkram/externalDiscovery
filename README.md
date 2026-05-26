**Micetro externalDiscovery**

externalDiscovery is a python based script developed by Sigfus Magnusson and myself (Mark Barrow). It extends Micetro network discovery capabilities using SNMP and vendor APIs where the built-in discovery engine is insufficient. 
While Micetro is continuously improving, we found that some customers still require this approach to identify and integrate unsupported or partially supported devices. The project also helps surface requirements for future product enhancements.

It supports:
•	VRF-aware discovery
•	Palo Alto PAN-OS API integration 
•	Cisco Nexus NX-API integration 
•	Fortigate FortiOS API integration
•	Custom SNMP OIDs 
•	Discovery filtering and subnet suppression
•	Device interface collection and population into IPAMDevices
•	L2 discovery using the SNMP BRIDGE-MIB

Recommended use cases:
•	Complex routed environments 
•	Multi-VRF deployments
•	Firewalls with limited SNMP support 
•	Environments requiring custom discovery logic

**Please note**
This is a personal project and is provided on an “as-is” basis without warranty or formal support.

Although we are unable to provide official support, I’m happy to answer questions and engage with the community where possible. 
I also encourage others to contribute integrations that may prove useful. 

For convenience, the script is provided as a Windows executable packaged using PyInstaller. The bundle includes the tested Python runtime along with all required dependencies and packages, allowing it to run without requiring a separate Python installation.
However, the source code can be shared with anyone interested in building their own integrations.

Micetro_External_Discovery.pdf  -  Installation and configuration instructions
externalDiscovery.exe           -  pyinstaller bundle containing externalDiscovery.py, Python 3.x and dependant packages.
                                   Requires Windows 2019 or higher
setup.json                      -  sample setup.json. Needs to be modified to match your environment
profiles.json                   -  sample profiles.json including examples for SNMP2, SNMP3, OID substitutes, PANOS API, NEXUS API and FORTI API



