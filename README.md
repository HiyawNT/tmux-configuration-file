# 🧩 Tmux Configuration README

This repository contains a custom **tmux configuration** focused on productivity, fast navigation, and a clean UI. It introduces intuitive keybindings, vi-style copy mode, and efficient pane/window/session management.

---

## 🚀 Key Features

* Custom prefix (`Ctrl + Space`)
* Vi-style copy mode
* Fast pane and window navigation (no prefix required)
* Session management shortcuts
* Mouse support enabled
* Clean, minimal status bar
* Smart window naming based on current path

---

## ⌨️ Prefix Key

| Action           | Key            |
| ---------------- | -------------- |
| Primary Prefix   | `Ctrl + Space` |
| Secondary Prefix | `Ctrl + b`     |

---

## 🔄 Reload Config

| Action             | Key          |
| ------------------ | ------------ |
| Reload tmux config | `Prefix + q` |

---

## 📋 Copy Mode (Vi-style)

| Action          | Key                    |
| --------------- | ---------------------- |
| Enter copy mode | `Prefix + [` (default) |
| Start selection | `v`                    |
| Copy selection  | `y`                    |

---

## 🧱 Pane Management

### Split Panes

| Action             | Key          |
| ------------------ | ------------ |
| Split vertically   | `Prefix + h` |
| Split horizontally | `Prefix + v` |
| Kill pane          | `Prefix + x` |

### Navigate Panes (No Prefix)

| Direction | Key              |
| --------- | ---------------- |
| Left      | `Ctrl + Alt + ←` |
| Right     | `Ctrl + Alt + →` |
| Up        | `Ctrl + Alt + ↑` |
| Down      | `Ctrl + Alt + ↓` |

### Resize Panes (No Prefix)

| Direction    | Key                      |
| ------------ | ------------------------ |
| Resize Left  | `Ctrl + Alt + Shift + ←` |
| Resize Right | `Ctrl + Alt + Shift + →` |
| Resize Up    | `Ctrl + Alt + Shift + ↑` |
| Resize Down  | `Ctrl + Alt + Shift + ↓` |

---

## 🪟 Window Management

| Action        | Key          |
| ------------- | ------------ |
| New window    | `Prefix + c` |
| Rename window | `Prefix + r` |
| Kill window   | `Prefix + k` |

### Switch Windows (No Prefix)

| Action          | Key          |
| --------------- | ------------ |
| Window 1–9      | `Alt + 1..9` |
| Next window     | `Alt + →`    |
| Previous window | `Alt + ←`    |

### Reorder Windows

| Action            | Key               |
| ----------------- | ----------------- |
| Move window left  | `Alt + Shift + ←` |
| Move window right | `Alt + Shift + →` |

---

## 🧵 Session Management

| Action           | Key          |
| ---------------- | ------------ |
| New session      | `Prefix + C` |
| Rename session   | `Prefix + R` |
| Kill session     | `Prefix + K` |
| Previous session | `Prefix + P` |
| Next session     | `Prefix + N` |

### Quick Switch (No Prefix)

| Action           | Key       |
| ---------------- | --------- |
| Previous session | `Alt + ↑` |
| Next session     | `Alt + ↓` |

---

## ⚙️ General Settings

* **Terminal:** `tmux-256color` with true color support
* **Mouse:** Enabled
* **History limit:** 50,000 lines
* **Window & pane indexing:** Starts at 1
* **Auto-renumber windows:** Enabled
* **Clipboard integration:** Enabled
* **Focus events:** Enabled
* **Aggressive resize:** Enabled
* **No auto-detach on session destroy**

---

## 🎨 Status Bar & UI

* Positioned at the **top**
* Minimal, clean theme
* Active elements highlighted in **blue**
* Shows:

  * Session name
  * Window list
  * Hostname
  * Prefix/zoom indicators

### Smart Window Naming

Windows automatically rename based on current directory:

```
#{b:pane_current_path}
```

---

## 📌 Notes

* Many keybindings **do not require the prefix**, making navigation faster.
* Designed for **keyboard-heavy workflows**.
* Works best with terminals that support:

  * True color
  * Alt/Meta key combinations

---

## 🛠 Installation

1. Save config to:

   ```
   ~/.config/tmux/tmux.conf
   ```

2. Reload tmux:

   ```
   Prefix + q
   ```

Or restart tmux:

```
tmux kill-server && tmux
```

---

## 💡 Tips

* If keybindings don’t work, check terminal support for `Alt` and `Ctrl+Alt+Shift`.
* Use `tmux list-keys` to debug bindings.
* Combine with tools like `fzf`, `zoxide`, or `k9s` for a powerful workflow.

---

## 📄 License

Feel free to modify and adapt this configuration to your needs.
