# Resume_parser
This project automates resume parsing using Google's Gemini AI. It extracts key details (name, contact, skills, experience) from PDFs with PyPDF2. Batch processing via concurrent.futures.ThreadPoolExecutor ensures efficiency. The structured data is saved in an Excel file, streamlining HR’s recruitment process.
Key Features:
PDF Resume Parsing: The program utilizes the PyPDF2 library to extract text from PDF resumes, making it compatible with non-editable resume formats and enabling efficient text extraction.

Generative AI Integration: By using the Gemini-1.5-Flash model, the AI intelligently processes the extracted text to identify and extract critical information, such as:

Name
Contact details (phone number)
University and course details
Key Skills
Generative AI and AI/ML experience scores
Supporting Information (certifications, internships, projects).
Batch Processing: To optimize performance, the project incorporates multi-threaded batch processing via Python’s concurrent.futures.ThreadPoolExecutor. This allows multiple resumes to be processed simultaneously, reducing extraction time and enhancing scalability when handling large datasets.

Data Export: After parsing, the structured data is exported into an Excel file (resumes_output.xlsx). This file can be used for further analysis, reporting, or integration into applicant tracking systems (ATS).
