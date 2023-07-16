# Host Scan

This script performs a ping sweep on the local network to identify active hosts. It sends ICMP echo requests (pings) to a range of IP addresses and displays the active hosts.

## Prerequisites

- `bash` shell
- `ping` utility

## Usage

1. Open a terminal.
2. Navigate to the directory containing the script.
3. Run the following command:

   ```bash
   ./hostScan.sh
   ```

## Description

The script uses a loop to send ICMP echo requests to a range of IP addresses on the local network. It starts with the address `192.168.1.1` and goes up to `192.168.1.254`. Each IP address is pinged with a timeout of 1 second.

If a host responds to the ping, the script displays a message indicating that the host is active. The output will be in the following format:

```
[+] Host <IP_ADDRESS> - ACTIVE
```

## Exiting the Script

To exit the script, press `Ctrl+C`. This will interrupt the script execution and display a message indicating that the script is exiting.

```plaintext
[!] Saliendo...
```

## Notes

- Make sure you have sufficient permissions to execute the script and use the `ping` utility.
- The script may take some time to complete, depending on the network size and the responsiveness of the hosts.
- The output will only show hosts that respond to ICMP echo requests. Some hosts may have ICMP disabled or may be configured to ignore such requests.

Feel free to modify the script to suit your specific requirements. Happy pinging!
