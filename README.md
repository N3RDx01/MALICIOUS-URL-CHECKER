# Malicious URL Checker

A lightweight client-side tool to detect potentially malicious URLs by checking them against a threat intelligence database. Built with vanilla JavaScript for easy integration and deployment.

## Features

- ðŸ” Real-time URL validation against known malicious domains
- ðŸŒ Client-side processing (no server required)
- ðŸ“± Responsive design that works on all devices
- ðŸ“‹ Scan history tracking with timestamps
- ðŸ“¤ Export scan logs as JSON for further analysis
- âŒ¨ï¸ Keyboard support (press Enter to scan)
- ðŸŒ™ Dark mode interface

## How It Works

1. Enter a URL or domain name in the input field
2. Click "Check URL" or press Enter
3. Get immediate visual feedback:
   - âœ… Green for safe domains
   - ðŸš¨ Red for malicious domains
   - âš ï¸ Yellow for invalid inputs
4. View scan history in the log section
5. Export all scan results as a JSON file

## Threat Intelligence

The checker uses a predefined list of known malicious domains stored in `maliciousDomains`. In a production environment, this could be replaced with:
- Real-time API calls to threat intelligence services
- Regularly updated domain blocklists
- Machine learning models for anomaly detection

## Usage

Simply open `index.html` in any modern browser. No installation or dependencies required.

### Example Domains

Try these examples:
- `phishing-bank.test` (Malicious)
- `https://github.com` (Safe)
- `malware-download.xyz` (Malicious)
- `google.com` (Safe)

## Technical Details

- **Framework**: Vanilla JavaScript (no dependencies)
- **Styling**: Pure CSS (no preprocessors)
- **Storage**: In-memory (refresh clears history)
- **Browser Support**: All modern browsers

## Security Notes

- This tool performs client-side checks only
- Does not send URLs to external servers
- Limited by the comprehensiveness of the local threat database
- Should be used as part of a broader security strategy

## Customization

To modify the threat database:
1. Edit the `maliciousDomains` array in the script section
2. Add/Remove domains as strings

To change styling:
1. Modify the CSS in the `<style>` section
2. Adjust colors, spacing, or layout as needed

## License

MIT License - see LICENSE file for details