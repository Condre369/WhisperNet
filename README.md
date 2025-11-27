WhisperNet – Peer-to-Peer Encrypted Communication (Prototype)
========================================================

WhisperNet is a lightweight, serverless, peer-to-peer communication tool that runs entirely in your browser.
It uses WebRTC data channels and locally generated cryptographic keys to enable encrypted messaging, file
sharing, and image/gif previews — with no installation required.

This project is an experimental prototype and is not intended for high-security or production use.

Features
--------

- No servers required for messaging  
  Connections are established directly between browsers using WebRTC.

- End-to-end encrypted messages and files  
  Each user generates a local RSA key pair. All encryption and decryption occur on the user's device.

- Invite Code / Reply Code connection flow  
  A simplified two-step pairing system for establishing encrypted peer connections.

- Persistent identity and contacts  
  Whisper IDs, display names, and contact entries remain stored locally until browser data is cleared.

- Session memory  
  Previously successful connections can be selected and retried with one click.

- File and image sharing  
  Drag-and-drop files or images directly into the chat. Previews are shown to both sender and receiver.

- GIF link previewing  
  Links to GIFs automatically display inside the chat.

- Multi-participant rooms (prototype)  
  Hosts can add up to four participants to an encrypted Whisper Room using additional Reply Codes.

- Collapsible interface panels  
  Identity, contacts, instructions, and chat sections can be expanded or collapsed for a cleaner layout.

How It Works
------------

1. Generate your identity  
   Your browser creates an RSA key pair and Whisper ID.

2. Create an Invite Code  
   The host chooses or creates a contact and generates an Invite Code.

3. Join with a Reply Code  
   The guest pastes the Invite Code and WhisperNet generates a Reply Code to send back.

4. Encrypted connection established  
   When both codes have been exchanged, the WebRTC channel forms and the chat becomes active.

5. Optional: add more participants  
   The host may accept additional Reply Codes to add users to the Whisper Room.

Usage
-----

1. Download the `whispernet.html` file.
2. Open it in a supported browser:
   - Chrome  
   - Firefox  
   - Edge  
3. Follow the on-screen instructions to generate an identity and connect.

Security Notice
---------------

WhisperNet is experimental. Do not use it for sensitive or mission-critical communication.

Because WebRTC exposes IP addresses between peers, users who do not fully trust their contact should:

- Use a VPN  
- Avoid sharing personal information  
- Only exchange Invite and Reply Codes with trusted individuals  

Contributing
------------

Contributions, improvements, and feature suggestions are welcome.

License
-------

Copyright © 2025 Condre369.  
Licensed under the Apache License, Version 2.0.  
You may obtain a copy of the license at:

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software distributed under the License is
distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.

