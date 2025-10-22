# Face Emotion Finder

A simple web application that detects facial emotions in real-time using a webcam.

## Description

This project leverages the `face-api.js` library to detect faces in a video stream from your webcam and predict the emotions displayed on those faces. It provides a live visual representation of the detected faces and their corresponding emotion predictions directly in your browser.

## Features

*   **Real-time Emotion Detection:** Analyzes video stream from your webcam to detect and display emotions in real-time.
*   **Face Detection:** Identifies faces within the video stream.
*   **Emotion Prediction:** Predicts emotions such as happy, sad, angry, surprised, neutral, etc., based on facial expressions.
*   **Visual Overlay:** Draws a bounding box around detected faces and displays the predicted emotion on the video feed using a canvas overlay.
*   **Minimal Dependencies:**  Uses `face-api.js` via CDN for easy setup.

## Requirements

*   Web browser with webcam support.
*   Internet connection (for loading `face-api.js` from CDN).
*   Modern JavaScript enabled.

## Installation

No installation is required. This project is designed to run directly in a web browser.

## Usage

1.  Open the `emotion/emotion.html` file in your web browser.
2.  The browser will prompt you to grant access to your webcam.  Allow access for the application to function.
3.  The video feed from your webcam will be displayed, and the application will begin detecting faces and predicting emotions.
4.  Detected faces will be highlighted with a bounding box, and the predicted emotion will be displayed near the face.

## File Structure

```
face-emotion-finder/
├── emotion/
│   └── emotion.html  # Main HTML file containing the application
└── README.md       # This file
```

## Testing

This project relies on visual inspection for testing.  Ensure that:

*   The webcam feed is displayed correctly in the browser.
*   Faces are detected accurately.
*   Emotion predictions are reasonably accurate for various facial expressions.
*   The overlay is drawn correctly, displaying the bounding box and emotion labels.
*   The "Loading models..." status message disappears after the models are loaded.

## Configuration

There is no configuration file. The `face-api.js` models are loaded directly within the HTML file using CDN.  Advanced users may wish to download the models and serve them locally, which would require modifying the JavaScript code within `emotion/emotion.html`.

## Contributing

Contributions are welcome!  If you would like to contribute to this project, please follow these steps:

1.  Fork the repository.
2.  Create a new branch for your feature or bug fix.
3.  Implement your changes.
4.  Test your changes thoroughly.
5.  Submit a pull request with a clear description of your changes.

## License

This project is open-source and available under the [MIT License](LICENSE).  (Replace with the appropriate license file).

## Improvements

Potential improvements for this project include:

*   **Local Model Loading:**  Download and serve the `face-api.js` models locally to eliminate the CDN dependency.
*   **Improved Accuracy:**  Experiment with different `face-api.js` model configurations to improve emotion prediction accuracy.
*   **User Interface Enhancements:** Add a user interface to allow users to start/stop the emotion detection, adjust parameters, and view statistics.
*   **Mobile Support:** Optimize the application for mobile devices.
*   **More Emotions:** Add support for detecting a wider range of emotions.
*   **Performance Optimization:** Improve the performance of the application to handle higher frame rates and multiple faces.
*   **Error Handling:** Implement more robust error handling to gracefully handle webcam access issues or model loading failures.
* Add a LICENSE file.
