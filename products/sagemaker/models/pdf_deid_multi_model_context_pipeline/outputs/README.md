## Output Format

### Supported Formats

| Format | Content-Type |
|--------|-------------|
| PDF (de-identified) | `application/octet-stream` or `application/pdf` |

### Notes

- Output is a de-identified PDF matching the structure and page count of the input.
- PHI entities (names, dates, locations, etc.) are redacted or obfuscated in the output PDF.
- The output file can be downloaded directly from the endpoint response body or from S3 after a batch transform job.
