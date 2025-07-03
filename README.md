# LiteSpeed Universal Updater

Simple bash script for automatic LiteSpeed Web Server updates via cron. Works with both LiteSpeed Enterprise (LSE) and OpenLiteSpeed (OLS).

## Features

- **Universal**: Works with both LSE and OLS installations
- **Bandwidth efficient**: Only downloads updates when needed
- **Simple**: No complex configuration or dependencies
- **Cron-ready**: Designed to run unattended in cron jobs

## How it works

- **OpenLiteSpeed**: Checks current version against latest release, downloads only if different
- **LiteSpeed Enterprise**: Uses built-in version checking mechanism (no unnecessary downloads)

## Installation

1. Download the script:
```bash
wget https://raw.githubusercontent.com/yourusername/litespeed-updater/main/litespeed-updater
```

2. Make it executable:
```bash
chmod +x litespeed-updater
```

3. Move to system PATH:
```bash
sudo mv litespeed-updater /usr/local/bin/
```

## Usage

### Manual execution
```bash
/usr/local/bin/litespeed-updater
```

### Automated via cron
Add to your crontab to run weekly on Sunday at 2 AM:
```bash
0 2 * * 0 /usr/local/bin/litespeed-updater
```

## Requirements

- LiteSpeed Web Server (LSE or OLS) already installed
- `curl` command available
- Root access for updates

## License

MIT License

## Contributing

1. Fork the repository
2. Create your feature branch
3. Commit your changes
4. Push to the branch
5. Create a Pull Request

## Support

For issues and questions, please use the GitHub issue tracker.
