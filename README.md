# Chill Spots

Chill Spots is a web application where users can discover and share popular spots within various cities. Users can add new spots, categorize them, and associate specific vibes with these spots. Additionally, users can upvote or downvote spots, contributing to a community-driven ranking system.

## Features

- User Authentication (Sign Up, Login, Logout)
- Add and categorize spots by city
- Assign vibes (e.g., “Exciting”, “Relaxing”) to spots
- Upvote and downvote spots
- Google Maps integration for location handling
- Responsive design using Bootstrap

## Tech Stack

- **Ruby:** Main programming language
- **Sinatra:** Web framework
- **ActiveRecord:** ORM for database interactions
- **SQLite3:** Database for development and testing
- **Puma:** Web server
- **ERB (Embedded Ruby):** Templating language
- **JavaScript:** For interactive features and AJAX
- **Google Maps API:** For map functionalities
- **Bootstrap:** For styling and responsive design
- **bcrypt:** For secure password handling

## Installation and Setup

### Prerequisites

Ensure you have the following installed:

- **Ruby** (version 2.5.0 or higher recommended)
- **Bundler**
- **SQLite3**
- **Git** (to clone the repository)

### Clone the Repository

```bash
git clone https://github.com/yourusername/chill_spots.git
cd chill_spots
```

### Install Dependencies
```bash
bundle install
```

### Database Setup

Create the database, Run migrations and Populate the database with initial data:
```bash
bundle exec rake db:create
bundle exec rake db:migrate
bundle exec rake db:populate
```

## Running the Application

To run the app in development mode with automatic code reloading:
```bash
bundle exec shotgun
```
Visit http://localhost:9393 in your browser.

### Environment Variables

SESSION_KEY: Custom session secret key for security (optional, defaults to 'lighthouselabssecret').

### Troubleshooting

- JSON Gem Issue: If you encounter errors with the json gem during installation, ensure you are using a compatible Ruby version (2.5.x or higher). Consider updating the json gem version in the Gemfile if necessary.
- Database Connection Issues: Ensure your SQLite3 database is properly configured and running.

### Contributing

Feel free to submit issues or pull requests. For major changes, please open an issue first to discuss what you would like to change.

### License

This project is licensed under the MIT License. See the LICENSE file for details.