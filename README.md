# Dundee Data Meetup Website

Official website for Dundee Data Meetup

🌐 **Live Site:** [https://ddm.scot](https://ddm.scot)

## About

Dundee Data Meetup is dedicated to fostering an inclusive community where individuals from diverse backgrounds can come together to share knowledge, spark ideas, ignite curiosity, foster collaboration, and promote responsible data practices. Each month features different themes and speakers from the local data community.

## Tech Stack

This website is built with:
- **Jekyll 4.3.3** - Static site generator
- **Bootstrap 5** - CSS framework
- **GitHub Pages** - Hosting platform

## Project Structure

```
├── _config.yml              # Jekyll configuration
├── _events/                 # Event markdown files organized by year
│   ├── 2023/
│   ├── 2024/
│   └── 2025/
├── _layouts/                # Page templates
│   ├── default.html         # Base layout
│   └── event.html           # Event page layout
├── _organisers/             # Organiser profiles
├── _speakers/               # Speaker profiles
├── _sponsors/               # Sponsor information
├── assets/                  # Static assets
│   ├── css/                 # Stylesheets
│   ├── img/                 # Images
│   ├── js/                  # JavaScript files
│   └── slides/              # Event presentation slides
├── data/                    # Data files
│   └── attendance.csv       # Event attendance records
├── index.html               # Homepage
├── events.html              # Events listing page
├── speakers.html            # Speakers page
├── speak.html               # Call for speakers
├── about.html               # About page
└── code-of-conduct.html     # Code of conduct
```

## Getting Started

### Prerequisites

- Ruby (version 2.7 or higher)
- Bundler gem

### Installation

1. Clone the repository:
```bash
git clone https://github.com/DundeeDataMeetup/dundeedatameetup.github.io.git
cd dundeedatameetup.github.io
```

2. Install dependencies:
```bash
bundle install
```

3. Run the development server:
```bash
bundle exec jekyll serve
```

4. Open your browser and navigate to `http://localhost:4000`

## Adding Content

### Adding a New Event

1. Create a new markdown file in `_events/YYYY/MM.md` (e.g., `_events/2025/12.md`)
2. Use the following frontmatter template:

```yaml
---
title: "Event Title"
description: "Event description"
date: YYYY-MM-DD HH:MM:SS
topics:
    - speaker: speaker-slug # or ["speaker-slug1", "speaker-slug2"]
      title: "Talk Title"
      description: Talk description
attendance: XX
slides:
    - url: /assets/slides/filename.pdf
      title: Slide Title
---
```

### Adding a New Speaker

1. Create a new markdown file in `_speakers/speaker-name.md`
2. Add speaker information following existing examples

### Adding a New Organiser

1. Create a new markdown file in `_organisers/organiser-name.md`
2. Add organiser information following existing examples

## Contributing

We welcome contributions! Whether it's fixing typos, improving documentation, or adding new features, please feel free to:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request
