# Data Dictionary for Music Streaming Database

## Table: users
| Column Name  | Data Type     | Description                                  |
|--------------|---------------|----------------------------------------------|
| user_id      | SERIAL PRIMARY KEY | Unique identifier for each user              |
| username     | VARCHAR(50)   | Display name of the user                     |
| email        | VARCHAR(100)  | User's email address (must be unique)       |
| signup_date  | DATE          | Date the user joined the platform           |

---

## Table: artists
| Column Name  | Data Type     | Description                               |
|--------------|---------------|-------------------------------------------|
| artist_id    | SERIAL PRIMARY KEY | Unique identifier for each artist          |
| name         | VARCHAR(100)  | Artist name                               |
| genre        | VARCHAR(50)   | Music genre (e.g., Afro-Pop, Afrobeat)   |

---

## Table: songs
| Column Name      | Data Type     | Description                             |
|------------------|---------------|-----------------------------------------|
| song_id          | SERIAL PRIMARY KEY | Unique identifier for each song         |
| title            | VARCHAR(150)  | Title of the song                        |
| artist_id        | INT REFERENCES artists(artist_id) | Links song to artist    |
| release_year     | INT           | Year the song was released               |
| duration_seconds | INT           | Duration of the song in seconds          |

---

## Table: user_favorites
| Column Name  | Data Type     | Description                             |
|--------------|---------------|-----------------------------------------|
| favorite_id  | SERIAL PRIMARY KEY | Unique identifier for each favorite     |
| user_id      | INT REFERENCES users(user_id) | Links favorite to a user      |
| song_id      | INT REFERENCES songs(song_id) | Links favorite to a song      |
| favorited_at | DATE          | Date when the song was favorited         |


