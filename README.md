# Stone-Network
Distributed relay network with real-time data broadcasting

# Stone Network 🌐

A distributed relay network system for real-time data broadcasting and monitoring.

## Architecture

### Global Node 1 - Source (Broadcaster)
- **File:** `index.html`
- **URL:** `https://thetheorizingstone.github.io/Stone-Network/`
- **Function:** Generates and broadcasts random data (0-100) to cloud relay every 1.5 seconds
- **PIN:** `1`

### Global Node 2 - Interface (Receiver)
- **File:** `interface.html`
- **URL:** `https://thetheorizingstone.github.io/Stone-Network/interface.html`
- **Function:** Polls cloud relay every 1 second and displays live data
- **PIN:** `2`
- **Wix Integration:** Embed in Wix iframe for live display

## Cloud Bridge

- **Service:** kvdb.io (free key-value database)
- **Channel ID:** `stone_relay_777`
- **Method:** REST API polling

## Setup

1. Clone this repository
2. Enable GitHub Pages in Settings (Source: main branch)
3. Access nodes at URLs above
4. Enter PIN to activate each node

## Usage in Wix

Add this HTML component to your Wix page:

```html
<iframe 
  src="https://thetheorizingstone.github.io/Stone-Network/interface.html" 
  style="width:100%; height:400px; border:none; background:#05070a;"
  allow="*">
</iframe>
```

## Security Notes

- PINs are basic; for production, implement proper authentication
- kvdb.io free tier has rate limits
- Consider HTTPS-only connections for production

## License
Copyright protected by Travis Raymond-Charlie Stone