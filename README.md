# Bank Statement Processor

A modern web application that processes bank statements, extracts transaction details, and generates categorized reports. The application features a clean, minimalist UI built with React and a FastAPI backend.

## Features

- Upload bank statements in Excel format (.xls, .xlsx)
- Automatic extraction of transaction details
- Categorization of transactions
- Highlighting of deposit transactions
- Export processed data to Excel
- Modern, responsive UI
- Real-time processing feedback

## Project Structure

```
bank-statement-processor/
├── backend/               # FastAPI backend
│   ├── main.py           # Main application file
│   └── requirements.txt  # Python dependencies
└── frontend/             # React frontend
    ├── src/             # Source files
    ├── public/          # Static files
    └── package.json     # Node dependencies
```

## Prerequisites

- Python 3.8 or higher
- Node.js 16 or higher
- npm or yarn

## Backend Setup

1. Navigate to the backend directory:
   ```bash
   cd backend
   ```

2. Create a virtual environment:
   ```bash
   # Windows
   python -m venv venv
   .\venv\Scripts\activate

   # Linux/Mac
   python3 -m venv venv
   source venv/bin/activate
   ```

3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

4. Start the backend server:
   ```bash
   uvicorn main:app --reload
   ```
   The backend will be available at `http://localhost:8000`

## Frontend Setup

1. Navigate to the frontend directory:
   ```bash
   cd frontend
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Start the development server:
   ```bash
   npm run dev
   ```
   The frontend will be available at `http://localhost:5173`

## Usage

1. Open your browser and navigate to `http://localhost:5173`
2. Click "Select Excel File" to upload your bank statement
3. Click "Process File" to start processing
4. The processed file will automatically download when ready

## API Endpoints

- `POST /upload/`: Upload and process Excel file
  - Accepts: Excel file (.xls, .xlsx)
  - Returns: Processed Excel file

## Development

### Backend Development
- The backend is built with FastAPI
- CORS is enabled for local development
- File processing is done using pandas and openpyxl

### Frontend Development
- Built with React and TypeScript
- Uses Material-UI for components
- Implements modern React practices with hooks

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the LICENSE file for details. 