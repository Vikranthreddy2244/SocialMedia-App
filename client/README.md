# Frontend - SocioMedia

This is the frontend of the SocioMedia application, built with React and Material-UI.

## Features
- User authentication (login/register)
- Responsive design with Material-UI
- User profile page
- Post feed with like and comment functionality
- Friend list management
- Dark and light mode toggle

## Tech Stack
- React.js
- Redux Toolkit (state management)
- Material-UI (UI components)
- React Router (routing)
- Formik & Yup (form validation)

## Setup Instructions

### Prerequisites
- Node.js installed
- Backend server running

### Installation
1. Navigate to the `client` directory:
   ```bash
   cd client
   ```
2. Install dependencies:
   ```bash
   npm install
   ```
3. Start the development server:
   ```bash
   npm start
   ```
4. The app will run on `http://localhost:3000`.

### Environment Variables
Create a `.env` file in the `client` directory with the following variable:
```
REACT_APP_API_URL=http://localhost:8080
```

## Usage
1. Ensure the backend server is running.
2. Start the frontend development server using:
   ```bash
   npm start
   ```
3. Open your browser and navigate to `http://localhost:3000`.

## File Structure
- `src/components/` - Reusable components
- `src/scenes/` - Pages and widgets
- `src/state/` - Redux state management
- `src/theme.js` - Theme settings for Material-UI

## Available Scripts
- `npm start` - Start the development server
- `npm run build` - Build the app for production
- `npm test` - Run tests

## Contributing
Contributions are welcome! Please follow these steps:
1. Fork the repository.
2. Create a new branch:
   ```bash
   git checkout -b feature-name
   ```
3. Commit your changes:
   ```bash
   git commit -m "Add feature-name"
   ```
4. Push to the branch:
   ```bash
   git push origin feature-name
   ```
5. Open a pull request.