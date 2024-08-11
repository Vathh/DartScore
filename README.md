# Dart Tournament Management System
## Introduction
Darts is a popular competitive game where players throw small, sharp-tipped darts at a circular target (dartboard) to score points. It is often played in leagues or tournaments, 
where the organization and management of matches, players, and statistics can become complex and time-consuming.

This project is designed to automate and simplify the management of dart tournaments, particularly those using the 'double K.O.' (double elimination) system. 
In this format, players have two opportunities to stay in the tournament before they are completely eliminated, making it a fair and exciting competition style.

By using this system, tournament organizers can efficiently manage player registrations, create tournament brackets, track match results, and update 
player statistics—all while maintaining a comprehensive record of each season's standings and achievements. This not only saves time but also enhances the experience for both organizers and participants by providing clear, organized, and accessible data.

## Project Overview
This repository contains the complete solution for managing dart tournaments, including a backend API, a web application for organizers, and a mobile 
application for live scorekeeping during matches.

### Backend (API)
- Description: The backend is a Spring Boot application that provides RESTful APIs for managing tournaments, players, and statistics. 
It handles all data storage, business logic, and user authentication.
### Web Application
- Description: The web application is designed for tournament organizers. It allows them to manage seasons, tournaments, and players. 
The web app also displays historical data and statistics for each season and tournament.
### Mobile Application
- Description: The mobile app is used for live scorekeeping during matches. It allows referees or players to track scores, log achievements, and submit match results directly to the backend.
  
## Technologies Used
### Backend:
- Spring Boot
- Spring Data JPA
- Spring Security with JWT
- PostgreSQL
- Flyway
- Lombok
- MapStruct
  
### Web Application:
- React
- Redux
- React Router
- Material-UI
- Styled-Components
  
### Mobile Application:
- React Native
- Expo
- React Navigation
  
## Project Structure
The repository is organized into three main directories, each corresponding to one of the major components of the system:
- /dart_league: Contains the Spring Boot API for managing the tournament data.
- /front_sld: Contains the React web application for tournament organizers.
- /sld_mobile: Contains the React Native mobile application for scorekeeping.
  
## Getting Started

### Prerequisites
To run this project locally, you'll need to have the following installed on your machine:
- Docker
  
### Installation and Setup
- Clone this repository to your local machine.
- In the /sld_mobile/helpers/apiConfig.js file, replace the existing IP address with the IP address of your local machine.
- Open a terminal in the root directory of the project.
- Run the following command: docker compose up --build.
- Docker will build and start all necessary services, including the backend, web, and mobile applications, as well as the database.
  
## Usage
### Example Workflow
- Create a Season: The admin can use the web application to create a new season, including multiple tournaments.
- Register Players: The admin adds players to the database via the web application.
- Start a Tournament: The admin activates a tournament and selects the players participating. The matches are then generated based on the selected participants.
- Play Matches: Players or referees use the mobile app to track scores in real-time and log achievements during the match.
- Track Tournament Progress: During the tournament, users can view the progress of the tournament bracket, seeing who won each match in real-time. 
Detailed statistics of the tournament are available after its ending.
- View Season Statistics: Users can track player performance and results across the entire season using the web application.
  
## Future Development
- Additional Game Modes: Implement support for pair tournaments, group-stage tournaments, and non-seasonal tournaments.
- Enhanced Statistics: Expand the mobile app's statistical tracking to include more detailed in-game metrics.
- Customizable Match Settings: Allow the admin to configure the number of legs/sets required to win a match.

## License
This project is intended primarily for personal and portfolio use. It showcases a complete solution for managing dart tournaments. 
There is no specific license applied to this project, but the code can be referenced and utilized for personal or educational purposes. For any commercial use or distribution, 
please contact the author for permission.

## Contact
For any questions or inquiries, please contact me at przestrzelski.maciej1@gmail.com.
