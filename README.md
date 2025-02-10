# Medical_DataExtraction_OCR_Project
This project focuses on efficient medical data extraction by converting patient details or prescriptions from PDFs into structured digital data. The process starts with converting the PDF to an image using `pdf2image`, followed by image enhancement through thresholding with OpenCV to improve text clarity. The refined image is then processed with `pytesseract` for accurate text extraction. Using `regex`, the extracted data is categorized and assigned to specific variables. Finally, the structured data is served via a `FastAPI` server, enabling seamless and efficient retrieval for medical applications.

## Project Structure  

- **backend/**: Contains the FastAPI backend server code.  
  - **src/**: Holds the FastAPI application code.  
  - **test/**: Contains test cases for the backend.  
  - **resources/**: Stores PDFs of patient details and prescriptions.  
- **requirements.txt**: Lists the required Python packages.  
- **README.md**: Provides an overview and instructions for the project.

## Setup Instructions

1. **Clone the repository**:
   ```bash
   git clone https://github.com/BhuvanKalyanGV/Medical_DataExtraction_OCR_Project.git
   cd Medical_DataExtraction_OCR_Project
   ```
1. **Install dependencies:**:   
   ```commandline
    pip install -r requirements.txt
   ```
1. **Run the FastAPI server:**:   
   ```commandline
    uvicorn server.server:app --reload
   ```
   
## Author
Bhuvan Kalyan G V
[LinkedIn: in/bhuvan-kalyan-g-v](https://www.linkedin.com/in/bhuvan-kalyan-g-v/)

## Version History
 0.1: Initial Release
