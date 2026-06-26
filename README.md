🔵 **Bluetooth Device Detection & Alert System (Python)**

This project is a Python-based Bluetooth Low Energy (BLE) scanner that continuously monitors nearby BLE devices and triggers an alert when a specific target device is detected.
It uses the bleak library for cross-platform BLE scanning and is suitable for security monitoring, asset tracking, and proximity-based alerts.

**🚀 Features**
📡 Scans nearby Bluetooth Low Energy (BLE) devices
🎯 Detects a specific target device by MAC address
🚨 Triggers an alert only once when the device is first detected
⏰ Logs the exact detection time
💻 Works on Windows, Linux, and macOS
⚡ Lightweight and easy to customize

**🛠️ Technologies Used**
Python 3.8+
asyncio – asynchronous scanning
bleak – BLE device scanning
datetime – timestamp logging

📂 **Project Structure**
bluetooth-device-detector/
│
├── app.py        # Main Python script
├── README.md         # Project documentation
└── requirements.txt  # Python dependencies


**📦 Installation**
1️⃣ Clone the Repository
git clone https://github.com/your-username/bluetooth-device-detector.git
cd bluetooth-device-detector

2️⃣ Create a Virtual Environment (Optional but Recommended)
python -m venv venv
source venv/bin/activate    # macOS/Linux
venv\Scripts\activate       # Windows

3️⃣ Install Dependencies
pip install bleak

Or using requirements.txt:

pip install -r requirements.txt
⚙️ Configuration

Open scanner.py and update the target device MAC address:

TARGET_DEVICE_ADDRESS = "A4:4B:D5:51:D0:8D"

💡 Tip: You can find BLE MAC addresses using Bluetooth scanner apps or tools like bluetoothctl (Linux) or system Bluetooth settings.

▶️ Usage

Run the scanner using:

python app.py

**Sample Output**
📡 Scanning for device...

ALERT!
Device detected: A4:4B:D5:51:D0:8D
Time: 18:42:15

🛑 Scan stopped

The scanner runs for 30 seconds by default and stops automatically.

**🧠 How It Works**
Starts an asynchronous BLE scan
Listens for advertisement packets
Compares detected device addresses with the target MAC
Triggers an alert when a match is found
Prevents duplicate alerts during the same scan session

**🔒 Use Cases**
🔐 Security & intrusion detection
📍 Proximity-based alerts
🧾 Asset tracking
🧪 BLE experimentation & learning
🏠 Smart home presence detection

**⚠️ Notes & Limitations**
Requires Bluetooth hardware support
BLE MAC addresses may change due to device privacy settings
On Windows, ensure Bluetooth is enabled and supported by the OS


**🔮 Future Enhancements**
🔔 Sound or email notifications
🗄️ Logging detection events to a file
🔁 Continuous scanning mode
📊 Dashboard or GUI interface
🌐 Webhook or API integration


**🤝 Contributing**

Contributions are welcome!
Feel free to fork this repository and submit a pull request.
