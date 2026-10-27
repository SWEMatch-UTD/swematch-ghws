# swematch-ghws

SWEMatch Git/GitHub Workshop: a shared web page where each team loads a random animal photo from an API.

## How it works

1. `index.html` shows one card per team, each with an image slot, a button, and three spots for names.
2. `script.js` has one function per team that fetches an image URL from that team's animal API. Clicking a team's button shows the picture in its slot.
3. If a request fails, the slot shows the error message.
4. `styles.css` styles the page and the buttons. Team branches start without it, and you get it by pulling from `main`.

## Files

| File | Purpose |
| --- | --- |
| `index.html` | Page structure |
| `script.js` | Button click handler and each team's API call |
| `styles.css` | Page and button styling |
| `GIT_COMMANDS.md` | Cheat sheet of the git commands used in the workshop |

## Running

No build step or dependencies. Open `index.html` in a browser (it needs an internet connection), then click a button.

## Workshop flow

1. Check out your team's branch.
2. Pull `styles.css` from `main`.
3. Do your tasks (see your `TEAMn_TASK.txt`).
4. `git add`, `git commit`, `git push`.
5. Open a pull request into `main` on GitHub.

## Branches

- feat/team1-dog
- feat/team2-cat
- feat/team3-monkey
- feat/team4-fish
- feat/team5-bird
- feat/team6-fox
