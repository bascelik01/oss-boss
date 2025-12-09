OSS BOSS – Martial Arts Technique Tracker

A full-stack React + Django application for tracking techniques in grappling, MMA, and Brazilian Jiu-Jitsu. OSS BOSS helps martial artists log techniques, organize them, take notes, and monitor their improvement journey.

🚀 Features

Full CRUD functionality for techniques


Notes, variations, and difficulty levels

User authentication

REST API built with Django REST Framework

Responsive, modern React dashboard

# Database Schema

| Field        | Type         | Description                        |
| ------------ | ------------ | ---------------------------------- |
| id           | Integer (PK) | Unique ID                          |
| user         | ForeignKey   | Owner of technique                 |
| title        | CharField    | Technique name                     |
| category     | CharField    | Sweep / Submission / Escape / etc. |
| difficulty   | Integer      | 1–5 scale                          |
| description  | TextField    | Full explanation                   |
| notes        | TextField    | Optional notes                     |
| video_url    | URLField     | Optional YouTube link              |
| progress     | CharField    | learning/drilling/mastered         |
| date_learned | DateField    | When learned                       |
| created_at   | DateTime     | Auto                               |
| updated_at   | DateTime     | Auto                               |

# Technique Endpoints
| Method | Endpoint            | Description                         |
| ------ | ------------------- | ----------------------------------- |
| GET    | `/techniques/`      | List all techniques (user-specific) |
| POST   | `/techniques/`      | Create technique                    |
| GET    | `/techniques/<id>/` | Retrieve technique                  |
| PUT    | `/techniques/<id>/` | Update technique                    |
| PATCH  | `/techniques/<id>/` | Partial update                      |
| DELETE | `/techniques/<id>/` | Delete technique                    |

