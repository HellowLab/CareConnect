
# CareConnect

**CareConnect** is a compact, wearable emergency alert device designed to keep you connected to help, without the need for costly subscriptions or complex third-party services. It's a sleek, user-friendly solution that empowers individuals to maintain their independence while ensuring their loved ones can provide timely assistance when needed.

## Key Features

- **No Subscription Fees**: Unlike traditional systems like LifeAlert, CareConnect requires no monthly fees or subscription services. It connects directly via Wi-Fi to notify caregivers through a mobile or web app.
- **Compact Design**: About the size of a half-dollar, CareConnect is comfortable to wear around the neck, with a prominent, easy-to-press button similar in size to a quarter.
- **Instant Alerts**: A simple press of the button sends an alert over Wi-Fi to the CareConnect app, allowing designated caregivers to receive real-time notifications.
- **Cost-Effective**: By utilizing Wi-Fi connectivity, CareConnect eliminates the need for expensive cellular networks or SIM cards, making it a one-time investment without recurring costs.
- **Rechargeable and Efficient**: Powered by a small, rechargeable battery and the Adafruit QT Py ESP32-S3 WiFi Dev Board, CareConnect is built to last with efficient power management and easy recharging via USB-C.
- **Customizable and Open-Source**: This repository contains all the source code and schematics needed to build, modify, and improve CareConnect for your own needs.

## Benefits Over Traditional Systems

- **No Recurring Costs**: Unlike systems like LifeAlert, which charge monthly fees, CareConnect provides a subscription-free experience.
- **Full Control**: CareConnect is open-source, giving users the freedom to modify and customize the device and software to fit their specific needs.
- **Simplified Connectivity**: By using existing Wi-Fi networks, it bypasses the need for cellular connectivity, reducing complexity and potential outages.

## Components

To build CareConnect, you'll need the following components:
- **Adafruit QT Py ESP32-S3 WiFi Dev Board** - [Link](https://www.adafruit.com/product/5540)
- **Adafruit Ultra Slim Lithium Polymer Battery - 150mAh** or equivalent - [Link](https://www.adafruit.com/product/1317)
- **Adafruit Massive Arcade Button (28mm)** or equivalent - [Link](https://www.adafruit.com/product/1185)
- **3D Printed Enclosure** - Design files will eventually be available in this repo.

## How It Works

1. **Button Press**: When the button is pressed, the ESP32-S3 microcontroller wakes up and connects to a pre-configured Wi-Fi network.
2. **Alert Sent**: The device sends a notification to the CareConnect app (via MQTT or HTTP) notifying caregivers of the event.
3. **Real-Time Notification**: The caregiver's device receives the alert, allowing them to take appropriate action.

## Installation

1. Clone this repository.
   ```bash
   git clone https://github.com/yourusername/careconnect.git
   ```
2. Set up your development environment with the **Arduino IDE** or **PlatformIO**.
3. Install necessary libraries (Wi-Fi, MQTT, etc.) as listed in `libraries.txt`.
4. Upload the firmware to the Adafruit QT Py ESP32-S3 WiFi Dev Board.
5. Customize the Wi-Fi credentials and notification endpoints (e.g., MQTT broker or webhook URL) in the firmware.

## Usage

- **Wearable Design**: Once built, the device can be worn around the neck and charged using a standard USB-C cable.
- **Recharging**: The rechargeable battery can last several days on a single charge with deep sleep modes enabled, ensuring the device is always ready for emergencies.

## Future Enhancements

- **GPS Integration**: Add location tracking for even more detailed alerts.
- **Fall Detection**: Incorporate motion sensors to automatically detect falls and trigger alerts.
- **Mobile App Development**: Enhance the companion app to include more features, such as location services, health monitoring, or voice alerts.

## License

This project is open-source and licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.

---

**CareConnect** – A smarter, more affordable approach to staying safe, with help just a button press away.
