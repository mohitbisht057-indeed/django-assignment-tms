# django-assignment-tms
Research on Django themes and shopping cart repositories for TMS Foundation internship assignment.
TMS Foundation Web Development Assignment
Task 1:
Find Themes for a Django Website
1. AdminLTE
Bootstrap-based admin dashboard.
Responsive design.
Easy to integrate with Django.

Website: https://adminlte.io/

2. Material Dashboard
Modern Material Design interface.
User-friendly and responsive.

Website: https://www.creative-tim.com/product/material-dashboard

3. CoreUI
Open-source Bootstrap admin template.
Responsive and customizable.

Website: https://coreui.io/

4. Tabler
Lightweight UI framework.
Mobile responsive.

Website: https://tabler.io/

5. Django Jet
Enhanced Django admin interface.

GitHub Repository:
https://github.com/geex-arts/django-jet

Conclusion

These themes help developers build attractive and responsive Django websites efficiently.

---

# Task 2: Dockerizing Django Website

## Dockerfile

```dockerfile
FROM python:3.12

WORKDIR /app

COPY requirements.txt .

RUN pip install -r requirements.txt

COPY . .

EXPOSE 8000

CMD ["python", "manage.py", "runserver", "0.0.0.0:8000"]
