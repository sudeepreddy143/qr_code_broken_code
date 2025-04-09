# QR Code REST API

![FastAPI](https://img.shields.io/badge/FastAPI-005571?style=for-the-badge&logo=fastapi)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=for-the-badge&logo=github-actions&logoColor=white)

A robust REST API solution for creating, retrieving, and managing QR codes. Built with FastAPI for high performance and modern features.

## 🌟 Key Features

- **Create QR Codes**: Generate and store QR codes locally
- **Retrieve QR Codes**: Access your saved QR codes anytime
- **Delete QR Codes**: Remove unwanted QR codes from storage
- **Interactive Documentation**: Auto-generated Swagger UI at `/docs`
- **Secure Access**: Basic authentication protection

## 📋 Requirements

- Python 3.8+
- Docker (optional)
- Internet connection (for dependencies)

## 🚀 Quick Start

### Option 1: Run Locally

1. **Clone the repository**
   ```bash
   git clone https://github.com/your-username/fastapi-qr-api.git
   cd fastapi-qr-api
   ```

2. **Set up virtual environment**
   ```bash
   python -m venv venv
   source venv/bin/activate  # Windows: venv\Scripts\activate
   ```

3. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

4. **Create storage directory**
   ```bash
   mkdir qr_codes
   ```

5. **Start the server**
   ```bash
   uvicorn app.main:app --reload
   ```

### Option 2: Using Docker

```bash
docker compose up --build
```

🌐 Access the API at [http://localhost/docs](http://localhost/docs)

## 🔒 Authentication

The API is protected with basic authentication:

- **Username**: `admin`
- **Password**: `secret`

To authenticate via the Swagger UI, click the "Authorize" button at the top.



## 🧪 Testing

Run the test suite to verify functionality:

```bash
pytest
```

All tests should pass, confirming the API is working correctly.

## 🛠️ Development

The project structure is organized as follows:

```
fastapi-qr-api/
├── app/
│   ├── main.py         # Main application entry point
│   ├── routers/        # API route definitions
│   └── services/       # Business logic
├── tests/              # Test suite
├── qr_codes/           # QR code storage directory
├── Dockerfile          # Container definition
├── docker-compose.yml  # Multi-container setup
└── requirements.txt    # Python dependencies
```

## 📝 License

This project is licensed under the MIT License - see the LICENSE file for details.
