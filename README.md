# 🖼️🔍 TextSnap Microservice

**TextSnap Microservice** is a lightweight, high-performance Python-based microservice powered by **FastAPI**, designed for accurate and efficient text extraction from images using Optical Character Recognition (OCR). It supports a variety of image formats including **PNG**, **JPEG**, and **JPG**, making it ideal for modern applications needing text recognition.

---

## ✨ Features

* **🔎 High Accuracy**: Achieves up to **95% accuracy** in text extraction for clear and structured images.
* **🖼️ Format Support**: Works seamlessly with commonly used image formats like PNG, JPG, and JPEG.
* **⚙️ Simple Integration**: Accepts HTTP `POST` requests with image uploads—easy to plug into any system.
* **💡 Open Source**: Fully open-source and customizable for your own use case or extension.

---

## 🚀 Getting Started

Follow these steps to set up and run **TextSnap Microservice** locally:

### 1. Clone the Repository

```bash
git clone https://github.com/Ramkrushna-Sahu/TextSnap-Microservice.git
```

### 2. Install Dependencies

```bash
cd TextSnap-Microservice
pip install -r requirements.txt
```

### 3. Start the Server

```bash
uvicorn main:app --reload
```

### 4. Send an Image for OCR

Use `curl` or Postman to send a POST request:

```bash
curl -X POST -F "image=@/path/to/your/image.jpg" http://localhost:8000/
```

### 5. Get OCR Output

You’ll receive the extracted text in JSON format:

```json
{
  "text": "Lorem ipsum dolor sit amet, consectetur adipiscing elit..."
}
```

---

## 🌍 Deployment Options

Though the microservice is not deployed yet, it can be easily hosted on platforms like:

* Docker
* Kubernetes
* Render / Railway / Vercel (with minor tweaks)
* Traditional VPS or cloud services (AWS, GCP, Azure)

---

## 🤝 Contributing

Want to contribute? Fork the repo, improve the code, fix bugs, or add new features — then submit a pull request!

---

## 📝 License

Licensed under the **MIT License**. See the [LICENSE](LICENSE) file for more details.
