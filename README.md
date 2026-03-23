# Smart Attendance System

A cutting-edge attendance management system that combines ID card scanning and facial recognition for accurate and automated attendance tracking.

## 🚀 Features

- **Dual Authentication**: Combines ID card scanning and facial recognition for secure attendance marking
- **Real-time Processing**: Simultaneous scanning of ID cards and face recognition
- **Automated Attendance**: System automatically marks attendance when ID and face match
- **Database Integration**: SQLite database for storing student records and attendance data
- **Report Generation**: Excel report export functionality for attendance records
- **User-friendly Interface**: Simple and intuitive operation



## 🛠️ Technologies Used

- **Python 3.10+** - Core programming language
- **OpenCV** - Computer vision and image processing
- **pyzbar** - Barcode and QR code scanning
- **SQLite** - Lightweight database for data storage
- **Pandas & OpenPyXL** - Excel report generation
- **NumPy** - Numerical computing support

## 📋 System Requirements

- Windows/macOS/Linux operating system
- Python 3.10 or higher
- Webcam for ID scanning and face recognition
- ID cards with barcodes or QR codes

## 🔧 Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/sutharson20069/smart-attendance.git
   cd smart-attendance
   ```

2. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

3. **Run the system:**
   ```bash
   python main.py
   ```

## 🎯 Usage

1. **Launch the application**: Run `python main.py`
2. **Scan ID card**: Hold the ID card in front of the camera
3. **Face recognition**: Position your face in front of the camera
4. **Attendance marking**: System automatically verifies and marks attendance
5. **Report generation**: Excel reports are generated automatically

## 📂 Project Structure

```
smart-attendance/
├── database.py              # Database operations
├── face_recognition_module.py # Face recognition functionality
├── id_card_scanner.py       # ID card scanning
├── main.py                  # Main application
├── report_generator.py     # Excel report generation
├── requirements.txt         # Project dependencies
└── README.md                # Project documentation
```

## 🔍 How It Works

1. **ID Card Scanning**: Uses OpenCV and pyzbar to detect and decode barcodes/QR codes from ID cards
2. **Face Recognition**: Captures face images and uses OpenCV's LBPH algorithm for recognition
3. **Verification**: Compares ID data with recognized face to ensure match
4. **Attendance Marking**: Records attendance in SQLite database when verification succeeds
5. **Reporting**: Generates comprehensive Excel reports of attendance data

## 📊 Database Schema

### Students Table
- `id` (TEXT, PRIMARY KEY): Student ID
- `name` (TEXT): Student name
- `email` (TEXT): Student email
- `registered_at` (TIMESTAMP): Registration timestamp

### Attendance Table
- `id` (INTEGER, PRIMARY KEY): Attendance record ID
- `student_id` (TEXT): Reference to student ID
- `timestamp` (TIMESTAMP): Attendance timestamp

## 📈 Report Generation

The system automatically generates two types of reports:

1. **Complete Attendance Report**: All attendance records with student details
2. **Daily Attendance Report**: Attendance records for a specific date

Reports are saved as Excel files (`attendance_report.xlsx` and `daily_attendance.xlsx`).

## 🤝 Contributing

Contributions are welcome! Please follow these steps:

1. Fork the repository
2. Create your feature branch: `git checkout -b feature/your-feature`
3. Commit your changes: `git commit -m 'Add some feature'`
4. Push to the branch: `git push origin feature/your-feature`
5. Open a pull request

## 📜 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- OpenCV team for computer vision libraries
- pyzbar contributors for barcode scanning
- Python community for excellent documentation and support

## 📞 Contact

For questions or support, please contact:
- **GitHub**: [sutharson-k](https://github.com/sutharson-k)

---

**Smart Attendance System** - Making attendance tracking intelligent and efficient! 🚀
