# AWS Workflows

## OCR Workflow

### Workflow JSON

The following JSON data is produced by OCR workflow:
```json
{
  "input-file" : "filename",
  "sequence" : [
    "convert",
    "threshold",
    "ocr"
  ],

  "convert": {
    "image-file" : "filename",
    "resolution" : "200",
    "input-format" : "bmp",
    "output-format" : "jpeg"
  },

  "threshold": {
    "image-file" : "filename"
  },

  "ocr": {
    "preprocessed-image" : "filename",
    "text-data-file" : "filename",
    "barcodes" : [
      {
        "type" : "type name",
        "data" : "barcode data",
        "data-file" : "barcode data file",
        "region" : {
          "x" : "x",
          "y" : "y",
          "width" : "width",
          "height" : "height"
        }
      }
    ]
  }
}
```
