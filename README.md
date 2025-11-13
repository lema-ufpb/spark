# ✨ Apache Spark - LEMA-UFPB

This project builds a custom Apache Spark Docker Image for various projects at LEMA-UFPB research lab. It is based on the official Apache Spark image and includes Python 3.11 configured as the default interpreter.

## 📋 Overview

This custom Spark implementation provides a containerized environment for distributed data processing and large-scale analytics at LEMA-UFPB laboratory.

## ✨ Features

- 🐳 Based on official `apache/spark:4.0.1` image
- 🐍 Python 3.11 configured as default interpreter
- ⚡ PySpark 4.0.1 integrated
- 🔧 Optimized configurations for LEMA-UFPB needs
- 📦 Production-ready containerized deployment
- 🚀 Simplified setup process

## 🛠️ Prerequisites

- Docker
- Docker Compose (optional, for multi-container environments)

## 📦 Building the Image

```bash
docker build -t spark-test .
```

## 🚀 Quick Start

### Start Interactive PySpark Shell

```bash
docker run -it spark-test /opt/spark/bin/pyspark
```

### Run Spark Shell (Scala)

```bash
docker run -it spark-test /opt/spark/bin/spark-shell
```

### Submit a Spark Application

```bash
docker run -it spark-test /opt/spark/bin/spark-submit \
  --master local[*] \
  /path/to/your/application.py
```

### Using Docker Compose

```bash
docker compose up -d
```

## 🚀 Deployment and Versioning

```bash
# Commit your changes
git add .
git commit -m "feat: description of change"

# Push to repository
git push origin main

# Create and publish version tag
git tag v4.0.1-python3.11
git push --tags
```

### 📌 Versioning Convention

We follow the pattern: `vX.Y.Z-pythonA.B`

- `X.Y.Z`: Apache Spark version
- `A.B`: Python version

Example: `v4.0.1-python3.11`

## 🤝 Contributing

Contributions are welcome! Follow these steps:

1. 🍴 Fork the repository
2. 🌿 Create your feature branch (`git checkout -b feature/MyFeature`)
3. 💾 Commit your changes (`git commit -m 'feat: Add MyFeature'`)
4. 📤 Push to the branch (`git push origin feature/MyFeature`)
5. 🔀 Open a Pull Request

### 📋 Commit Pattern

We use [Conventional Commits](https://www.conventionalcommits.org/):

- `feat:` New feature
- `fix:` Bug fix
- `docs:` Documentation changes
- `chore:` Maintenance tasks
- `refactor:` Code refactoring

## 📞 Support

For support and questions, contact LEMA-UFPB laboratory:

- 🌐 Website: [LEMA-UFPB](https://lema.ufpb.br)
- 💬 Issues: Use the [Issues](../../issues) tab of this repository
- 📖 Spark Docs: [Official Documentation](https://spark.apache.org/docs/latest/)

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

<div align="center">

[![LEMA-UFPB](https://img.shields.io/badge/LEMA-UFPB-blue)](https://lema.ufpb.br)
[![Spark](https://img.shields.io/badge/Spark-4.0.1-orange)](https://spark.apache.org/)
[![Python](https://img.shields.io/badge/Python-3.11-blue)](https://www.python.org/)
[![Docker](https://img.shields.io/badge/Docker-Ready-brightgreen)](https://www.docker.com/)

</div>
