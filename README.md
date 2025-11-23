
# 📘 PhonoLearn – Offline Phonological Awareness Platform


PhonoLearn is an offline, local-hosted, and child-friendly educational application designed to strengthen phonological awareness and foundational literacy skills in preschool and early-school children. It runs through a self-contained executable that launches a local Go HTTP server, and the user interacts with the platform through Microsoft Edge at:

http://localhost:8080

All data (sessions, answers, progression) is stored locally on the machine using JSON files — ensuring complete privacy, no network dependency, and a simple installation experience.
## Table of Contents

Description
## 📘 Description

PhonoLearn is a self-contained, offline intervention platform built to help children develop:

phonological awareness

The system delivers interactive exercises, manages progression automatically, and stores every answer and session locally.

The executable launches a local Go server and instructs the user to open http://localhost:8080 in Microsoft Edge to begin using the application.

✔ No installation
✔ No internet required
✔ Highly privacy-safe
✔ Designed for children, educators, and therapists


## 🖼 Logo

![alt text](app_shortcut.ico)



## ⭐ Features

### 🎒 Educational

- Progressive difficulty (advances when score ≥ 80%)

- Structured JSON-based exercise bank

- Wrong-answer reuse for mastery learning

- Automatic session summaries

- Multiple exercise templates

### 🛠 Technical

- Go-based local HTTP server

- HTML/JS user interface

- No internet access

- Real-time JSON answer storage

- Folder structure auto-generated per child/session

### 👶 Child-Friendly UI

- Large icons and simple interactions

- Audio playback support

- Consistent templates


## 🧠 Tech Stack

- **Golang** (server, logic, scoring, persistence)

- **HTML / CSS / JavaScript** (interface)

- **JSON** (exercise + answer storage)


## 🏗 Architecture

PhonoLearn uses a **Layered Architecture** combined with **MVC + Repository + Services**.

    1. Presentation Layer
        HTML pages (main.html, ...)
        JavaScript logic (main.js, ...)
        Audio, images, templates

    2. Application Layer
        Go handlers
        HTTP routing
        Session management
        Template rendering

    3. Domain Layer
        Scoring rules
        Difficulty progression engine
        Wrong-answer prioritization
    
    4. Infrastructure Layer
        Local JSON files
        Folder auto-creation
        Real-time answer persistence









## 📦 Installation

End-users do not install anything — they simply:

    1. 
    Receive the project folder (provided by the developer).

    2. 
    Double-click: intervention-app.exe
    A command window opens and displays: Open in Microsoft Edge http://localhost:8080

    3. 
    User copies/pastes the link into Microsoft Edge.
    
    4. 
    The app runs fully locally.


## 🧩 Usage / Examples

- User starts a session

- App loads exercises dynamically

- Answers saved in real time

- Scoring determines next level

- Session completed and marked


## 🔧 Configuration & Environment

Configuration is stored in:Configuration is stored in:
data/config.json

Variables include:

- patientId

- users
## 🗄 Data Storage

/individual/{patientId}/sessionX/answers/*.json

sessionX_done.txt

SectorLevel.json
## Documentation

[Documentation](https://github.com/argyri-kyr/PhonoLearn/blob/dea6dc773894bbc52701c28b964fdd6b807ae8b8/Documentation.docx)


## ❓ FAQ

#### Do I need internet?

No. Localhost does not require internet.

#### Why Edge?

Guaranteed compatibility with HTML/CSS/JS features used.

#### What ages can play the app?
The app is for ages 7-8 and up. Children in 2nd - 3rd grade could play the game, perhaps with some guidance by their side.

#### Can I see my answers?
Yes, you can see them at any time, as they are stored locally.




## Support

For support, email kyriakaki.argyri@gmail.com .


## 👥 Authors

- [@argyri-kyr](https://github.com/argyri-kyr)



## 🧑‍🏫 Used By

This project can be used by the following:

- Children
- Educators
- Therapists

