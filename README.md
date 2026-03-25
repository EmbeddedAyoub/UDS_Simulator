# UDS Simulator — Automotive Diagnostic Tool

A lightweight UDS (Unified Diagnostic Services) simulator built in Python to emulate communication between a diagnostic tester and an ECU — without requiring CAN hardware.

This project is designed for embedded systems, automotive diagnostics, and cybersecurity learning, with a focus on realistic behavior and strict protocol handling.
---
# Features

UDS protocol simulation (ISO 14229)
ECU + Tester architecture
PyQt5 graphical interface
DID-based data system (JSON)
Role-based access control (Admin / Technician / Reader)
Real-time trace/log viewer
Accurate Negative Response handling (NRC)
Strict validation of request length and format
---
# Supported Services

Service	Name
0x10	Diagnostic Session Control
0x11	ECU Reset
0x22	Read Data By Identifier
0x27	Seccurity Accesses
---
# How It Works

The simulator mimics real ECU communication:

Tester (Client)  →  ECU Simulator  →  Response
Communication is direct (no CAN hardware)
Messages follow UDS Single Frame format (8 bytes)
Payload is validated before processing
---
# Loging by this JSON data

[text](DIDs/users.json)