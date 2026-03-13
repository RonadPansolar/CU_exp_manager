# CU_exp_manager
This project builds a deep-learning pipeline that automatically extracts barcodes, product names, and expiration dates from convenience-store product images. It aims to reduce manual work, improve management accuracy, and provide a reproducible structure that others can easily understand, run, and extend.
Input Image
   ↓
YOLO Detection
   ↓
Crop Regions
   ├─ Barcode → ZXing multi-try decoding
   ├─ Product Name → Donut or Swin+ByT5
   └─ Expiration Date → OCR / model-based extraction
   ↓
Postprocessing
   ↓
CSV / JSON output
