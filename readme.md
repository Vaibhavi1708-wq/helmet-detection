# Helmet Detection and Traffic Violation System

## Project Overview
An automated system that detects and processes traffic violations, specifically focusing on motorcycle riders not wearing helmets. The system uses computer vision and machine learning to analyze video footage, detect violations, generate challans (tickets), and automatically notify violators via email.

## Key Features
- *Real-time Detection*: Processes both recorded videos and live camera feeds
- *Automated Violation Processing*: 
  - Detects motorcycles and riders
  - Checks for helmet usage
  - Captures license plate information
  - Records violation details with timestamps
- *Smart Notification System*:
  - Generates digital challans (tickets) in PDF format
  - Sends automated email notifications to violators
  - Includes violation evidence (images) in notifications
- *Administrative Dashboard*:
  - View and manage violation records
  - Generate violation reports
  - Access violation statistics and analytics

## Technology Stack
- *Frontend*: HTML, CSS, JavaScript
- *Backend*: FastAPI (Python)
- *Machine Learning*: 
  - YOLOv8 for object detection
  - EasyOCR for license plate recognition
- *Database*: CSV-based storage system
- *Email Service*: SMTP with Gmail

## System Requirements
- Python 3.8 or higher
- CUDA-compatible GPU (recommended for better performance)
- Minimum 8GB RAM
- Webcam (for live detection)

## Installation
1. Clone the repository:
bash
git clone https://github.com/yourusername/helmet-detection-system.git
cd helmet-detection-system


2. Create and activate virtual environment:
bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate


3. Install required packages:
bash
pip install -r requirements.txt


4. Configure email settings:
   - Update email_service.py with your SMTP credentials
   - Set up environment variables for email configuration

5. Start the application:
bash
python backend/main.py


## Project Structure
helmet-detection-system/
├── backend/
│ ├── detection.py # ML model implementation
│ ├── database.py # Data storage operations
│ ├── email_service.py # Email notification system
│ ├── main.py # FastAPI application
│ └── pdf.py # Challan generation
├── frontend/
│ ├── index.html
│ ├── style.css
│ └── script.js
├── models/ # ML model files
├── violations/ # Violation images
├── challans/ # Generated PDFs
└── requirements.txt

## Usage
1. Access the web interface at http://localhost:8000
2. Upload a video file or start live stream
3. System automatically detects violations
4. View detected violations in the dashboard
5. Generate and send challans to violators

## Features in Detail
1. *Video Processing*
   - Supports multiple video formats
   - Real-time processing capabilities
   - Frame-by-frame analysis

2. *Violation Detection*
   - Motorcycle detection
   - Rider identification
   - Helmet presence verification
   - License plate recognition

3. *Violation Management*
   - Automatic record creation
   - Image evidence storage
   - PDF challan generation
   - Email notification system

4. *Security Features*
   - Secure file handling
   - Email verification
   - Data validation
   - Error handling

## Contributing
Contributions are welcome! Please feel free to submit a Pull Request.

## License
This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgments
- YOLOv8n for object detection
- EasyOCR for text recognition
- FastAPI for backend framework
- Contributors and maintainers

## Contact
For any queries or support, please contact:
- Email: vaibhaviingole24@gmail.com
- GitHub: [Your GitHub Profile](https://github.com/Vaibhavi1708-wq)