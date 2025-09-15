# Workshop Booking – UI/UX Enhanced Version

[![Django](https://img.shields.io/badge/Made%20with-Django-092E20?style=for-the-badge&logo=django)](https://www.djangoproject.com/)  
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
- ⚡ **Balanced performance with richer UI/UX** — slight trade-off in speed for smoother animations powered by GSAP
- ♿ Continued **focus on accessibility and usability**



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
<summary><b>Superuser</b></summary>

* Login with superuser credentials.
* Create a group `"instructor"` and assign all permissions.
* Add selected users to `"instructor"` group.
* Update their profile positions accordingly.

</details>

<details>
<summary><b> Coordinator</b></summary>

* Registers via `/workshop/register/`.
* Completes account activation via activation link through email/terminal.
* Logs in via `/workshop/login/`.
* View statistics under **Statistics → Workshop Statistics**
* Can propose workshops via **Workshops → Propose a Workshop**.

</details>

<details>
<summary><b> Instructor</b></summary>

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
  | ![Before login](screenshots/login/old/old.png) | ![After login 1](screenshots/login/new/Screenshot%202025-09-16%20015104.png)<br>![After login 2](screenshots/login/new/Screenshot%202025-09-16%20015150.png) |
</details>

<details>
  <summary>Forgot Password</summary>
  
  | Before | After |
  | ------ | ----- |
  | ![Before login](screenshots/forgot_password/new/Screenshot%202025-09-16%20020008.png) | ![After login 1](screenshots/forgot_password/new/Screenshot%202025-09-16%20020028.png)<br>![After login 2](screenshots/forgot_password/new/Screenshot%202025-09-16%20020008.png) |
</details>

<details>
  <summary>Registration</summary>
  
  | Before | After |
  | ------ | ----- |
  | ![Before login](screenshots/registration/old/old.png) | ![After login 1](screenshots/registration/new/Screenshot%202025-09-16%20020655.png)<br>![After login 2](screenshots/registration/new/Screenshot%202025-09-16%20020746.png) |
</details>

<details>
  <summary>Change Password</summary>
  
  | Before | After |
  | ------ | ----- |
  | ![Before login](screenshots/change_password/old/old.png) |![After login 1](screenshots/change_password/new/Screenshot%202025-09-16%20021303.png)<br>![After login 2](screenshots/change_password/new/Screenshot%202025-09-16%20021324.png) |
</details>



<details>
  <summary>Navbar</summary>
  
  | Before | After |
  | ------ | ----- |
  | ![Before login](screenshots/navbar/old/old.png) | ![After login](screenshots/navbar/new/Screenshot%202025-09-16%20021901.png) |
</details>

<details>
  <summary>Coordinator Status Page</summary>
  
  
  | Before | After |
  | ------ | ----- |
  | ![Before login](screenshots/coordinator_status/old/old.png) |![After login 1](screenshots/coordinator_status/new/Screenshot%202025-09-16%20022133.png)<br>![After login 2](screenshots/coordinator_status/new/Screenshot%202025-09-16%20022242.png) |
</details>

<details>
  <summary>Workshop-Statistics Page</summary>
  
  
  | Before | After |
  | ------ | ----- |
  | ![Before login](screenshots/work_shop_stats/old/old.png) |![After login 1](screenshots/work_shop_stats/new/Screenshot%202025-09-16%20023014.png)<br>![After login 2](screenshots/work_shop_stats/new/Screenshot%202025-09-16%20023022.png)<br>![After login 3](screenshots/work_shop_stats/new/Screenshot%202025-09-16%20023138.png)<br>![After login 4](screenshots/work_shop_stats/new/Screenshot%202025-09-16%20023303.png) | 
</details>

<details>
  <summary>Instructor Status Page</summary>
  

  | Before | After |
  | ------ | ----- |
  | ![Before login](screenshots/instructor_status/old/old.png) |![After login 1](screenshots/instructor_status/new/Screenshot%202025-09-16%20023847.png)<br>![After login 2](screenshots/instructor_status/new/Screenshot%202025-09-16%20023909.png) |
</details>

<details>
  <summary>Propose Workshop Page</summary>
  
  | Before | After |
  | ------ | ----- |
  | ![Before login](screenshots/propose_workshop/old/old.png) |![After login 1](screenshots/propose_workshop/new/Screenshot%202025-09-16%20024134.png)<br>![After login 2](screenshots/propose_workshop/new/Screenshot%202025-09-16%20024201.png) |
</details>


<details>
  <summary>Edit Workshop Type Page</summary>
  
  
  | Before | After |
  | ------ | ----- |
  | ![Before login](screenshots/edit_workshop_type/old/old.png) |![After login 1](screenshots/edit_workshop_type/new/Screenshot%202025-09-16%20024459.png)<br>![After login 2](screenshots/edit_workshop_type/new/Screenshot%202025-09-16%20024837.png) |
</details>

<details>
  <summary>View Profile Page</summary>
  
  
  | Before | After |
  | ------ | ----- |
  | ![Before login](screenshots/profile/old/old.png) |![After login 1](screenshots/profile/new/Screenshot%202025-09-16%20031159.png)<br>![After login 2](screenshots/profile/new/Screenshot%202025-09-16%20031332.png) |
</details>


<details>
  <summary>Workshop Details Page</summary>
  
 
  | Before | After |
  | ------ | ----- |
  | ![Before login](screenshots/workshop_details/old/old.png) |![After login 1](screenshots/workshop_details/new/Screenshot%202025-09-16%20031901.png)<br>![After login 2](screenshots/workshop_details/new/Screenshot%202025-09-16%20031925.png)<br>![After login 3](screenshots/workshop_details/new/Screenshot%202025-09-16%20031950.png) |
</details>


<details>
  <summary>Workshop Type Details Page</summary>
  
  
  | Before | After |
  | ------ | ----- |
  | ![Before login](screenshots/workshop_type_details/old/old.png) |![After login 1](screenshots/workshop_type_details/new/Screenshot%202025-09-16%20032625.png) |
</details>


<details>
  <summary>Workshop Types List Page</summary>
  
  
  | Before | After |
  | ------ | ----- |
  | ![Before login](screenshots/workshop_type_list/old/old.png) |![After login 1](screenshots/workshop_type_list/new/Screenshot%202025-09-16%20033133.png)<br>![After login 2](screenshots/workshop_type_list/new/Screenshot%202025-09-16%20033218.png) |
</details>

<details>
  <summary>Add Workshop Type Page</summary>
  
  
  | Before | After |
  | ------ | ----- |
  | ![Before login](screenshots/add_workshop_type/new/Screenshot%202025-09-16%20034309.png) |![After login 1](screenshots)<br>![After login 2](screenshots) |
</details>

<details>
  <summary>Team Statistics Page</summary>
  
  
  | Before | After |
  | ------ | ----- |
  | ![Before login](screenshots/team_stats/old/old.png) |![After login 1](screenshots/team_stats/new/Screenshot%202025-09-16%20033933.png) |
</details>

---

## Design Reasoning

### 1️⃣ Design Principles (As Used in This Project)



- **Mobile-first Approach**  
  Ensured seamless use on phones and tablets through responsive layouts, collapsible navigation, and touch-friendly controls.

- **Visual Consistency**  
  Applied a unified dark-and-green color palette, consistent spacing, and standardized layouts for cards and tables.

- **Clear Information Hierarchy**  
  Used headings, icons, and card layouts to guide users in quickly understanding page structure and locating key actions or data.

- **Role-based UI**  
  Designed the interface to adapt by user type (instructor, coordinator, admin) so each user only sees relevant actions and information.

- **Modern & Lively Experience**  
  Added subtle animations (using GSAP) and balanced use of black and green shades to create a fresh, engaging feel while keeping load times optimized.


### 2️⃣ Ensuring Responsiveness Across Devices

- Built the base layout using **Bootstrap’s responsive grid system** and components, and then built upon it.  
- Applied knowledge from **TailwindCSS/ CSS** (similar utility classes) to fine-tune spacing and alignment.  
- Used **card-based layouts** for storing and displaying data, which simplified responsiveness across different pages.  
- Focused primarily on **mobile phones and laptops**, ensuring navigation and readability remain smooth across both.  



### 3️⃣ Trade-offs Between Design and Performance

- I aimed to maintain a **balance** between design quality and performance.  
- Prioritized an **interactive and lively design** to improve user engagement.
- Used advanced, high-performance animations JS library live **GSAP**, that is not considered heavy.  
- At the same time, kept the site **lightweight**, ensuring load times and accessibility were not compromised.  
- The approach leaned slightly towards **design enhancements**, but without adding heavy or unnecessary elements that could slow down performance.  



### 4️⃣Challenges and How I Approached Them

- **Design Choices**: Choosing the right color combinations and overall theme was time-consuming, as I wanted the UI to be modern yet readable.  
- **Bootstrap Complexity**: While Bootstrap helped with responsiveness, its default classes and utilities often conflicted with my custom design. I had to carefully study and override them, supported by my background in Tailwind CSS.  
- **Maintaining Responsiveness**: Ensuring a smooth experience across devices was challenging. I adopted a **card-based structure** for data display, which worked well for consistency and mobile-friendliness, though adapting cards to every page sometimes required extra adjustments.  
- **UI-Functionality Alignment**: Some existing functionality did not align well with the new design, and in a few cases, I found issues that needed fixing. I modified views and forms where necessary to ensure the UI and functionality matched correctly.  
- **Bug Fix**: Fixed an error related to automatic redirection of a superuser to the admin panel after login, ensuring smoother workflow for administrators.  


### ✅ Overall Summary

This project focused on enhancing the **UI/UX of the workshop booking system** while keeping the core structure intact.  
The improvements were guided by **mobile-first design principles**, consistent visuals, and a clear information hierarchy.  
By leveraging **Bootstrap** as the base, fine-tuning layouts with CSS utilities, and using a **card-based structure**, I ensured responsiveness across devices, especially for mobile and laptop users.  

I carefully balanced **design and performance**, introducing modern animations with **GSAP** for a lively experience while keeping the site lightweight and accessible.  
During development, I faced challenges around design decisions, Bootstrap overrides, and maintaining responsiveness, but resolved them through structured approaches and prior CSS knowledge.  
Additionally, I fixed some functional issues, including an error with **superuser auto-redirection to the admin panel**, ensuring smoother workflows.  

Overall, the redesigned interface is **cleaner, more responsive, and user-friendly**, delivering a better experience for students and administrators alike.  


> 📝 This project was developed as part of the **Python Screening Task 1: UI/UX Enhancement** for FOSSEE Semester Long Internship - Autumn 2025