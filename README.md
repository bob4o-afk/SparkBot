# SparkBot

![SparkBot](https://github.com/bob4o-afk/SparkBot/assets/80552018/f0fc268a-ceae-4656-84d2-f658327644ae)

SparkBot is a robot inspired by the beloved character Wall-E. It is equipped with a camera and utilizes Python and OpenCV to detect trash in its surroundings. Once trash is detected, SparkBot employs its robotic hand to pick it up and deposit it into its trash bin. Additionally, SparkBot has the ability to identify holes in the road, enhancing its utility in various scenarios.

## Features

- Trash Detection: SparkBot utilizes a camera and OpenCV to identify and locate trash within its field of vision.
- Robotic Hand: SparkBot's robotic hand enables it to pick up trash and deposit it into its designated trash bin.
- Hole Detection: SparkBot can identify holes in the road, making it an ideal companion for tasks involving navigation and safety.

## Setup

To set up SparkBot, follow these steps:

1. Connect the required components, including the camera and robotic hand, according to the provided pin configuration.
2. Ensure that the ESP32 board used has sufficient PSRAM for optimal performance.
3. Update the Wi-Fi credentials in the code by modifying the `ssid` and `password` variables to match your network.
4. Upload the code to SparkBot's ESP32 board using the Arduino IDE or another compatible method.
5. Open the Serial Monitor to view the output and monitor SparkBot's status.

## Usage

Once SparkBot is powered on and connected to Wi-Fi, it will start the camera and begin scanning its environment for trash and holes. The main loop in the code calls the `distance_calc()` function repeatedly to calculate the distance to nearby objects using an ultrasonic sensor.

To interact with SparkBot, you can access the camera feed and receive trash detection updates by visiting the IP address displayed in the Serial Monitor. This will allow you to monitor SparkBot's activities remotely and observe its detections in real-time.

## Dependencies

SparkBot relies on the following dependencies:

- [esp32-camera](https://github.com/espressif/esp32-camera): ESP32 library for camera support.
- [WiFi](https://github.com/arduino-libraries/WiFi): Arduino library for Wi-Fi connectivity.
- [OpenCV](https://opencv.org/): Open-source computer vision library for Python.

## Future Enhancements

The development of SparkBot is an ongoing process. Here are some potential future enhancements:

- Intelligent Trash Sorting: Implement advanced algorithms to enable SparkBot to classify different types of trash for more efficient disposal.
- Autonomous Navigation: Integrate additional sensors and algorithms to enable SparkBot to navigate autonomously and avoid obstacles.
- Cloud Integration: Connect SparkBot to a cloud platform for data storage, analysis, and remote control capabilities.
- Voice Interaction: Incorporate speech recognition and synthesis to enable SparkBot to respond to voice commands and communicate with users.

## Contributions

Contributions to SparkBot are welcome! If you have any ideas, bug fixes, or improvements, feel free to submit a pull request or open an issue on the [GitHub repository](https://github.com/bob4o-afk/SparkBot).
