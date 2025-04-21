# Biometric Authentication App

An Angular 19 application implementing facial recognition for secure biometric authentication. This application demonstrates a complete authentication flow using facial biometrics, with a focus on performance and responsive design.

## Features

- **User Registration**: Create accounts with username, password, and facial biometric data
- **Biometric Login**: Authenticate using facial recognition technology
- **Responsive Design**: Works seamlessly on both desktop and mobile devices
- **Client-side Processing**: Processes facial data locally using face-api.js
- **Secure Storage**: Stores facial data as byte arrays for efficient comparison

## Tech Stack

- Angular 19
- TypeScript
- face-api.js for facial recognition
- Local Storage for data persistence (demo mode)
- RxJS for reactive programming

## Prerequisites

- Node.js (v18 or later)
- npm (v9 or later)
- Modern web browser with camera access

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/YOUR_USERNAME/biometric-auth-app.git
   cd biometric-auth-app
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Download face-api.js models:
   ```bash
   mkdir -p src/assets/face-api-models
   # Download the models from https://github.com/justadudewhohacks/face-api.js/tree/master/weights
   # and place them in the src/assets/face-api-models directory
   ```

4. Start the development server:
   ```bash
   ng serve
   ```

5. Navigate to `http://localhost:4200/` in your browser

## Usage

1. **Registration**:
   - Navigate to the registration page
   - Enter your username and password
   - Allow camera access when prompted
   - Position your face in the frame and capture your facial data
   - Complete registration

2. **Login**:
   - Navigate to the login page
   - Enter your username and password
   - Allow camera access when prompted
   - Position your face in the frame for verification
   - If the facial data matches, you'll be logged in

## Demo Mode

This application currently runs in demo mode, storing all data in the browser's local storage. This approach is for demonstration purposes only and wouldn't be suitable for a production environment.

## Security Considerations

- In a real-world implementation, biometric data should be securely stored on a server
- The application should use HTTPS for all communications
- Additional security measures like rate limiting and anomaly detection should be implemented
- Consider using WebAuthn for standards-compliant biometric authentication

## License

[MIT](LICENSE)

## Acknowledgments

- [face-api.js](https://github.com/justadudewhohacks/face-api.js) for the facial recognition functionality
