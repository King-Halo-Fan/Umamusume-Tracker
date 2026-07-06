<!-- Back to top anchor -->
<a id="readme-top"></a>

<!-- PROJECT SHIELDS -->
[![Contributors][contributors-shield]][contributors-url]
[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]
[![License][license-shield]][license-url]

<!-- PROJECT LOGO -->
<br />
<div align="center">

  <h3 align="center">🏇 Umamusume Tracker</h3>

  <p align="center">
    A fan-made progress tracker for <em>Umamusume Pretty Derby</em> (Global Server)
    <br />
    <a href="https://github.com/King-Halo-Fan/Umamusume-Tracker"><strong>Explore the docs »</strong></a>
    <br />
    <br />
    <a href="https://github.com/King-Halo-Fan/Umamusume-Tracker">View Project</a>
    &middot;
    <a href="https://github.com/King-Halo-Fan/Umamusume-Tracker/issues/new?labels=bug">Report Bug</a>
    &middot;
    <a href="https://github.com/King-Halo-Fan/Umamusume-Tracker/issues/new?labels=enhancement">Request Feature</a>
  </p>
</div>

---

<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
      <ul>
        <li><a href="#built-with">Built With</a></li>
      </ul>
    </li>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#prerequisites">Prerequisites</a></li>
        <li><a href="#installation">Installation</a></li>
      </ul>
    </li>
    <li><a href="#usage">Usage</a></li>
    <li><a href="#roadmap">Roadmap</a></li>
    <li><a href="#contributing">Contributing</a></li>
    <li><a href="#license">License</a></li>
    <li><a href="#contact">Contact</a></li>
    <li><a href="#acknowledgments">Acknowledgments</a></li>
    <li><a href="#ai-usage-disclaimer">AI Usage Disclaimer</a></li>
  </ol>
</details>

---

<!-- ABOUT THE PROJECT -->
## About The Project

Umamusume Tracker is a fan-made web app for tracking your progress in *Umamusume Pretty Derby* on the Global server. Built with no frameworks — just vanilla HTML, CSS, and JavaScript — it runs entirely in the browser with optional cloud save support via Supabase. This means it can run on both phone and pc!

Here's what makes it useful:
* Track which characters you own, their story events, epitapths, and race data all in one place
* Save your progress to the cloud using a simple PIN — no account needed. If youre using this without making your own repository, please be respectful of other peoples saves if a PIN has already been used.
* Support for costume alternates so your tracker reflects your preferred outfits

<p align="right">(<a href="#readme-top">back to top</a>)</p>

---

### Built With

* [![HTML5][HTML5-badge]][HTML5-url]
* [![CSS3][CSS3-badge]][CSS3-url]
* [![JavaScript][JS-badge]][JS-url]
* [![Supabase][Supabase-badge]][Supabase-url]
* [![Google Fonts][Fonts-badge]][Fonts-url]

<p align="right">(<a href="#readme-top">back to top</a>)</p>

---

<!-- GETTING STARTED -->
## Getting Started

No build steps required. Just clone the repo and open `index.html`.

### Prerequisites

* A modern web browser (Chrome recommended)
* A free [Supabase](https://supabase.com) account if you want cloud save support

### Installation

1. Clone the repo
   ```sh
   git clone https://github.com/King-Halo-Fan/Umamusume-Tracker.git
   ```
2. Open `index.html` in your browser — that's it!

3. *(Optional)* Set up Supabase for PIN-based save states:
   - Create a free project at [supabase.com](https://supabase.com)
   - Add your Supabase project URL and anon key to `index.html`
   - Create a save state table matching the app's schema

> **Tip:** If CSV changes don't appear after editing, close and reopen your browser to clear the cache.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

---

<!-- USAGE -->
## Usage

### Character Tracking
Each character is loaded from `characters.csv`. Cards display character colors and support costume alternates — click the **⟳** button on any card to cycle through available skins.

### Story Events
Story events are loaded from `story_events.csv`. Each event should be on its own row. Use `ALL` (uppercase) in the character column to mark events that apply to every character.

### Race Data
Race info is loaded from `races.csv` and includes surface type (Turf/Dirt), distance, grade, and when it takes place.

### Save States
Set your PIN from the website to sync your progress to Supabase. If saves stop working, check whether your Supabase free-tier project has paused due to inactivity.

### CSV Format — Quick Reference

**`characters.csv`**
| Column | Required | Description |
|---|---|---|
| `name` | ✅ | Character name |
| `color` | ✅ | Primary hex color |
| `text` | ✅ | Text color |
| `alt1_label` | ➖ | Costume alternate label |
| `alt1_color` | ➖ | Costume alternate color |
| `alt1_text` | ➖ | Costume alternate text color |

**`story_events.csv`**
| Column | Description |
|---|---|
| `character` | Character name, or `ALL` for universal events |
| `event` | Event name — one per row |

<p align="right">(<a href="#readme-top">back to top</a>)</p>

---

<!-- ROADMAP -->
## Roadmap

- [x] Character card system with color theming
- [ ] complete story event tracking per character
- [x] Universal (`ALL`) story events
- [x] PIN-based cloud save via Supabase
- [x] Costume alternate / skin swapping for all outfits


See the [open issues](https://github.com/King-Halo-Fan/Umamusume-Tracker/issues) for a full list of proposed features and known bugs.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

---

<!-- CONTRIBUTING -->
## Contributing

This is a personal fan project, but suggestions and feedback are welcome! If you spot a data error or have an idea for a feature:

1. Fork the project
2. Create your feature branch (`git checkout -b feature/YourFeature`)
3. Commit your changes (`git commit -m 'Add YourFeature'`)
4. Push to the branch (`git push origin feature/YourFeature`)
5. Open a Pull Request

Feel free to also just send me a message, or leave an issue of any feedback / ideas. 
Don't forget to give the project a ⭐ if you find it useful!

<p align="right">(<a href="#readme-top">back to top</a>)</p>

---

<!-- LICENSE -->
## License

Distributed under the MIT License. See `LICENSE.txt` for more information.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

---

<!-- CONTACT -->
## Contact

King-Halo-Fan — [@King-Halo-Fan](https://github.com/King-Halo-Fan)

Project Link: [https://github.com/King-Halo-Fan/Umamusume-Tracker](https://github.com/King-Halo-Fan/Umamusume-Tracker)

<p align="right">(<a href="#readme-top">back to top</a>)</p>

---

<!-- ACKNOWLEDGMENTS -->
## Acknowledgments

* [Umamusume Pretty Derby (Global)](https://umamusume.cy-us.games/) — the game this tracker is built for
* [Supabase](https://supabase.com) — free open-source backend for save state storage
* [Google Fonts](https://fonts.google.com) — Playfair Display & DM Sans
* [Img Shields](https://shields.io) — badge generation
* [othneildrew/Best-README-Template](https://github.com/othneildrew/Best-README-Template) — README structure inspiration
* [Cygames](https://www.cygames.co.jp/) — creators of Umamusume Pretty Derby

> **Fan Disclaimer:** This is an unofficial fan project and is not affiliated with, endorsed by, or sponsored by Cygames or DeNA. All character names, artwork references, and game content belong to their respective owners.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

---

<!-- AI USAGE DISCLAIMER -->
## AI Usage Disclaimer

This project was developed with assistance from **Claude (Anthropic)**, an AI assistant, during the design and development process. AI was used to help with:

* Writing and debugging JavaScript logic
* Generating and refining CSS styling
* Structuring CSV data formats
* Drafting documentation (including this README)

All code, data, and content have been reviewed and directed by the project owner. AI-generated suggestions were evaluated and modified as needed — the creative direction, decisions, and final output remain the work of the developer.

This disclaimer is included in the spirit of transparency. While I love Umamusume, and can be pretty particular about things I want to track, I just did not have the coding skills to make this the way I wanted to.
I hope yall can find use in this like I am (since I often get too annoyed with having to leave a career to reference the races I want / the events I need).
Please no hate, while I am ashamed of my AI usage I just really needed something to track this outside the app - and I thought others might find use too.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

---

<!-- MARKDOWN LINKS & IMAGES -->
[contributors-shield]: https://img.shields.io/github/contributors/King-Halo-Fan/Umamusume-Tracker.svg?style=for-the-badge
[contributors-url]: https://github.com/King-Halo-Fan/Umamusume-Tracker/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/King-Halo-Fan/Umamusume-Tracker.svg?style=for-the-badge
[forks-url]: https://github.com/King-Halo-Fan/Umamusume-Tracker/network/members
[stars-shield]: https://img.shields.io/github/stars/King-Halo-Fan/Umamusume-Tracker.svg?style=for-the-badge
[stars-url]: https://github.com/King-Halo-Fan/Umamusume-Tracker/stargazers
[issues-shield]: https://img.shields.io/github/issues/King-Halo-Fan/Umamusume-Tracker.svg?style=for-the-badge
[issues-url]: https://github.com/King-Halo-Fan/Umamusume-Tracker/issues
[license-shield]: https://img.shields.io/github/license/King-Halo-Fan/Umamusume-Tracker.svg?style=for-the-badge
[license-url]: https://github.com/King-Halo-Fan/Umamusume-Tracker/blob/main/LICENSE.txt
[product-screenshot]: images/screenshot.png

[HTML5-badge]: https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white
[HTML5-url]: https://developer.mozilla.org/en-US/docs/Web/HTML
[CSS3-badge]: https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white
[CSS3-url]: https://developer.mozilla.org/en-US/docs/Web/CSS
[JS-badge]: https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black
[JS-url]: https://developer.mozilla.org/en-US/docs/Web/JavaScript
[Supabase-badge]: https://img.shields.io/badge/Supabase-3ECF8E?style=for-the-badge&logo=supabase&logoColor=white
[Supabase-url]: https://supabase.com
[Fonts-badge]: https://img.shields.io/badge/Google%20Fonts-4285F4?style=for-the-badge&logo=google&logoColor=white
[Fonts-url]: https://fonts.google.com
