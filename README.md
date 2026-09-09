# polar-h10-data-reader
Web-based data extractor for Polar H10 heart rate sensors using Web Bluetooth API.

# Polar H10 BLE Data Extractor

A lightweight, static web application designed to extract and visualize real-time data from a Polar H10 heart rate sensor. The tool operates entirely on the client side using the Web Bluetooth API, requiring no backend infrastructure or local installation.

## Live Application

[Link](https://gonzaloesloga.github.io/polar-h10-data-reader/)

## System Requirements

Due to the reliance on the Web Bluetooth API, specific hardware and software criteria must be met:

*   **Hardware:** A Polar H10 chest strap and a device (computer or Android smartphone) with active Bluetooth functionality.
*   **Browser Compatibility:** Google Chrome, Microsoft Edge, or Opera. 
*   **Restrictions:** Apple iOS devices (including Chrome for iOS) and Mozilla Firefox do not currently support the Web Bluetooth API and cannot run this application.

## Usage Instructions

1. Moisten the electrode areas of the strap and wear the Polar H10 sensor around your chest to activate it. The sensor will not broadcast a Bluetooth signal unless it detects a heartbeat.
2. Navigate to the live application URL using a supported browser.
3. Click the connection button on the interface.
4. A browser-native prompt will appear displaying nearby Bluetooth devices. Select your Polar H10 sensor and click "Pair".
5. The application will immediately begin reading and displaying the broadcasted data.

## Architecture

This project is built using standard HTML5 and Vanilla JavaScript. All data processing, event handling, and Bluetooth communication are executed locally in the browser memory. No telemetry or data storage is implemented.

## License

This project is licensed under the MIT License.
