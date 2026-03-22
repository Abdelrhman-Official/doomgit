# DOOM.git

> Every frame of DOOM is a git commit.
> Your death is in the git log.
> You can `git bisect` to find exactly when you got hit.

---

## 🎮 Demo (this is what goes viral)

```
$ doomgit log

commit a4f2b91  frame 4521 | E1M1 | health:72 kills:3
................................................................................
......########......################################################............
......#      #......#                                            #............
......# DOOM #......#         [player here] ---->               #............

$ git checkout HEAD~50
# ⏪ You just moved back in time

$ doomgit bisect --when "health < 50"
# 🎯 Finds the exact moment you got hit
```

---

## 💡 What is this?

**DOOM.git** turns Git into a game engine.

* Every frame = a commit
* Game state = Git objects
* Saves = branches
* Death = detached HEAD
* Time travel = `git checkout`

---

## 🔥 Features

* 🧠 Play DOOM through Git history
* ⏪ Rewind gameplay with `git checkout`
* 🔍 Find your death with `git bisect`
* 💾 Save runs as branches
* 🌍 Share full playthroughs via GitHub
* 🖥️ ASCII-rendered frames in terminal

---

## ⚡ Quick Start

```bash
git clone https://github.com/Abdelrhman-Official/doomgit
cd doomgit

make build
pip install -e .

doomgit init
doomgit play
```

---

## 🕹️ Commands

| Command             | Description               |
| ------------------- | ------------------------- |
| `doomgit play`      | Start the game            |
| `doomgit rewind 50` | Go back 50 frames         |
| `doomgit save run1` | Save progress             |
| `doomgit load run1` | Load save                 |
| `doomgit log`       | View gameplay in git log  |
| `doomgit bisect`    | Find when you took damage |

---

## 🤯 Why this exists

Because Git was never meant to be a game engine.

And that's exactly why it works.

---

## 🧱 How it works (simple)

* DOOM engine renders frames
* Frames → ASCII
* Stored as Git commits via `pygit2`
* Game state saved in blobs
* CLI navigates history

Full details → see `ARCHITECTURE.md`

---

## 📸 Demo Idea (record this!)

* Run `doomgit play`
* Show `git log` updating live
* Run `git checkout HEAD~100`
* Show rewind
* End with `git bisect`

---

## 🤝 Contributing

PRs welcome.

Ideas to build:

* Colored rendering
* Multiplayer spectate
* Web viewer
* Performance improvements

---

## ⭐ Star History

If this made you say “what??” — give it a star 😄

---

## 📜 License

apeche 2.0
