# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project

PoolTrick is a browser-based game that will be packaged as a mobile app by wrapping the web build in a native container framework.

The repository is currently empty. No language, game engine, wrapper framework, build tooling or test setup has been chosen yet. Update this file as those decisions are made. Don't assume a stack that isn't in the repo.

## Architecture intent

- The game runs in a browser first, and the web build is the source of truth. Mobile builds wrap that same output rather than forking the game code.
- Keep game logic independent of the native wrapper. Native or device features (haptics, storage, orientation, app lifecycle) should go behind a thin adapter layer so the game still runs in a plain browser.
- Design input and layout for touch and mobile screen sizes, not only mouse and desktop.

## Commands

None yet. Add the build, dev-server, lint, test (including how to run a single test) and mobile build/sync commands here once the tooling exists.
