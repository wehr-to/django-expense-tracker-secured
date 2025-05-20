django-expense-tracker-secured

## 🎯 Learning Goals

- Build a Django app that handles user-generated financial data
- Visualize expenses over time using Chart.js or Matplotlib
- Prevent injection and data exposure vulnerabilities
- Implement secure export and optional data protection

## 🔐 Security Focus

This project includes mitigations for:

- ❌ Injection via input fields  
- ❌ Exposure of another user’s data  
- ❌ Unencrypted storage of sensitive values  
- ✅ Audit log of key actions (add, delete, export)

See [`audit-checklist.md`](./audit-checklist.md) for details.

## ✅ Core Features

- User registration and login
- Add, edit, and delete expenses
- View monthly expense summaries via chart
- Filter expenses by category/date
- Export data to CSV (secure path only)
- Optional: mock data encryption or obfuscation

## 🚀 Getting Started

```bash
git clone https://github.com/yourusername/django-expense-tracker-secured.git
cd django-expense-tracker-secured
python -m venv venv
source venv/bin/activate  # Windows: venv\Scripts\activate
pip install -r requirements.txt
python manage.py migrate
python manage.py runserver

🧪 Optional Enhancements
Add category-based filtering
Add CSV export with user ownership enforcement
Use AES or Fernet mock encryption for stored amounts
Add pagination and summary statistics
