🔒 Firewall Configuration on Windows
📌 Objective

Configure Windows Firewall to block inbound traffic on port 23 (Telnet) and test its effect.

🛠 Tools Used

Windows 10/11

Windows Defender Firewall with Advanced Security

📑 Steps Followed
1. Open Windows Firewall

Press Win + R, type wf.msc, and press Enter.

This opens the Windows Defender Firewall with Advanced Security console.

2. Check Existing Rules

Navigated to Inbound Rules to view active firewall rules.

3. Block Inbound Traffic on Port 23 (Telnet)

In Inbound Rules, clicked New Rule….

Selected Port → TCP → Specific Local Port: 23.

Chose Block the connection.

Applied rule to Domain, Private, and Public profiles.

Named the rule: Block Telnet.

4. Test the Rule

Used telnet localhost 23 (if Telnet Client feature installed).

Connection failed → Rule confirmed working.

5. Remove Test Rule (Optional)

Right-clicked Block Telnet rule → Delete.

📸 Screenshots (to add in repo)

Firewall console showing Inbound Rules.

Custom rule: Block Telnet.

Test attempt using Telnet (failed connection).

📖 Summary

Windows Firewall allows granular traffic filtering by ports, protocols, and applications.

Port 23 (Telnet) is blocked because it is an insecure protocol (transmits data and passwords in plaintext).

Demonstrated understanding of firewall configuration and network traffic filtering.
