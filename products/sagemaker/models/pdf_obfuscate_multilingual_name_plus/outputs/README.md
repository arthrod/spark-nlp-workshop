## Output Format

### Supported Content Types

| Content-Type |
|---|
| `application/octet-stream` |
| `application/pdf` |
| `image/png` |

### Notes

- Output is an obfuscated file where PHI entities (names, dates, locations, IDs, etc.) are replaced with realistic fake values rendered directly onto the document.
- PDF input returns an obfuscated PDF matching the structure and page count of the input.
- Image input always returns an obfuscated PNG regardless of the original image format (JPEG, BMP, TIFF, GIF inputs all produce PNG output).
- The output file can be downloaded directly from the endpoint response body or from S3 after a batch transform job.
