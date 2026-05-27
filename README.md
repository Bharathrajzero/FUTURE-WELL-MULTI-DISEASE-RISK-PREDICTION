# FUTURE WELL: MULTI DISEASE RISK PREDICTION

**Future Well** is an intelligent, high-performance web portal built using the Streamlit framework. It serves as an enterprise entry point featuring secure multi-tier user classification paths. The portal intercepts user login packets, writes structural audit trails via a JSON tracking engine, and dynamically switches execution panels depending on administrative, clinical, or client privilege vectors.

---

## ⚡ Core Platform Features

* **Dynamic Role-Based Access Control (RBAC):** Integrates an automated login UI state manager that queries session vectors and cleanly mounts distinct interfaces:
* **Administrative Dashboard (`admin`):** Global cluster controls and system monitoring.
* **Clinical Console (`doctor`):** Specialized operational viewports and patient triage tracking.
* **Client Portal (`user`):** Tailored self-service metric interfaces.


* **Modern High-Contrast Interface Design:** Custom injection of Google Fonts styling elements alongside dynamic CSS animations, featuring a specialized glowing neural brand asset tracking engine.
* **Persistent Session Isolation Engine:** Completely flushes residual unencrypted browser memory frames and authorization keys on application boot sequence to prevent state leakage between separate sessions.
* **Automated Audit Telemetry:** Integrates directly with a backend logging pipeline to record access events systematically into persistent structures.

---

## 🛠️ System Technology Stack

* **Core Engine:** Streamlit Web Framework
* **Identity Management:** Custom authenticated login UI widget framework with remote token mappings (`courier_auth_token`)
* **Graphics Processing:** Pillow (PIL) binary rendering pipeline
* **Design Systems:** Base64 asset injection pipelines, custom CSS injection, Google Fonts API

---

## 📂 Project Directory Structure

```text
├── app.py                      # Main orchestration gateway entry point
├── logger.py                   # Async telemetry logging engine
├── background1.jpg             # Sidebar graphical background configuration
├── background7.jpg             # High-contrast core workspace background asset
├── logo3.png                   # High-resolution neural glow asset
└── Login/                      # Multi-tier compartmentalized dashboard views
    ├── admin_dashboard.py      # Administrative operations module
    ├── doc.py                  # Clinical operational viewports
    └── user_dashboard.py       # Client metric tracking panel

```

---

## 🚀 Local Initialization and Setup

### Prerequisites

* Ensure a stable deployment of Python 3.9 or higher is active within your isolated virtual execution domain.

### 1. Provision Environment Dependencies

Install the required architectural packages into your isolated runtime space:

```bash
pip install streamlit pillow streamlit-login-auth-ui

```

### 2. Verify Asset Placement

Confirm that all core identity visual elements (`background1.jpg`, `background7.jpg`, and `logo3.png`) are located precisely inside the repository root directory before initializing the runtime engine.

### 3. Launch the Application Node

Execute the Streamlit server mapping locally:

```bash
streamlit run app.py

```

Upon successful internal server binding, access the application locally via your secure loopback address: **`http://localhost:8501`**

---

## ⚙️ Structural Code Overview

### Streamlit Tab Layout Fluidity & Mask Overrides

To preserve design consistency across modern web rendering engines, standard fade masks built into the Streamlit tab array components are systematically stripped via explicitly targeted CSS overrides:

```css
/* Removes structural visual fade styling masks built into default Streamlit containers */
div[data-testid="stTabs"] > div {
    -webkit-mask-image: none !important;
    mask-image: none !important;
}
div[data-testid="stTabs"]::after {
    display: none !important;
}

```

### Event Routing & Privilege Escalation Engine

User structural records are audited securely at login, matching role tags cleanly to prevent unauthorized operations:

```python
if LOGGED_IN:
    username = st.session_state.get("USERNAME", "guest")
    role = st.session_state.get("ROLE", "user")

    # Pass credential elements directly into the security logging pipeline
    log_login_event_json(username, role)

    # Dynamic UI redirection sequence
    if role == "admin":
        show_admin_dashboard(username)
    elif role == "doctor":
        show_doc_dashboard(username)
    else:
        show_user_dashboard(username)

```

---

## 📝 Compliance & Attribution

* **Distribution Engine:** Internal Proprietary Platform.
* **System Operations Framework:** Engineered and Maintained by **AlphaGroupLtd** © 2025.
