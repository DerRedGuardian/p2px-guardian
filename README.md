You can use the tool directly: [Start](https://derredguardian.github.io/p2px-guardian/P2PxGuardian.html)

<img width="1865" height="942" alt="grafik" src="https://github.com/user-attachments/assets/060f248a-5c01-4a54-92d2-d9240d008dff" />


Or download P2PxGuardian.html and open it directly in your browser; on cell phones, the link is better because of microphone usage, since local HTML files don't have access to the microphone.

IMPORTANT: You have to exchange Keys very fast. <20s otherwise the conaction will fail.


User Manual

1. Initialization (Pairing)
Before you can communicate, you must establish a P2P tunnel. One party acts as the host, and the other as the participant.
Host (Node A):
Click “INITIALIZE HOST”.
The system generates a “HOST KEY (SDP)”.
Click “COPY SECURITY KEY”.
Send this key to your partner via an external, secure channel.
Participant (Node B):
Click “JOIN PEER NODE”.
Paste the host’s key into the “INSERT HOST KEY” field.
Click “CALCULATE RESPONSE KEY”.
Copy the generated “YOUR ANSWER TOKEN” and send it back to the host.
Completion (Host):
Paste the received answer token into the “INSERT PARTNER ANSWER TOKEN” field.
Click “ACTIVATE CONNECTION”.

3. Security Configuration (AES-256 E2EE)
Encryption is at the heart of the system. To ensure that messages and images are decrypted correctly, both sides must be synchronized.
Key Entry: Enter an identical 256-bit AES password in the “256-BIT AES KEYPHRASE” field.
Generation: Use the “GEN” button to create a cryptographically secure key.
Security Check: Pay attention to the “KEY STRENGTH INDICATOR.” A secure key should be marked as “1000% HARDCORE ENCRYPTED.”

5. Tactical Communication
As soon as the status changes to “CONNECTED,” the data channel is active.
Text Messages: Enter text in the input field. Use CTRL + ENTER (or CMD + ENTER) to send the encrypted message.
File Sharing: Click the paperclip icon (“Encrypt Secure Image”) to transfer images. These are compressed and encrypted locally before passing through the tunnel.
Voice Channels: When a connection is established, the phone icon appears. Click it to request an encrypted voice connection.

Troubleshooting
If the system does not respond as expected, follow this procedure:
Status: “FAILED” or connection drops: It should usually work after a few attempts.
Tested with two independent devices logged into two different mobile networks.
Check whether you are on a network with strict NAT (e.g., restrictive corporate firewalls), although it should still work. Reconnect to the internet (this helped during testing).
“UNSECURE PROTOCOL” warning: If you’re using the tool via http:// instead of https://, microphone access and native cryptographic functions are blocked.
In this case, use text messages only, as the system automatically falls back to an XOR fallback algorithm.
Synchronization error: If messages are displayed as [DECRYPTION_ERROR], both parties are not using exactly the same password. Please double-check your input.
Display: You can adjust the height of the chat window to match your screen resolution at any time using the “CHAT HEIGHT” slider.

If you want to open a new chat or something went wrong, just reload the page!

