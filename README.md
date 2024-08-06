# Job Finder

Welcome to the Job finder, a matchmaking API repository for Developers and Companies! This API aims to connect developers and companies, facilitating the meeting of qualified professionals and job openings through a matchmaking system.

## Table of Contents

- [Description](#description)
- [Technologies Used](#technologies-used)
- [Installation](#installation)
- [Usage](#usage)
- [API Endpoints](#api-endpoints)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)

## Description

This API is designed to provide a matchmaking platform between developers and companies. Users can create detailed profiles, list and apply for job openings, and communicate after a "match." The system uses a Domain-Driven Design (DDD) architecture and offers features such as JWT authentication, data validation, and reporting.

## Technologies Used

- **Language**: C# with .NET 8
- **Database**: MySQL with Entity Framework Core
- **Authentication**: JWT (JSON Web Tokens)
- **Validation**: FluentValidation
- **Documentation**: Swagger
- **Testing**: xUnit, Moq

## Installation

### Prerequisites

- .NET 8 SDK
- MySQL
- Visual Studio or any code editor compatible with C#

### Steps

1. Clone the repository:

   ```bash
   git clone https://github.com/MatthewAraujo/job_finder.git
   cd job_finder
   ```

2. Configure the database:

   - Create a MySQL database.
   - Update the connection settings in `appsettings.json`.

3. Run the migrations to create the database tables:

   ```bash
   dotnet ef database update
   ```

4. Build and run the project:

   ```bash
   dotnet run
   ```

## Usage

After starting the application, you can access the API documentation on Swagger at `http://localhost:7831/swagger`. From there, you can test the endpoints and better understand the API's functionality.

## API Endpoints

### Authentication

- `POST /api/auth/register`: User registration.
- `POST /api/auth/login`: User login and JWT token generation.

### Developers

- `GET /api/developers`: List all developers.
- `GET /api/developers/{id}`: Get details of a specific developer.
- `PUT /api/developers/{id}`: Update developer information.
- `DELETE /api/developers/{id}`: Delete a developer.

### Companies

- `GET /api/companies`: List all companies.
- `GET /api/companies/{id}`: Get details of a specific company.
- `PUT /api/companies/{id}`: Update company information.
- `DELETE /api/companies/{id}`: Delete a company.

### Job Offers

- `GET /api/joboffers`: List all job offers.
- `GET /api/joboffers/{id}`: Get details of a specific job offer.
- `POST /api/joboffers`: Create a new job offer.
- `PUT /api/joboffers/{id}`: Update a job offer.
- `DELETE /api/joboffers/{id}`: Delete a job offer.

### Matchmaking

- `POST /api/match`: Create a match between a developer and a company.
- `GET /api/matches`: List all matches.

## Contributing

Contributions are welcome! Feel free to open issues or pull requests. For larger contributions, it's recommended to open an issue for discussion before submitting changes.

## Contact

For more information or questions, contact us at [matthewaraujo20@gmail.com](mailto:matthewaraujo20@gmail.com).
