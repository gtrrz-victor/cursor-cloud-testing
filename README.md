# Clock Football

A terminal game that plays like clock football: two players, one tick at a time, and `00` is a goal.

This project is planned as a small Go CLI built with [Bubble Tea](https://github.com/charmbracelet/bubbletea). The repo is empty today; this README describes what it will become.

## The game

Clock football is a two-player match on a clock face.

- Each player has a color.
- A tick starts the play and moves the clock.
- When the clock lands on `00`, that play is a goal.
- The match continues until someone wins, or until the players quit.

The terminal UI will show the clock, both scores, and whose turn it is.

## Planned stack

- **Go** for the CLI
- **Bubble Tea** for the interactive TUI
- **Lip Gloss** for colors and layout, so each player has a clear identity on screen

## Planned shape

- `cmd/` — entrypoint for the `clock-football` command
- `internal/game` — rules: ticks, turns, goals, score
- `internal/ui` — Bubble Tea model: clock, scoreboard, player colors

## Roadmap

1. Start a match from the command line
2. Tick to play, land on `00` to score
3. Two players, one color each, live scoreboard
4. Keyboard controls to start, tick, and quit

## Status

Not implemented yet. The next step is the Go CLI and the first playable tick.
