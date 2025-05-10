# 🚗 Egyptian License Plate Recognition (Streamlit App)

A Streamlit-based web application for detecting and recognizing Egyptian vehicle license plates using YOLO models and custom OCR logic.

## 🔍 Features

- Upload or capture an image using a camera
- Detect license plates in images using YOLO
- Perform OCR to extract Arabic characters and numbers
- Convert detected elements to Arabic format
- Automatically classify the governorate based on plate structure
- Bilingual interface: English and Arabic
- Download processed results as images
- python version >> 3.11
## 🗂 Project Structure

```
project/
│
├── web/
│   ├── web.py              ← Main Streamlit app
│   ├── depiweb.py          ← Plate detection + OCR logic
│   ├── best.pt             ← OCR model
│   ├── plate.pt            ← License plate detector
│   ├── yolo11n.pt          ← Optional general object detector
│   └── requirements.txt    ← Dependencies
│
└── README.md
```

## 🚀 How to Run

1. Open a terminal and navigate to the `web` folder:

   ```bash
   cd web
   ```

2. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```

3. Ensure the following model files are in the same folder:
   - `best.pt`
   - `plate.pt`
   - `yolo11n.pt` (optional)

4. Start the app:

   ```bash
   python -m streamlit run web.py
   ```

5. The web app will open in your browser.

## 📝 Notes

- Make sure your webcam permissions are allowed when using the "Use Camera" option.
- The app supports both English and Arabic interface (selectable at the top).
- Governorate classification is based on the recognized plate letters.

## 📄 License

MIT License.
