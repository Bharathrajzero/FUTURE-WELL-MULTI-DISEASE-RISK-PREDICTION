# FUTURE WELL: MULTI‑DISEASE RISK PREDICTION

**Future Well** is an intelligent, high‑performance web portal built using the Streamlit framework. It serves as an enterprise entry point featuring secure multi‑tier user classification paths. The portal intercepts user login packets, writes structural audit trails via a JSON tracking engine, and dynamically switches execution panels depending on administrative, clinical, or client privilege vectors.

---

## ⚡ Core Platform Features
- **Dynamic Role‑Based Access Control (RBAC):** Automated login UI state manager that queries session vectors and mounts distinct interfaces:
  - **Administrative Dashboard (`admin`)** – Global cluster controls and system monitoring.
  - **Clinical Console (`doctor`)** – Specialized operational viewports and patient triage tracking.
  - **Client Portal (`user`)** – Tailored self‑service metric interfaces.
- **Modern High‑Contrast Interface Design:** Custom Google Fonts styling with dynamic CSS animations and glowing neural brand asset tracking.
- **Persistent Session Isolation Engine:** Flushes residual unencrypted browser memory frames and authorization keys on boot to prevent state leakage.
- **Automated Audit Telemetry:** Backend logging pipeline records access events systematically into persistent structures.

---

## 🛠️ System Technology Stack
- **Core Engine:** Streamlit Web Framework  
- **Identity Management:** Custom authenticated login UI widget framework with remote token mappings (`courier_auth_token`)  
- **Graphics Processing:** Pillow (PIL) binary rendering pipeline  
- **Design Systems:** Base64 asset injection pipelines, custom CSS injection, Google Fonts API  

---

## 📂 Project Directory Structure
```text
├── app.py                      # Main orchestration gateway entry point
├── logger.py                   # Async telemetry logging engine
├── background1.jpg              # Sidebar graphical background configuration
├── background7.jpg              # High‑contrast core workspace background asset
├── logo3.png                    # High‑resolution neural glow asset
└── Login/                       # Multi‑tier compartmentalized dashboard views
    ├── admin_dashboard.py       # Administrative operations module
    ├── doc.py                   # Clinical operational viewports
    └── user_dashboard.py        # Client metric tracking panel
```

---

## 🚀 Local Initialization and Setup

### Prerequisites
- Python 3.9 or higher installed in an isolated virtual environment.

### 1. Install Dependencies
```bash
pip install streamlit pillow streamlit-login-auth-ui
```

### 2. Verify Asset Placement
Ensure `background1.jpg`, `background7.jpg`, and `logo3.png` are located in the repository root directory.

### 3. Launch the Application
```bash
streamlit run app.py
```
Access locally via: **http://localhost:8501**

---

## ⚙️ Structural Code Overview

### Streamlit Tab Layout Overrides
```css
/* Removes fade styling masks in default Streamlit containers */
div[data-testid="stTabs"] > div {
    -webkit-mask-image: none !important;
    mask-image: none !important;
}
div[data-testid="stTabs"]::after {
    display: none !important;
}
```

### Event Routing & Privilege Escalation
```python
if LOGGED_IN:
    username = st.session_state.get("USERNAME", "guest")
    role = st.session_state.get("ROLE", "user")

    log_login_event_json(username, role)

    if role == "admin":
        show_admin_dashboard(username)
    elif role == "doctor":
        show_doc_dashboard(username)
    else:
        show_user_dashboard(username)
```

---

## 📖 Usage
- Log in with your assigned role (`admin`, `doctor`, or `user`).  
- Explore dashboards tailored to your privilege level.  
- Track audit logs and verify session isolation.  
- Customize UI themes with provided background assets.  

---

## 🤝 Contributing
Contributions are welcome!  
- Fork the repository  
- Create a new branch  
- Submit a pull request  

For major changes, open an issue first to discuss what you’d like to change.

---

## 👨‍💻 Author
**Bharath Raj**  
GitHub: [Bharathrajzero](https://github.com/Bharathrajzero)

---

## 📝 Compliance & Attribution
- **Distribution Engine:** Internal Proprietary Platform  
- **System Operations Framework:** Engineered and Maintained by **AlphaGroup Ltd** © 2025  

---

## 📜 License
This project is licensed under the MIT License © 2026 Bharath Raj, AlphaGroup Ltd.  
See the `[Looks like the result wasn't safe to show. Let's switch things up and try something else!]` file for details.

---
