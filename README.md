# Eco-Ideathon  
## AI-Powered Rooftop Solar PV Detection & Area Estimation

This project implements an end-to-end **AI-based verification pipeline** for detecting rooftop solar photovoltaic (PV) installations using satellite imagery.  
It was developed for **EcoInnovators Ideathon 2026** under the theme of governance-ready solar verification.

---

## Problem Statement

Government solar subsidy programs require **reliable, scalable verification** of rooftop solar installations.  
Manual inspections are slow, expensive, and inconsistent.

This system answers:

> **Given a latitude and longitude, is a rooftop solar PV system installed at that location?**

If present, the system estimates the **total PV panel area** and generates **audit-friendly evidence**.

---

## Core Capabilities

- Satellite image retrieval using **Google Static Maps API**
- Solar panel detection using **YOLO segmentation**
- Buffer-based verification logic:
  - **1200 sq.ft** primary buffer
  - **2400 sq.ft** fallback buffer
- Selection of the panel with **maximum overlap** inside the buffer
- Estimation of:
  - PV area (m²)
  - Panel count
  - Capacity (kW)
  - Euclidean Distance Verification
- Quality Control (QC) classification:
- Explainable outputs with polygon masks and audit overlays
