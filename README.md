# SADP

## Introduction

SADP (Search Active Device Protocol) is a network utility designed for discovering, configuring, and managing devices within a local network segment. It is commonly used to identify devices that do not yet have a known IP configuration or are deployed with default network settings. The tool operates by broadcasting discovery packets across the subnet and collecting responses from compatible devices, allowing administrators to quickly obtain device information without prior connectivity setup.

The interface presents a tabular view of detected devices, including parameters such as IP address, subnet mask, gateway, MAC address, firmware version, and activation status. This visibility enables rapid auditing of newly installed or reset devices. SADP is particularly useful in scenarios where devices are inaccessible due to unknown addressing or misconfigured network parameters.

One of the core capabilities of SADP is device activation and initial configuration. Devices that are not yet activated can be assigned secure credentials and configured with valid network settings directly from the tool. This reduces the need for manual console access or vendor-specific initialization workflows.

The utility supports batch operations, allowing administrators to modify network parameters for multiple devices simultaneously. This is essential in large-scale deployments where consistent configuration must be applied efficiently. SADP also provides filtering and sorting mechanisms to isolate devices based on specific attributes.

Overall, SADP simplifies early-stage device management and troubleshooting by providing direct visibility and control over network-connected endpoints in a controlled and efficient manner.

## Device Discovery and Identification

SADP performs device discovery using broadcast-based communication within the local subnet. When launched, it continuously scans the network and populates a list of detected devices in real time. Each entry includes critical metadata such as IP address, MAC address, device type, port, and activation state. This eliminates the need for manual network scanning or guessing device addresses.

In practical use, administrators can connect multiple devices to a switch without preconfiguring IP addresses. SADP will automatically detect them, even if they are on different default IP ranges, as long as they respond to the discovery protocol. This is particularly useful during initial deployment or after factory resets.

The filtering functionality allows narrowing down results based on criteria such as IP range or activation status. For example, filtering unactivated devices helps quickly identify which units still require initialization. Sorting by MAC address or IP can assist in mapping physical devices to logical entries, especially when working with labeled hardware.

Another important feature is the ability to refresh the device list without restarting the application. This ensures that newly connected devices appear immediately. In environments with frequent changes, such as testing labs, this dynamic update capability improves workflow efficiency.

By providing structured visibility into all compatible devices on the network, SADP serves as a centralized discovery tool that reduces setup time and minimizes configuration errors.

## Network Configuration and Activation

SADP enables direct configuration of network parameters for one or multiple devices. After selecting a device, administrators can modify its IP address, subnet mask, gateway, and port settings. These changes are applied instantly after authentication, allowing rapid alignment with the target network topology.

For uninitialized devices, SADP provides an activation workflow. This involves setting a secure password that meets defined complexity requirements. Once activated, the device becomes fully configurable and accessible through standard management interfaces. This step is mandatory in secure environments to prevent unauthorized access using default credentials.

Batch configuration is a key feature for scalability. Administrators can select multiple devices and apply consistent network settings in one operation. For example, assigning sequential IP addresses to a group of cameras can be done efficiently without accessing each device individually.

SADP also supports exporting and importing device lists, which can be useful for documentation or migration scenarios. In troubleshooting cases, incorrect IP configurations can be quickly corrected by reassigning valid parameters through the tool.

A common use case involves recovering devices that are unreachable due to subnet mismatch. By connecting a workstation to the same physical network, SADP can detect the device and reconfigure its IP settings to match the desired range.

These capabilities make SADP a practical tool for both initial deployment and ongoing network maintenance.
