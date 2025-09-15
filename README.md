# 🎓 Workshop Booking – UI/UX Enhanced Version

[![Made with Django](https://img.shields.io/badge/Made%20with-Django-092E20?style=for-the-badge&logo=django)](https://www.djangoproject.com/)  
[![Bootstrap](https://img.shields.io/badge/Bootstrap-5-7952B3?style=for-the-badge&logo=bootstrap)](https://getbootstrap.com/)
[![GSAP](https://img.shields.io/badge/GSAP-3F3F85?style=for-the-badge&logo=greensock)](https://greensock.com/gsap/)
[![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5)](https://developer.mozilla.org/en-US/docs/Web/HTML)
[![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3)](https://developer.mozilla.org/en-US/docs/Web/CSS)
[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)



---

## ✨ Overview

This is an enhanced version of the [FOSSEE Workshop Booking system](https://github.com/FOSSEE/workshop_booking).  
The project was redesigned with **improved UI/UX** to make it more modern, mobile-friendly, and user-focused.  

Key Highlights:
- 🔄 **Upgraded from Bootstrap 4 → Bootstrap 5**
- 📱 Optimized for **mobile-first usage** (students often access via phones)
- 🎨 Enhanced **forms, navigation, and layout**
- ⚡ Maintained **fast load times** and accessibility

---

## 🚀 Quick Setup Guide

> ⚠️ **Important:** Use **Python3** and Keep the **exact Django version** mentioned in `requirements.txt`.  
> Upgrading Django may cause errors.

```bash
# 1️⃣ Clone the repository
git clone https://github.com/Bishal-NITS-2003/workshop_booking.git
cd workshop_booking

# 2️⃣ Create a virtual environment and install dependencies
pip install -r requirements.txt

# 3️⃣ Run migrations
python manage.py makemigrations
python manage.py migrate

# (If errors occur for cms_table/teams_table, run migrations manually)
python manage.py makemigrations cms
python manage.py migrate
python manage.py makemigrations teams
python manage.py migrate

# 4️⃣ Create superuser
python manage.py createsuperuser

# 5️⃣ Start server
python manage.py runserver
````

Now, open: **[http://127.0.0.1:8000/](http://127.0.0.1:8000/)** 🎉

---

## 🔑 User Roles & Access

<details>
<summary><b>👑 Superuser</b></summary>

* Login with superuser credentials.
* Create a group `"instructor"` and assign all permissions.
* Add selected users to `"instructor"` group.
* Update their profile positions accordingly.

</details>

<details>
<summary><b>📌 Coordinator</b></summary>

* Registers via `/workshop/register/`.
* Completes account activation via activation link through email/terminal.
* Logs in via `/workshop/login/`.
* View statistics under **Statistics → Workshop Statistics**
* Can propose workshops via **Workshops → Propose a Workshop**.

</details>

<details>
<summary><b>👨‍🏫 Instructor</b></summary>

* Create workshops via **Create Workshop** tab.
* View statistics under **Statistics → Workshop Statistics**.
* Post comments on coordinator profiles.

</details>

---

## 🖼️ Screenshots of Enhancement

<details>
  <summary>Login Page</summary>
  
  | Before | After |
  | ------ | ----- |
  | ![Before login](Screenshots/Login-Form/old.png) | ![After login](Screenshots/Login-Form/new.png) |
</details>

<details>
  <summary>Reset Password</summary>
  
  | Before | After |
  | ------ | ----- |
  | ![Before login](Screenshots/Reset-Password/old.png) | ![After login](Screenshots/Reset-Password/new.png) |
</details>

<details>
  <summary>Registraion Page</summary>
  
  | Before | After |
  | ------ | ----- |
  | ![Before login](Screenshots/Registration-form/old.png) | ![After login](Screenshots/Registration-form/new.png) |
</details>

<details>
  <summary>Navbar</summary>
  
  | Before | After |
  | ------ | ----- |
  | ![Before login](Screenshots/Navbar/old.png) | ![After login](Screenshots/Navbar/new.png) |
</details>

<details>
  <summary>Coordinator Status Page</summary>
  
  | Before | After |
  | ------ | ----- |
  | ![Before login](Screenshots/Coordinator-Page/old.png) | ![After login](Screenshots/Coordinator-Page/new.png) |
</details>

<details>
  <summary>Workshop-Statistics Page</summary>
  
  | Before | After |
  | ------ | ----- |
  | ![Before login](Screenshots/Workshop-Statistics/old.png) | ![After login](Screenshots/Workshop-Statistics/new.png) |
</details>

<details>
  <summary>Instructor Status Page</summary>
  
  | Before | After |
  | ------ | ----- |
  | ![Before login](Screenshots/Instructor-Status-Page/old.png) | ![After login](Screenshots/Instructor-Status-Page/new.png) |
</details>

<details>
  <summary>Propose Workshop Page</summary>
  
  | Before | After |
  | ------ | ----- |
  | ![Before login](Screenshots/Propose-Workshop/old.png) | ![After login](Screenshots/Propose-Workshop/new.png) |
</details>


<details>
  <summary>View And Edit Workshop Page</summary>
  
  | Before | After |
  | ------ | ----- |
  | ![Before login](Screenshots/View-And-Edit-Workshop-Page/old.png) | ![After login](Screenshots/View-And-Edit-Workshop-Page/new.png) |
</details>


<details>
  <summary>View Profile Page</summary>
  
  | Before | After |
  | ------ | ----- |
  | ![Before login](Screenshots/View-Profile/old.png) | ![After login](Screenshots/View-Profile/new.png) |
</details>


<details>
  <summary>Workshop Details Page</summary>
  
  | Before | After |
  | ------ | ----- |
  | ![Before login](Screenshots/Workshop-Details/old.png) | ![After login](Screenshots/Workshop-Details/new.png) |
</details>


<details>
  <summary>Workshop Type Details Page</summary>
  
  | Before | After |
  | ------ | ----- |
  | ![Before login](Screenshots/Workshop-Type-Details/old.png) | ![After login](Screenshots/Workshop-Type-Details/new.png) |
</details>


<details>
  <summary>Workshop Types List Page</summary>
  
  | Before | After |
  | ------ | ----- |
  | ![Before login](Screenshots/Workshop-Types-List/old.png) | ![After login](Screenshots/Workshop-Types-List/new.png) |
</details>

<details>
  <summary>Team Statistics Page</summary>
  
  | Before | After |
  | ------ | ----- |
  | ![Before login](Screenshots/Team-Statistics/old.png) | ![After login](Screenshots/Team-Statistics/new.png) |
</details>

---

## 🎨 Design Reasoning

### 1️⃣ Design Principles

* **Mobile-first** 📱 → Collapsible navbar, larger tap targets.
* **Consistency** 🎨 → Unified typography, spacing, and color.
* **Clarity** ✍️ → Headings, card layouts, and alerts for feedback.
* **Accessibility** ♿ → High contrast, semantic HTML, ARIA roles.

### 2️⃣ Responsiveness

* Used **Bootstrap 5 grid system** for flexible layouts.
* Used **Media Queries** wherever required.
* Used **Custom CSS Scripts** too for better design and layout control.
* Forms and tables scale smoothly on all devices.
* Navbar collapses into a hamburger menu on small screens.

### 3️⃣ Trade-offs

* ✅ Chose **Bootstrap 5** → modern design.
* ✅ Kept **Django version fixed** (from `requirements.txt`) → avoids backend errors.
* ✅ Avoided heavy JS libraries → fast page loads.

### 4️⃣ Challenges

* Refactoring Bootstrap classes as the Bootstrap version is updated.
* Maintaining balance between **performance** and **UI richness**.
* Ensuring design consistency across roles (**Coordinator, Instructor, Admin**).
* Fixing a bug that was giving error for auto redirection to admin panel for superuser when logged in. Fixed in commit **25b1bf0**.
* Django auto-generated form fields for file attachments were not displaying as intended. Fixed by customizing form rendering logic and ensuring empty file inputs show correctly for new uploads. Fixed in commit **c637582**
---

## ✅ Conclusion

This enhanced version of the **Workshop Booking System** focuses on making the platform more **modern, responsive, and user-friendly**, while keeping the **core Django structure and functionality intact**.  

Overall, this redesign improves **accessibility, usability, and scalability**, ensuring the system is well-suited for real-world academic use.  

> 📝 This project was developed as part of the **Python Screening Task 1: UI/UX Enhancement** for FOSSEE Semester Long Internship - Autumn 2025