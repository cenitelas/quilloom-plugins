# document-skills

Document processing skills for Quilloom Code: PDF, Word (DOCX), Excel (XLSX), PowerPoint (PPTX).

Each skill parses the file **client-side** and feeds extracted text to the model, so even text-only coding models can work with binary documents.

## Install

```
/extensions install cenitelas/quilloom-plugins:document-skills
```

## Skills

| Skill | What it does |
|---|---|
| `pdf` | Read, extract text/tables, merge, split, rotate, watermark, fill forms, encrypt/decrypt, OCR |
| `docx` | Read and generate Word documents |
| `xlsx` | Read and generate Excel spreadsheets |
| `pptx` | Read and generate PowerPoint decks |

## Usage

After install, just reference a document in your prompt — Quilloom Code detects the file type and invokes the right skill automatically:

```
extract the tables from report.pdf
```

```
summarize the action items in meeting-notes.docx
```

## Credits

Based on Anthropic's open-source skills marketplace (`anthropics/skills`), adapted for Quilloom.
