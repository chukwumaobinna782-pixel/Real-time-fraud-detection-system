# Real-Time Fraud Detection System

**XGBoost + FastAPI + Docker** — Production-ready credit card fraud detection with live simulation

![demo gif or screenshot]

## Performance
- ROC-AUC: **0.99942**  
- Fraud detection recall: **94%+** at 0.1% false positive rate  
- Inference latency: **< 1ms** (p95)  
- Throughput: 2000+ transactions/sec (single container)

## Quick Start (2 commands)

```bash
# 1. Start the API
docker build -t fraud-api .
docker run -p 8000:8000 fraud-api

# 2. In another terminal — start live transaction stream
python simulation/simulate_transactions.py