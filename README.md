Enterprise Asterisk PBX Configuration

📱 Overview
A complete Asterisk PBX configuration setup designed for enterprise environments, featuring departmental organization, IVR menus, voicemail systems, and queue management. This configuration demonstrates a professional-grade VoIP telephony system implementation.

🎯 Features

Department-based Structure
- Reception (1XXX)
- Management (2XXX)
- Human Resources (3XXX)
- Production (4XXX)
- Marketing (5XXX)

Core Functionality
- ✨ Interactive Voice Response (IVR) System
- 📧 Voicemail with Email Integration
- 👥 Call Queues for Sales and Customer Support
- 🔄 Ring Groups
- 📞 Extension-to-Extension Dialing
- 🎵 Music on Hold
- 📊 Call Detail Records (CDR)

🛠 Technical Configuration

SIP Configuration
- PJSIP-based configuration
- Secure authentication
- NAT traversal support
- UDP transport on port 5060

RTP Settings
- Port range: 10000-20000
- Binding on all interfaces

Security Features
- Password protection for extensions
- Limited contact registration
- Network access control

📁 File Structure

asterisk/
├── asterisk.conf       Core configuration
├── pjsip.conf         SIP endpoint configuration
├── extensions.conf    Dialplan configuration
├── voicemail.conf    Voicemail settings
├── queues.conf       Queue management
├── modules.conf      Module loading preferences
└── various other configuration files


🚀 Implementation Details

IVR Menu Structure
1. Main Menu (9000)
   - 1 → Reception
   - 2 → Management
   - 3 → Human Resources
   - 4 → Production
   - 5 → Marketing
   - 0 → Operator

Voicemail Features
- Direct voicemail access (`*XXXX`)
- Email notifications
- Multiple formats support (wav49, wav, gsm)
- Custom greetings
- Time zone support

Queue Management
- Ring-all strategy for sales team
- Customer advocate queue system
- Customizable hold music
- Agent monitoring

📋 Prerequisites
- Asterisk 18.0 or higher
- Linux-based operating system
- Sufficient network bandwidth
- SIP-compatible phones or softphones

🔧 Installation

1. Clone this repository:

git clone https://github.com/mwizerwahf/VoIP-asterisk/.git

2. Copy configuration files:

cp -r * /etc/asterisk/


3. Set proper permissions:

chown -R asterisk:asterisk /etc/asterisk


4. Reload Asterisk:

asterisk -rx "core reload"


 🔒 Security Considerations
- Change default passwords
- Implement firewall rules
- Regular security audits
- Monitor for suspicious activity
- Keep Asterisk updated

📄 License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

✨ Acknowledgments
- Asterisk Community
- PJSIP Team
- VoIP Security Project

 📞 Contact
MWIZERWA Honore Frank 
mwizerwahonorefrank@gmail.com

Project Link: https://github.com/mwizerwahf/VoIP-asterisk/
