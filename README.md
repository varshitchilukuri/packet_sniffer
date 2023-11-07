# Network Packet Sniffer

This is a simple network packet sniffer tool that captures HTTP requests and looks for potential login information in the packet payload. It utilizes the `scapy` library to intercept network traffic.

## Prerequisites

Before running the script, make sure you have the following requirements installed:

- Python 3
- `scapy` library

You can install `scapy` using pip:

```shell
pip install scapy
```

## Usage

1. Clone the repository:

   ```shell
   git clone https://github.com/varshitchilukuri/packet_sniffer.git
   ```

2. Navigate to the project directory:

   ```shell
   cd your-repo
   ```

3. Run the script with root privileges (as it requires packet capturing capabilities):

   ```shell
   sudo python packet_sniffer.py
   ```

## Functionality

- The script listens to network traffic on the specified network interface (e.g., "eth0") using the `scapy` library.

- It captures HTTP requests and extracts the requested URL.

- If the packet payload contains potential login information, such as usernames or passwords, it will print this information to the console.

Please note that this script should be used responsibly and only on networks and systems where you have permission to capture and analyze traffic.

## Customization

You can customize the network interface to monitor by modifying the `sniff("eth0")` line in the script. Change "eth0" to the name of the interface you want to sniff.

## Disclaimer

**Use this tool responsibly and only on networks and systems where you have explicit permission to monitor and capture network traffic. Unauthorized interception of network traffic may violate privacy and legal regulations.**

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Contribution

Feel free to contribute to this project by creating issues, providing feedback, or submitting pull requests.

If you find any issues or have suggestions for improvements, please [create an issue](https://github.com/yourusername/your-repo/issues) on the project's GitHub repository.

---

Happy packet sniffing responsibly! 🕵️🌐
