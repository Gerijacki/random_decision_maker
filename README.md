# Decision Maker

A roulette-style app for Flipper Zero that **lets you type your own choices** and then picks one at random — perfect for when you can't make up your mind.

Add as many decisions as you want (up to 20), delete them one by one, and spin whenever you're ready.

## How to Use

### Manage screen

| Button | Action |
|--------|--------|
| **UP / DOWN** | Navigate the list |
| **OK** *(cursor on "Añadir")* | Open the keyboard to type a new decision |
| **OK** *(cursor on a decision, ≥ 2 total)* | Shortcut to spin immediately |
| **LEFT** | Delete the highlighted decision |
| **RIGHT** | Spin the roulette (requires ≥ 2 decisions) |
| **BACK** | Exit the app |

### Keyboard screen

Type your decision (up to 20 characters), then press **OK** to confirm or **BACK** to cancel.

### Spinning screen

The roulette cycles through your options at full speed, then gradually slows down and lands on the chosen one. A progress bar shows how close it is to stopping.

### Result screen

| Button | Action |
|--------|--------|
| **OK** | Spin again with the same list |
| **BACK** | Return to the manage screen |

## Building

### With fbt (full firmware repo)

```bash
# From the root of flipperzero-firmware:
./fbt fap_random_decision_maker
```

The `.fap` file is placed in `dist/f7-D/apps/Games/random_decision_maker.fap`.

### With ufbt (standalone, recommended)

```bash
pip install ufbt
cd random_decision_maker/
ufbt
```

## Requirements

- Flipper Zero with official firmware (Release or Release Candidate).
- No external hardware required — screen and buttons only.

## License

MIT License — see [LICENSE](LICENSE).
