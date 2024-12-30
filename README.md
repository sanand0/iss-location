# ISS Location Data Collection

Automated collection of International Space Station (ISS) position data using GitHub Actions. The data is collected daily at 12:00 UTC and stored in JSONL format.

- Data provided by [Open Notify](http://open-notify.org/)
- Powered by [GitHub Actions](https://github.com/features/actions)

## Data Collection

- **Frequency**: Daily at 12:00 UTC
- **Source**: [Open Notify ISS Position API](http://api.open-notify.org/iss-now.json)
- **Format**: JSONL (JSON Lines)
- **Storage**: `iss-location.jsonl`

## Data Format

Each line in the JSONL file looks like this:

```json
{
  "message": "success",
  "iss_position": {"latitude": "0.5776", "longitude": "131.0008"},
  "timestamp": 1735520294
}
```

## License

[MIT](https://opensource.org/license/mit)
