## Input Format

### Supported Formats

| Format | Content-Type |
|--------|-------------|
| PDF (single-page or multi-page) | `application/octet-stream` or `application/pdf` |

### Notes

- Input must be a valid PDF file sent as raw bytes.
- Both single-page and multi-page PDFs are supported.
- For batch transform jobs, upload each PDF as a separate S3 object and use `SplitType: None` with `BatchStrategy: SingleRecord` to prevent binary splitting.
