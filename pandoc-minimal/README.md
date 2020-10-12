# Minimal Pandoc: Convert docx to md

Use-case: easy conversion from MS Word .docx (useful for generic compatibility between software including google docs) and Markdown (useful for blog publishing).

Example usage:

```
docker build -t almad/pandoc-minimal .
docker run --rm -v "/tmp/tmpdir:/docs" almad/pandoc-minimal pandoc /docs/doc.docx -f docx -t markdown -o /docs/doc.md
```
