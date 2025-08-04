# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a static HTML website for the PT Jobs Hub, which presents Product Team responsibilities using the M.A.C.E. framework (Market Insight, Aim & Roadmap, Cross-team Execution, Evaluate & Iterate). The site is served by a custom Node.js HTTP server.

## Development Commands

### Start the server
```bash
npm start
# or
node server.js
```

The server runs on http://localhost:3000 by default.

### Change server port
Edit the `PORT` constant in `server.js:7` to use a different port.

## Architecture

- **Static Website**: Pure HTML/CSS/JS frontend with no build process
- **Custom HTTP Server**: Simple Node.js server in `server.js` that serves static files
- **File Structure**:
  - `index.html`: Main homepage
  - `outcomes/`: Individual HTML pages for each M.A.C.E. component
  - `css/styles.css`: All styling (no preprocessors)
  - `js/script.js`: Minimal client-side JavaScript
  - `server.js`: HTTP server with MIME type handling and security checks

## Key Features

- **Security**: Directory traversal protection in `server.js:38-43`
- **Error Handling**: Custom 404 page with styling
- **MIME Types**: Configured for common web assets in `server.js:11-22`
- **Responsive Design**: CSS uses flexbox and grid layouts
- **Navigation**: Dropdown menu system for outcomes pages

## Content Organization

The site is organized around the M.A.C.E. framework:
- **M**: Market Insight (market understanding, competitor analysis)
- **A**: Aim & Roadmap (product roadmaps, requirements)
- **C**: Cross-team Execution (project coordination, releases)
- **E**: Evaluate & Iterate (KPIs, funnel analysis)

Each component has a dedicated page in the `outcomes/` directory with detailed explanations and deliverables.