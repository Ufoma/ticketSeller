# TicketSeller

## Table of Contents
- [Overview](#overview)
- [Features](#features)
- [Installation](#installation)
  - [Prerequisites](#prerequisites)
  - [Steps](#steps)
- [Usage](#usage)
  - [API Endpoints](#api-endpoints)
- [Contributing](#contributing)
  - [Guidelines](#guidelines)
- [Issues](#issues)
- [License](#license)
- [Hacktoberfest](#hacktoberfest)
- [Special Thanks](#special-thanks)

---

## Overview

**TicketSeller** is a web application designed to simplify event ticketing and management. It enables users to:

- Search events by date and time
- Follow or unfollow events
- View the number of event followers
- Use intuitive API endpoints

---

## Features

- **Event Search**: Look up events by date and time.
- **Follow and Unfollow Events**: Users can follow or unfollow specific events.
- **Followers Count**: Easily view how many followers each event has.
- **User-friendly API**: Simple endpoints for easy integration.

---

## Installation

### Prerequisites

Ensure you have the following installed:

- **Python 3.8+**
- **Flask 2.0+**
- **Flask-SQLAlchemy 2.5+**

### Steps

1. **Clone the repository**:  
   ```bash
   git clone https://github.com/your-username/TicketVerse.git
   ```

2. **Install dependencies**:  
   ```bash
   pip install -r requirements.txt
   ```

3. **Set up the database**:  
   The application uses SQLite. To configure the database, use the provided connection string:
   ```bash
   sqlite:///ticketverse.db
   ```

4. **Run the application**:  
   Start the Flask development server:
   ```bash
   flask run
   ```

---

## Usage

### API Endpoints

Below are the key API endpoints for interacting with TicketVerse:

#### 1. **Search Events**

- **URL**: `/search_events`
- **Method**: `GET`
- **Parameters**:
  - `date`: Event date (required)
  - `time`: Event time (required)
- **Response**: A JSON array containing event details.

#### 2. **Follow Event**

- **URL**: `/follow_event/<event_id>`
- **Method**: `POST`
- **Parameters**:
  - `user_id`: The ID of the user following the event.
- **Response**: A JSON object indicating success or failure.

#### 3. **Unfollow Event**

- **URL**: `/unfollow_event/<event_id>`
- **Method**: `POST`
- **Parameters**:
  - `user_id`: The ID of the user unfollowing the event.
- **Response**: A JSON object confirming success or failure.

#### 4. **Get Event Followers**

- **URL**: `/get_event_followers/<event_id>`
- **Method**: `GET`
- **Response**: A JSON array listing the followers of the event.

---

## Contributing

Contributions are always welcome! If you'd like to contribute to TicketVerse, follow these steps:

### Guidelines

1. **Fork the repository** to your GitHub account.
2. **Create a new branch** for your feature or bug fix:  
   ```bash
   git checkout -b your-branch-name
   ```
3. **Make your changes** and commit them:  
   ```bash
   git commit -m "Describe your changes here"
   ```
4. **Push your changes** to your GitHub repository:  
   ```bash
   git push origin your-branch-name
   ```
5. **Submit a pull request** and describe the changes you made.

---

## Issues

Have questions or found a bug? Please feel free to [open an issue](https://github.com/Ufoma/TicketVerse/issues). We're happy to help!

---

## License

This project is licensed under the terms of the [MIT License](LICENSE).

---

## Hacktoberfest

🎉 **TicketSeller is participating in Hacktoberfest!** 🎉  
Contribute to our project and earn rewards by submitting your pull requests during the Hacktoberfest event!

---

## Special Thanks

We would like to extend a special thanks to the SCA community  and all contributors for helping improve ticketSeller. 🙌

---

Happy contributing!




