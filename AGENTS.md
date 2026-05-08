# AGENTS.md

This file provides guidance to Codex (Codex.ai/code) when working with code in this repository.

## Project Overview
Static personal homepage hosted as a GitHub Pages user site (junfeng1212.github.io). Deploys automatically from the `main` branch with no build step required.

## Architecture
- Single-page site: All HTML, CSS, and JS are inline in `index.html`
- Assets: `avatar.jpg` (profile image) located in the root directory
- No build tooling, dependencies, or test suite

## Development
- Edit `index.html` directly to update site content or styling
- Commit changes to the `main` branch to trigger immediate GitHub Pages deployment
- No build, lint, or test commands are needed for this project
