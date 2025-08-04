# PT Jobs Hub

A central hub website for viewing all aspects of Product Team (PT) jobs using the M.A.C.E. framework.

## Overview

This website provides a comprehensive view of Product Team responsibilities organized around the M.A.C.E. framework:
- **M** - Market Insight
- **A** - Aim & Roadmap
- **C** - Cross-team Execution
- **E** - Evaluate & Iterate

## Access the Hub

### Live Website (Recommended)
The PT Jobs Hub is deployed and accessible via GitHub Pages:

🌐 **https://tom-dynamsoft.github.io/pt-jobs-hub/**

No setup required - simply visit the link above to explore the M.A.C.E. framework and all Product Team outcomes.

## Local Development

### Prerequisites
- Node.js (version 12 or higher)

### Running the Server

1. Navigate to the project directory:
   ```bash
   cd D:\work\pt-jobs-hub
   ```

2. Start the server using Node.js:
   ```bash
   node server.js
   ```
   
   Or using npm:
   ```bash
   npm start
   ```

3. Open your web browser and visit:
   ```
   http://localhost:3000
   ```

4. To stop the server, press `Ctrl+C` in the terminal.

## Project Structure

```
pt-jobs-hub/
├── index.html          # Main homepage
├── server.js           # Node.js HTTP server
├── package.json        # Project configuration
├── README.md           # This file
├── css/
│   └── styles.css      # Website styling
├── js/
│   └── script.js       # Interactive functionality
├── outcomes/           # Individual outcome pages
│   ├── market-insight.html
│   ├── aim-roadmap.html
│   ├── cross-team-execution.html
│   └── evaluate-iterate.html
└── images/            # Image assets (if any)
```

## Features

- Clean, professional design
- Responsive layout
- Easy navigation with dropdown menus
- Detailed outcome pages for each M.A.C.E. component
- Simple Node.js server for local development

## Customization

To customize the content:
1. Edit the HTML files to update text and structure
2. Modify `css/styles.css` for styling changes
3. Update `js/script.js` for additional functionality

## Server Configuration

The server runs on `http://localhost:3000` by default. To change the port:
1. Open `server.js`
2. Change the `PORT` variable to your desired port number
3. Restart the server

## Troubleshooting

- **Port already in use**: Change the PORT in server.js or stop the other process
- **404 errors**: Make sure you're accessing files that exist in the project
- **Permission errors**: Run the terminal as administrator if needed
