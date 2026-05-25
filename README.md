# 🌐 Distributed Monitoring System
## Big Data Architectures – Projekt 14
### Hochschule Bielefeld – Summer Term 2026

---

## 📋 Beschreibung
Ein verteiltes Monitoring-System für Website-Traffic-Daten auf Basis einer Multi-Storage-Strategie (Hot/Warm/Cold).

| Datenbank | Typ | Verwendungszweck |
|-----------|-----|-----------------|
| 🔴 Redis | Hot Data | Letzte 5 Minuten |
| 🟡 InfluxDB | Warm Data | Letzte 30 Tage |
| 🔵 Cassandra | Cold Data | Älter als 30 Tage |

---

## 🚀 Schnellstart

### 1. Repository klonen
```bash
git clone https://github.com/EUER-LINK/distributed-monitoring-system.git
cd distributed-monitoring-system
```

### 2. Docker Datenbanken starten
```bash
cd docker
docker compose up -d
```

### 3. Python Pakete installieren
```bash
cd ..
pip install -r requirements.txt
```

### 4. Kaggle Datensatz herunterladen
```bash
kaggle datasets download vishnu0399/server-logs -p datasets/ --unzip
```

### 5. Jupyter Notebook starten
```bash
jupyter notebook notebooks/dms.ipynb
```

---

## 📁 Projektstruktur
```
distributed-monitoring-system/
├── 📁 docker/
│   ├── compose.yml        → Startet alle Datenbanken
│   ├── redis/             → Redis Konfiguration
│   ├── influxdb/          → InfluxDB Konfiguration
│   └── redisinsight/      → RedisInsight Dashboard
├── 📁 datasets/           → Kaggle CSV hier reinlegen
├── 📁 notebooks/
│   └── dms.ipynb          → Jupyter Notebook (Python Code)
├── 📁 docs/               → Dokumentation
├── .gitignore
├── requirements.txt       → Python Pakete
└── README.md
```

---

## 🔗 Dashboards
- **InfluxDB:** http://localhost:8086 (admin/password)
- **RedisInsight:** http://localhost:5540

---

## 👥 Team
- Student 1
- Student 2

**Modul:** Big Data Architectures
**Professor:** Prof. Dr. Alexander Maier
