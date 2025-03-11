# ✈️ SkyVoyage

This project focuses on implementing a given design and translating it into code using Vue.js. Our task was to accurately follow the design specifications and visual guidelines to create a fully functional and responsive web application.

[Link to live version](https://medieinstitutet.github.io/fed24d-grafiska-verktyg-mandarinfiskarna/)

[Link to Figma design](https://www.figma.com/design/0uhAuKSgWbY6wmtoa6Ddx9/Dabbagam?node-id=5-50&t=oNVcVJKLufmXLho4-1)

## 📒 Table of Contents

- [What we did](#what-we-did)
- [Features](#features)
- [Tech Stack](#tech-stack)
- [Installation](#installation)
- [Screenshots](#screenshots)
  - [Wireframes](#wireframes)
- [Documentation](#documentation)
  - [Lighthouse report](#lighthouse-report)
  - [Validation](#validation)
- [Authors](#authors)

## 🗺️ What we did
- **Design Implementation:** We received a design created in Figma and translated it into code while ensuring pixel-perfect accuracy.
- **Vue.js Development:** The project was built using Vue.js, leveraging its component-based architecture for maintainability and scalability.
- **Responsive Design:** We ensured that the application works seamlessly across different screen sizes and devices.
- **Code Structure & Best Practices:** The project follows clean code principles and best practices to enhance readability, reusability, and maintainability.

## 🗝️ Features

* **Cookie Popup & Banner:** Our website uses cookies to improve your experience. When you visit, a popup banner will appear letting you know about it. You can easily hide the popup or banner by clicking the "Accept" or "Decline" buttons.
  
* **Product Cards as Props:** To make it easier to create more product cards on the site, we've set them up to be added through props. This allows you to add new products without having to rewrite the same code every time. It's a flexible and efficient way to keep the site scalable and easy to update.

* **Dynamic Review Carousel:** Users can cycle through reviews with smooth fade transitions. We created an IReview interface to structure the reviews, making it easy to add more reviews to the array over time.

* **Easy Review Navigation:** The nextReview and previousReview functions allow users to navigate through reviews, with the carousel looping back to the start when reaching the end.

* **Interactive Navigation Bar for tablet & desktop:** The navbar highlights the active link using Vue's ref, and adds hover effects for a better user experience.

* **Booking Form with v-Model:** Our booking form uses v-model to bind the input fields to their respective values. This ensures that the data entered by users is automatically synchronized with the form fields. On form submission, a function validates the inputs, ensuring that the fields are not empty before proceeding. The form also handles the submit action, and another function is triggered to clear all input fields once the form is submitted.

* **Dynamic and Mobile-Friendly Navigation:** The project includes two navigation bars. The first is a standard navbar for larger screens with active link highlighting and hover effects. The second is a mobile-only bottom navbar, which appears on smaller screens and offers easy access to Home, Luftballong, and Boka using intuitive icons.

* **SVG Animation Created with GSAP:** An animated SVG logo featuring a plane flying away on a continuous loop. The animation is built using GSAP to ensure smooth motion and high performance.

## 💻 Tech Stack

- ![Vite](https://img.shields.io/badge/Vite-%23646CFF.svg?style=for-the-badge&logo=vite&logoColor=white)
- ![Vue.js](https://img.shields.io/badge/Vue.js-%234FC08D.svg?style=for-the-badge&logo=vue.js&logoColor=white)
- ![TypeScript](https://img.shields.io/badge/TypeScript-%23007ACC.svg?style=for-the-badge&logo=typescript&logoColor=white)
- ![Sass](https://img.shields.io/badge/Sass-%23CC6699.svg?style=for-the-badge&logo=sass&logoColor=white)
- ![ESLint](https://img.shields.io/badge/ESLint-%234B32C3.svg?style=for-the-badge&logo=eslint&logoColor=white)
- ![Prettier](https://img.shields.io/badge/Prettier-%23F7B93E.svg?style=for-the-badge&logo=prettier&logoColor=white)

## 🚀 Installation

Install fed24d-grafiska-verktyg-mandarinfiskarna locally with pnpm

```bash
# Clone this repository
$ git clone https://github.com/Medieinstitutet/fed24d-grafiska-verktyg-mandarinfiskarna

# Go into the repository
$ cd fed24d-grafiska-verktyg-mandarinfiskarna

# Install dependencies
$ pnpm install

# Run app
$ pnpm run dev
```

## 📸 Screenshots

### Mobile

![Screenshot mobile screen](/assets/screenshots/mobil.png)

### tablet

![Screenshot tablet screen](/assets/screenshots/tablet.png)

### Desktop

![Screenshot desktop welcome-screen](/assets/screenshots/desktop.png)

### Wireframes

#### Desktop
![Wireframe desktop](/assets/screenshots/wireframe-desktop.png)

#### Tablet

![Wireframe tablet home](/assets/screenshots/wireframe-tablet.png)

#### Mobile

![Wireframe mobile home](/assets/screenshots/wireframe-mobile.png)

## 📝 Documentation

### Lighthouse report

![Lighthouse_report](/assets/validation/lighthouse.png)

### Validation

#### HTML

![Validation HTML](/assets/validation/HTML_validation.png)

## 👩‍💻 Authors

- [@karinHson](https://github.com/KarinHson)
- [@TeaGross](https://github.com/TeaGross)
- [@axandranathalie](https://github.com/axandranathalie)
- [@ellinorjohansson](https://github.com/ellinorjohansson)
