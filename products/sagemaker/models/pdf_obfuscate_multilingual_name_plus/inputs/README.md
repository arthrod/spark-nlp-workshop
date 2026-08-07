## Input Format

### Supported Content Types

| Content-Type |
|---|
| `application/octet-stream` |
| `application/pdf` |
| `image/png` |
| `image/jpeg` |
| `image/bmp` |
| `image/tiff` |
| `image/gif` |

### Notes

- Input must be a valid PDF or image file sent as raw bytes.
- Both single-page and multi-page PDFs are supported.
- `application/octet-stream` is accepted for any supported format — the model detects the file type automatically from the binary content.
- For batch transform jobs, upload each file as a separate S3 object and use `SplitType: None` with `BatchStrategy: SingleRecord` to prevent binary splitting.
