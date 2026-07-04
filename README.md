# IFTAS DNI

A simple single-page HTML tool for converting the IFTAS DNI CSV list into a plain newline-separated list of domains.

The tool runs entirely in the browser. No data is uploaded or sent anywhere.

## Source

The source CSV is available from IFTAS:

https://about.iftas.org/library/iftas-dni-list/

## Usage

1. Open `index.html` in your browser.
2. Paste the IFTAS DNI CSV into the input box.
3. The domains will be extracted automatically.
4. Click **Copy domains** to copy the newline-separated domain list to your clipboard.

## Expected CSV Format

```csv
#domain,#severity,#reject_media,#reject_reports,#public_comment,#obfuscate
example.org,suspend,FALSE,FALSE,iftas:hate-speech;online-harassment,TRUE
example.com,suspend,FALSE,FALSE,iftas:hate-speech;online-harassment,TRUE
```

## Output Format

```txt
example.org
example.com
```

## License

MIT
