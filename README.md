📄 README.md

# 🛠️ Cloudmen Odoo Scaffold CLI

A command-line tool to quickly scaffold Odoo custom modules without manually creating folder structures and base files.

---

## 🚀 Quick Setup

### 1. Clone the script

```bash
git clone https://github.com/cloudmen/scafcloudmen.git
cd scafcloudmen
chmod +x scafcloudmen

2. Make it globally accessible

sudo mv scafcloudmen /usr/local/bin/

3. Add the default icon (if no custom icon is provided)

sudo mkdir -p /usr/local/bin/static/src/img
sudo cp icon.png /usr/local/bin/static/src/img/icon.png

✅ How to Use

Run this from any terminal:

scafcloudmen

The tool will ask you the following:

    📦 Module name

    📁 Absolute path to create the module (e.g. /home/yourname/odoo18/custom_addons)

    🔥 Odoo version

    📂 Which folders you want (models, views, controllers, reports, demo, security)

    📝 Module title, summary, long description, category

    📷 Icon path (or it will use the default one automatically)

📁 What’s Generated

Depending on your choices, the tool generates a structure like:

your_module/
├── __init__.py
├── __manifest__.py
├── controllers/
│   ├── __init__.py
│   └── controllers.py
├── models/
│   ├── __init__.py
│   └── models.py
├── views/
│   └── views.xml
├── reports/
│   └── custom_report.xml
├── demo/
│   └── demo.xml
├── security/
│   └── ir.model.access.csv
└── static/
    └── src/
        └── img/
            └── icon.png

⚠️ Notes

    You must use sudo to move the script to /usr/local/bin/ for global access

    The icon file is optional — if you don’t provide one, the script uses:

    /usr/local/bin/static/src/img/icon.png

👨‍💻 Built by Cloudmen

    Made with ❤️ by Cloudmen Odoo Engineers
