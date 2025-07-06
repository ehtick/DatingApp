# 🎉 DatingApp: A Full Stack Dating Application

![GitHub release](https://img.shields.io/github/release/Elie5464DE/DatingApp.svg?style=flat-square)

Welcome to the **DatingApp** repository! This is a full stack application built using **ASP.NET Core** and **Angular**. Our goal is to create a user-friendly platform for individuals seeking to connect and form meaningful relationships.

## Table of Contents

- [Features](#features)
- [Technologies Used](#technologies-used)
- [Installation](#installation)
- [Usage](#usage)
- [API Documentation](#api-documentation)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)

## Features

- User registration and authentication
- Profile creation and management
- Advanced search filters to find potential matches
- Real-time chat functionality
- User-friendly interface with responsive design
- Secure API endpoints

## Technologies Used

This project employs a range of technologies to provide a seamless experience:

- **Frontend**: Angular, HTML, CSS, JavaScript
- **Backend**: ASP.NET Core, C#
- **Database**: SQL Server, Entity Framework Core
- **APIs**: RESTful services for data handling

## Installation

To set up the DatingApp on your local machine, follow these steps:

1. **Clone the repository**:
   ```bash
   git clone https://github.com/Elie5464DE/DatingApp.git
   cd DatingApp
   ```

2. **Install dependencies**:
   - For the frontend, navigate to the `ClientApp` directory and run:
     ```bash
     npm install
     ```
   - For the backend, ensure you have the necessary packages in the `DatingApp` directory:
     ```bash
     dotnet restore
     ```

3. **Set up the database**:
   - Create a new SQL Server database.
   - Update the connection string in `appsettings.json` to point to your database.

4. **Run the application**:
   - Start the backend server:
     ```bash
     dotnet run
     ```
   - In a separate terminal, navigate to the `ClientApp` directory and run:
     ```bash
     ng serve
     ```

5. **Access the application**:
   Open your web browser and navigate to `http://localhost:4200`.

For the latest releases, visit our [Releases page](https://github.com/Elie5464DE/DatingApp/releases) to download and execute the necessary files.

## Usage

Once the application is running, you can:

- **Register**: Create a new account by filling out the registration form.
- **Log In**: Access your account using your credentials.
- **Create a Profile**: Add personal details and interests to your profile.
- **Search for Matches**: Use the search filters to find users that match your preferences.
- **Chat**: Send and receive messages in real-time with potential matches.

## API Documentation

The DatingApp API follows RESTful principles. Below are some key endpoints:

### User Endpoints

- **POST /api/users/register**: Register a new user.
- **POST /api/users/login**: Log in an existing user.
- **GET /api/users/{id}**: Retrieve user profile by ID.

### Matchmaking Endpoints

- **GET /api/matches**: Get a list of potential matches based on user preferences.
- **POST /api/matches/send**: Send a match request to another user.

### Chat Endpoints

- **GET /api/chat/{userId}**: Retrieve chat history with a specific user.
- **POST /api/chat/send**: Send a message to another user.

For detailed API documentation, please refer to the API section in the project or consult the code comments.

## Contributing

We welcome contributions to improve DatingApp. To contribute:

1. Fork the repository.
2. Create a new branch for your feature or bug fix.
3. Make your changes and commit them.
4. Push your branch and create a pull request.

Please ensure that your code adheres to the existing coding standards and includes appropriate tests.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Contact

For questions or suggestions, feel free to reach out:

- **Email**: [your-email@example.com](mailto:your-email@example.com)
- **GitHub**: [Elie5464DE](https://github.com/Elie5464DE)

Thank you for checking out the DatingApp! We hope you enjoy using it and find it useful in your journey to connect with others. For the latest updates and releases, please visit our [Releases page](https://github.com/Elie5464DE/DatingApp/releases).