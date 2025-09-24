
# 🚀 File-Flow

![GitHub stars](https://img.shields.io/github/stars/venkat-0706/File-Flow?style=social)
![GitHub forks](https://img.shields.io/github/forks/venkat-0706/File-Flow?style=social)
![GitHub license](https://img.shields.io/github/license/venkat-0706/File-Flow)

**File-Flow** is a **JavaScript-based automation tool** for organizing files efficiently.  
It declutters folders, categorizes files by type, and can run anywhere using **Docker** for deployment.  

---

## 🛠️ Tech Stack

| Technology | Icon |
|------------|------|
| JavaScript | ⚡ |
| Node.js    | 🟢 |
| Docker     | 🐳 |
| FS Module  | 📂 |
| Path Module| 🛣️ |
| JSON       | 📄 |
| CLI        | 💻 |

---

## ✨ Features

- ✅ **Automatic File Sorting** – Categorize files by type  
- ✅ **Custom Folder Categories** – Tailor categories via `config.json`  
- ✅ **Cross-Platform Support** – Works on Windows, macOS, and Linux  
- ✅ **Lightweight & Fast** – Minimal dependencies, high performance  
- ✅ **Dockerized Deployment** – Run in any environment  
- ✅ **Modular Design** – Easy to extend  

---

## 📂 Project Structure

```

File-Flow/
│
├── index.js           # Main script
├── config.json        # Folder categories & extensions
├── Dockerfile         # Docker deployment setup
├── README.md          # Project documentation
├── package.json       # Node.js dependencies & scripts
├── package-lock.json  # Dependency lock file
└── utils/             # Helper modules (optional)

```

---

## ⚙️ How It Works

1. **Provide Directory Path** – Specify the folder to organize.  
2. **Read Config** – Reads `config.json` for folder types and extensions.  
3. **Sort Files** – Moves files into respective folders.  
4. **Docker Ready** – Run in a container for consistent execution.  

**Workflow Diagram (Example)**  

```

+-------------------+
\|   User Directory  |
+-------------------+
|
v
+-------------------+
\|  File-Flow Script |
\|  (index.js)       |
+-------------------+
|
v
+-------------------+
\|  Reads config.json|
+-------------------+
|
v
+-------------------+
\|   Categorizes     |
\|   & Moves Files   |
+-------------------+
|
v
+-------------------+
\| Organized Folders |
+-------------------+

````

---

## 📂 Folder Categories Example

```json
{
  "Images": [".jpg", ".jpeg", ".png", ".gif"],
  "Documents": [".pdf", ".docx", ".txt"],
  "Audio": [".mp3", ".wav"],
  "Video": [".mp4", ".mkv"]
}
````

---

## 🚀 Installation

```bash
git clone https://github.com/venkat-0706/File-Flow.git
cd File-Flow
npm install
```

---

## 💻 Usage

Run locally:

```bash
node index.js
```

* Enter the directory path with files to organize
* Files are automatically sorted as per `config.json`

---

### 🐳 Docker Deployment

Build the Docker image:

```bash
docker build -t file-flow .
```

Run the container:

```bash
docker run -v /path/to/your/files:/app/files file-flow
```

* Replace `/path/to/your/files` with your local folder path
* Files inside the mounted volume will be organized automatically

---

## 🤝 Contributing

We welcome contributions!

1. Fork the repository
2. Create a branch (`git checkout -b feature-name`)
3. Make your changes and commit (`git commit -m "Add feature"`)
4. Push the branch (`git push origin feature-name`)
5. Open a Pull Request

---

## 📜 License

This project is licensed under **MIT License** – see [LICENSE](LICENSE)

---

### 🌟 Support & Connect

If you like this project, **star ⭐ the repo** and share feedback!

