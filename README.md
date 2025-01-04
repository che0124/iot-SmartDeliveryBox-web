# IoT SmartDeliveryBox

A smart delivery box system that leverages IoT technology to enhance the delivery and pickup experience. It integrates electronic lock control and a web-based user interface to provide security and convenience.



## 📦 Project Overview

**IoT SmartDeliveryBox** is a smart delivery box designed to address security and delivery challenges in the food delivery process, offering an improved experience for users.

### Key Features
1. **OTP Verification for Delivery Personnel** : Delivery personnel can use a one-time password (OTP) for secure access.
2. **LCD Display for Delivery Personnel** : An LCD screen provides delivery personnel with clear instructions and feedback.
3. **Group Access Management** : Users can create and manage groups, allowing multiple people to control the same box.
4. **Secure Lock Control** : Electronic lock supports control via the web interface.
5. **User-Friendly Operation** : Operated through a web-based interface.


## 🛠 Technical Details

### Hardware
- **Electronic Lock** : [Specifications and Purchase Link]([https://example.com/electronic-lock](https://www.icshop.com.tw/products/368011000480))
  - Voltage : 12V / 24V
  - Current : 0.8A / 1.2A
  - Power Consumption : 9.6W / 28.8W
  - Bolt Stroke Length : 10mm
  - Power-On Action Time : ≤ 1S
  - Continuous Power-On Time : ≤ 10S
- **Raspberry Pi** : Central control unit
- **LCD Screen** : Used to display OTP-related instructions and feedback for delivery personnel

### Software
- **Development Frameworks**:
  - Flask: Web interface and API
  - Firebase/SQLite: Data storage
- **Platform**:
  - Web Interface

### Workflow
1. Delivery personnel uses OTP to unlock the box and place the package.
2. Instructions and status are displayed on the LCD screen.
3. Users can manage access and lock the box remotely.
4. Group members can access the box if permissions are granted.



## 🚀 Installation and Usage

### Hardware Setup
1. Ensure Raspberry Pi is connected to the electronic lock and LCD screen.
2. Check for stable network connectivity.

### Software Installation
#### For Raspberry Pi
1. Clone the Raspberry Pi repository:
   ```bash
   git clone https://github.com/yourusername/SmartDeliveryBox-Pi.git
   ```
2. Install dependencies:
   ```bash
   cd SmartDeliveryBox-Pi
   pip install -r requirements.txt
   ```
3. Run the program:
   ```bash
   python pi_app.py
   ```

#### For Web Server (Computer)
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/SmartDeliveryBox.git
   ```
2. Install dependencies:
   ```bash
   cd SmartDeliveryBox
   pip install -r requirements.txt
   ```
3. Start the server:
   ```bash
   python app.py
   ```
4. Open `http://<Computer_IP>:5000` in a browser to access the interface.



## 📄 File Structure

```plaintext
SmartDeliveryBox/
├── app.py            # Main application entry point
├── requirements.txt  # Dependency requirements
├── templates/        # HTML files
├── static/           # Static resources (CSS, JS, Images)
└── README.md         # Documentation

SmartDeliveryBox-Pi/
├── pi_app.py         # Raspberry Pi application entry point
├── requirements.txt  # Dependency requirements
└── README.md         # Documentation
```

---

## 🛡 Security and Privacy
- All data transmission is encrypted to ensure user privacy.

---

## 🤝 Contributing
We welcome contributions from everyone:
1. Fork the repository.
2. Submit a Pull Request.
3. Provide feedback or report issues via [Issues](https://github.com/yourusername/SmartDeliveryBox/issues).

---

## 📧 Contact
For any questions or suggestions, please contact:
- Author: Zhe-Wei Kang
- Email: example@example.com

---

## 📜 License
This project is licensed under the [MIT License](https://opensource.org/licenses/MIT).
