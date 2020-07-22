# Extracting-information-from-PDF-files-using-OCR-and-NLP

This project demonstrates how to extract relevant information like invoice number, date, amount etc. from PDF files using OCR and NLP techniques. 

For OCR the Textract library was used with the method as "Tesseract". The advantage of using Textract instead of Google's Tesseract is that it processes PDF files directly instead of having to first convert the files to an image. It is also much faster and gives the same output as Tesseract (since the internal engine used is anyway Tesseract)

Once the text has been extracted using OCR techniques, various NLP and text parsing techniques like Regular extressions, NER, SpaCy etc. have been used to identify and extract the relevant information

There are two challenges addressed in this project
1) Identify whether a document is an invoice / engineering drawing
2) If it's an invoice extract - Invoice number, date, amount. If it's an engineering drawing extract the job ID and pipe class
    
