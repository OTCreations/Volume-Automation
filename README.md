# Volume-Automation
Automate your volume with Fingers Gestures
This application allows you to control the system's volume through hand gestures detected using your webcam. By moving your fingers and touching certain areas, you can increase or decrease the volume. The app uses hand tracking with MediaPipe, and the volume control works across all major platforms (Windows, macOS, Linux).

## Features
- **Volume Control**: Increase or decrease the volume by gestures.
- **Hand Gesture Detection**: Uses thumb-index and thumb-middle finger touch gestures.
- **Cross-Platform Support**: Works on Windows, macOS, and Linux.
- **Exit Gesture**: Closes the application when a fist (closed hand) is detected.
- **Volume Display**: Displays the current volume level in percentage.

## Requirements
- Python 3.x
- OpenCV
- MediaPipe
- Platform-specific tools for volume control:
  - **Windows**: `nircmd`
  - **macOS**: `osascript`
  - **Linux**: `amixer`

## Installation
1. Install the required packages using pip:
   ```bash
   pip install opencv-python mediapipe
   ```
2. For platform-specific tools:
   - **Windows**: Download and install `nircmd` from [NirCmd](https://www.nirsoft.net/utils/nircmd.html).
   - **macOS**: No additional installation needed for volume control (`osascript` is built-in).
   - **Linux**: Ensure `amixer` is installed (usually available by default).

## Usage
1. Run the script:
   ```bash
   python volumeUpDown.py
   ```
2. Allow the webcam to start, and position your hand in front of the camera.
3. Use the following gestures:
   - **Increase Volume**: Touch the **thumb** and **index finger** twice.
   - **Decrease Volume**: Touch the **thumb** and **middle finger** twice.
   - **Exit**: Make a **closed fist** (hand closed).
4. The volume will be displayed on the screen as a percentage.
5. The app will close when the hand is fully closed.

## Controls
- Press `q` to exit the app manually if needed.

## Troubleshooting
- Ensure your webcam is working properly.
- Verify that the platform-specific tools (e.g., `nircmd` on Windows) are correctly installed.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
