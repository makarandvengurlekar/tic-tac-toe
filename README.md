# Tic-Tac-Toe

A clean, modern, and fully responsive **Tic-Tac-Toe** game built with **HTML5, CSS3, and vanilla JavaScript** — no frameworks, no build step, and no backend. It runs directly in any web browser and is ready to publish on GitHub Pages.

![No frameworks](https://img.shields.io/badge/frameworks-none-brightgreen)
![No build step](https://img.shields.io-badge/build-none-blue)
![License: MIT](https://img.shields.io/badge/license-MIT-green)

---

## Features

- **Main menu** to choose a game mode.
- **Single Player** mode — you play as **X** against a built-in computer **O**.
- **Multiplayer** mode — two players take turns on the same device (Player 1 = X, Player 2 = O).
- **Sensible computer AI** that tries to win, blocks your winning moves, and otherwise plays a reasonable move.
- **X always moves first** in every game.
- **Correct win and draw detection** for all eight winning combinations.
- **Winning combination highlighting** with a subtle animation.
- **Clear result message** and a status line showing whose turn it is.
- **Play Again** to restart (keeps the chosen mode) and **Main Menu** to return without reloading.
- **Responsive layout** that works on desktop, tablet, and mobile screens.
- **Accessible & keyboard-friendly** controls with good color contrast and reduced-motion support.

## Technologies Used

- HTML5 — page structure
- CSS3 — styling, layout, and animations
- Vanilla JavaScript (ES6) — all game logic

No React, Vue, Angular, TypeScript, Bootstrap, Tailwind, jQuery, or any other library or framework is used.

## Project Structure

```
tic-tac-toe/
├── index.html      # Markup for the menu and game screens
├── style.css       # All styling, layout, and animations
├── script.js       # All game logic (vanilla JavaScript)
├── README.md       # Project documentation
└── .gitignore      # Files to ignore in version control
```

## Running the Game Locally

Because this is a purely static project, you only need a web browser. Choose whichever method is easiest for you:

**Option 1 — Open the file directly**
1. Open the project folder.
2. Double-click `index.html` to open it in your default browser.

**Option 2 — Run in Visual Studio Code (recommended)**
1. Open the `tic-tac-toe` folder in VS Code.
2. Install the **Live Server** extension (by Ritwick Dey) from the Extensions Marketplace.
3. Right-click `index.html` and choose **"Open with Live Server"**.
4. The game will open in your browser and reload automatically when you save changes.

**Option 3 — Any simple static server**
Serve the folder with any static file server, for example:

```bash
# Python 3
python -m http.server 8000

# Node.js (if you have the "serve" package)
npx serve
```

Then open `http://localhost:8000` in your browser.

## Publishing with GitHub Pages

The game is a static site with no build step, so it can be hosted directly on GitHub Pages.

### 1. Initialize Git in the project folder
```bash
cd tic-tac-toe
git init
```

### 2. Create a repository on GitHub
Go to [github.com/new](https://github.com/new), give the repository a name (for example `tic-tac-toe`), set it to **Public**, and click **Create repository** (do **not** add a README, `.gitignore`, or license — the project already has them).

### 3. Connect your local project to the repository
Replace `YOUR-USERNAME` with your GitHub username and `REPO-NAME` with your repository name:
```bash
git add .
git commit -m "Initial commit: Tic-Tac-Toe game"
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/REPO-NAME.git
git push -u origin main
```

### 4. Enable GitHub Pages
1. In your repository on GitHub, open **Settings → Pages**.
2. Under **Source**, select the **`main`** branch and the **`/ (root)`** folder, then click **Save**.
3. Wait a minute or two, then visit:
   `https://YOUR-USERNAME.github.io/REPO-NAME/`

> **Note on file paths:** All links in `index.html` are relative (`style.css` and `script.js`), so the game works correctly whether it is hosted at the root of a domain or inside a repository subdirectory (as with GitHub Pages).

## How to Contribute

Contributions are welcome! To keep things organized:

1. **Fork** the repository (click the "Fork" button on GitHub).
2. **Clone** your fork locally:
   ```bash
   git clone https://github.com/YOUR-USERNAME/REPO-NAME.git
   ```
3. **Create a branch** for your change:
   ```bash
   git checkout -b feature/my-new-feature
   ```
4. **Make your changes** and test them in a browser.
5. **Commit** with a clear message:
   ```bash
   git commit -m "Add: short description of the change"
   ```
6. **Push** to your fork and open a **Pull Request** describing what you changed and why.

Please keep the code clean and consistent with the existing style, and avoid adding frameworks or build tools.

## Testing Checklist

Use this list to verify the game works as expected:

- [ ] The main menu shows the title and both mode buttons.
- [ ] Single Player: you are **X**, the computer is **O**, and **X** moves first.
- [ ] Multiplayer: Player 1 (**X**) and Player 2 (**O**) alternate turns.
- [ ] The computer never overwrites an occupied cell and never moves after the game ends.
- [ ] All eight winning combinations are detected and highlighted.
- [ ] A draw is detected when the board fills with no winner.
- [ ] Occupied cells cannot be selected again.
- [ ] No moves can be made after a win or draw.
- [ ] **Play Again** resets the board, clears the result, and keeps the current mode.
- [ ] **Main Menu** returns to the menu, and switching modes resets the game.
- [ ] The layout looks good on a small (mobile) screen.

## License

This project is released under the [MIT License](LICENSE). You are free to use, modify, and share it.
