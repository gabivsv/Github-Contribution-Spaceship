# 🚀 GitHub Contribution Spaceship
[🇧🇷 Português](README.pt-BR.md)
> **Turn your GitHub contribution graph into a journey through space.** 🌌

A custom space animation for GitHub contribution graphs, built with JavaScript, Node.js, SVG, CSS, and GitHub Actions.

Instead of the traditional snake 🐍, this project transforms the contribution calendar into a starry sky, where a spaceship travels along a route formed by the most active weeks. ✨

---

## 🌌 Demo

<picture>
  <source
    media="(prefers-color-scheme: dark)"
    srcset="https://raw.githubusercontent.com/gabivsv/github-contribution-spaceship/output/github-contribution-spaceship-dark.svg?v=1">

<source
 media="(prefers-color-scheme: light)"
 srcset="https://raw.githubusercontent.com/gabivsv/github-contribution-spaceship/output/github-contribution-spaceship.svg?v=1">

<img
 alt="Nave espacial percorrendo o gráfico de contribuições"
 src="https://raw.githubusercontent.com/gabivsv/github-contribution-spaceship/output/github-contribution-spaceship.svg?v=1"> </picture>

---

## 🛰️ How does it work?

The project queries the **GitHub contribution calendar** and transforms this data into an animated SVG visualization while preserving the real GitHub data.

* ⭐ Each contribution is represented by a star according to the activity level;
* 🌠 One highlighted star is selected per week to form the route;
* 🛸 The spaceship travels along this route and visually interacts with the stars;
* ⚙️ GitHub Actions automatically generates the graph versions for light and dark themes.

---

## 🧠 Technologies

| Technology                  | Use                             |
| --------------------------- | ----------------------------    |
| 🟨 **JavaScript / Node.js** | Graph logic and generation      |
| 🎨 **SVG**                  | Visualization construction      |
| ✨ **CSS**                  | Animations and visual effects   |
| ⚙️ **GitHub Actions**       | Generation automation           |
| 🔗 **GitHub GraphQL API**   | Contribution queries            |

---

## 📁 Project structure

```text
github-contribution-spaceship/
│
├── .github/
│   └── workflows/
│       └── spaceship.yml       # Runs and publishes the generator
│
├── src/
│   ├── github.mjs              # Queries contributions
│   ├── stars.mjs               # Creates stars, legend, and route
│   ├── spaceship.mjs            # Draws the spaceship
│   ├── animation.mjs            # Defines CSS animations
│   └── generate.mjs             # Combines the components and generates the SVG
│
├── README.md                    # Documentation
├── LICENSE                      # Project license
```

---

## 🚀 Use it on your own profile

**Fork** this repository and adapt it to your GitHub profile.

The profile repository must have the same name as your username:

```text
YOUR_USERNAME/YOUR_USERNAME
```
Then:

* Copy the `src/` folder and the workflow `.github/workflows/spaceship.yml`.
* Create a branch named `output`.
* Under **Settings → Actions → General → Workflow permissions**, enable **Read and write permissions**.
* Run the workflow under **Actions → Generate contribution spaceship → Run workflow**.
---

## 👤 Add it to your profile README

After the workflow finishes, add the following snippet to your profile README.

Replace `YOUR_USERNAME` with your GitHub username:

```html
<picture>
  <source
    media="(prefers-color-scheme: dark)"
    srcset="https://raw.githubusercontent.com/YOUR_USERNAME/YOUR_USERNAME/output/github-contribution-spaceship-dark.svg?v=1">

  <source
    media="(prefers-color-scheme: light)"
    srcset="https://raw.githubusercontent.com/YOUR_USERNAME/YOUR_USERNAME/output/github-contribution-spaceship.svg?v=1">

  <img
    alt="Nave espacial percorrendo o gráfico de contribuições"
    src="https://raw.githubusercontent.com/YOUR_USERNAME/YOUR_USERNAME/output/github-contribution-spaceship.svg?v=1">
</picture>
```

## 🧩 Architecture

The project's main flow can be summarized as follows:

```text
GitHub GraphQL API
        ↓
Contribution calendar
        ↓
Data processing
        ↓
Stars + activity levels
        ↓
Route definition
        ↓
Spaceship
        ↓
SVG + CSS
        ↓
GitHub Actions
        ↓
Image displayed in the README
```

---

## 👩🏻‍🚀 Author

This project was conceived and customized by **@gabivsv**, using JavaScript, Node.js, SVG, CSS, and GitHub Actions, with AI assistance in parts of the implementation.

---

## 📄 License

This project is available under the **MIT License**.

