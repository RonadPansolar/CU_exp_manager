# CU_exp_manager
This project builds a deep-learning pipeline that automatically extracts barcodes, product names, and expiration dates from convenience-store product images. It aims to reduce manual work, improve management accuracy, and provide a reproducible structure that others can easily understand, run, and extend.  <br/>
Input Image
<br/>   ↓
<br/>YOLO Detection
<br/>   ↓
<br/>Crop Regions
<br/>   ├─ Barcode → ZXing multi-try decoding
<br/>   ├─ Product Name → Donut or Swin+ByT5
<br/>   └─ Expiration Date → OCR / model-based extraction
<br/>   ↓
<br/>Postprocessing
<br/>   ↓
<br/>CSV / JSON output
