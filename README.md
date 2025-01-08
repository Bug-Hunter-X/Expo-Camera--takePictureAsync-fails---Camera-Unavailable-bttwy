# Expo Camera: takePictureAsync Failure - Asynchronous Initialization

This repository demonstrates a common error when using the Expo Camera API:  `takePictureAsync` failing because the camera hasn't fully initialized.  The solution showcases the correct asynchronous approach to handle the camera's readiness.

## Problem:

Attempting to use `takePictureAsync` before the camera is ready leads to errors indicating the camera is undefined or unavailable.

## Solution:

Ensure `takePictureAsync` is called only *after* the camera has successfully initialized using the `onCameraReady` callback.  This ensures asynchronous handling of the camera initialization process.

## Setup:

1. Clone the repository.
2. Run `npm install` to install dependencies.
3. Run `expo start` to start the development server.