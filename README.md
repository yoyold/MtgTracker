# MTG Tracker

[![Deploy to GitHub Pages](https://github.com/yoyold/MtgTracker/actions/workflows/deploy.yml/badge.svg)](https://github.com/yoyold/MtgTracker/actions/workflows/deploy.yml)
[![Live Demo](https://img.shields.io/website?url=https%3A%2F%2Fyoyold.github.io%2FMtgTracker%2F&label=live%20demo&up_message=online&down_message=offline)](https://yoyold.github.io/MtgTracker/)
[![.NET 9](https://img.shields.io/badge/.NET-9.0-512BD4?logo=dotnet&logoColor=white)](https://dotnet.microsoft.com/)
[![Blazor WebAssembly](https://img.shields.io/badge/Blazor-WASM-512BD4?logo=blazor&logoColor=white)](https://learn.microsoft.com/aspnet/core/blazor/)
[![License: MIT](https://img.shields.io/github/license/yoyold/MtgTracker)](LICENSE)
[![Last Commit](https://img.shields.io/github/last-commit/yoyold/MtgTracker)](https://github.com/yoyold/MtgTracker/commits/main)

A gamestate tracker for **Magic: The Gathering** — life points, counters, commander damage, turn timer and more.
Runs fully client-side as a Blazor WebAssembly PWA. No accounts, no server, no tracking.

**Live:** [yoyold.github.io/MtgTracker](https://yoyold.github.io/MtgTracker/)

![Page Preview](images/preview.png "Page Preview")

## Features

- **Players (1–6)** — life points, active-player tracking, turn counter
- **Dynamic counters** per player — +1/+1, −1/−1, Poison, Energy, Experience, Loyalty, Charge, Ki, Time, Fate, Quest, Storage, plus custom names
- **Commander format** — commander name, cast-based tax (+2 per cast), partner support, commander-damage grid per opponent with auto life deduction, 21-damage kill banner, emblem tracker
- **Turn timer & slow-play detection** — configurable threshold with visual warning
- **Shared board notes** — shared textarea for tracking complex states
- **Widget menu** — show/hide any widget, configure auto-loss rules (poison @ 10, commander damage @ 21, +1/+1 vs −1/−1 auto-cancel)
- **Utilities** — animated coin toss and dice roller (d4–d100) with history
- **PWA** — installable, works offline after first load

## Run locally

```bash
dotnet run -c Release
```

## Build

```bash
dotnet publish -c Release -o publish
```

Static output lands in `publish/wwwroot/` and can be hosted anywhere.

## Deployment

Pushes to `main` trigger [.github/workflows/deploy.yml](.github/workflows/deploy.yml), which publishes the app to GitHub Pages.

## License

[MIT](LICENSE)
