# CC LAB 2 – Monolithic Architecture

**SRN:** PES1UG23AM359

## Description
This repository contains the implementation of CC Lab 2 demonstrating a monolithic FastAPI application.

The lab demonstrates:
- Setup and execution of a monolithic application
- Observing monolithic failure
- Bug fixing
- Load testing using Locust
- Performance optimization of routes

## Optimizations Performed

### /checkout
- Removed inefficient loop-based fee calculation
- Improved average response time

### /events
- Removed unnecessary CPU-intensive loop
- Reduced response time significantly

### /my-events
- Removed artificial computation loop
- Improved route performance

## How to Run
```bash
python -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
python insert_events.py
uvicorn main:app --reload
