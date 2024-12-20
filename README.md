# Exercise Laravel 11 React Inertia.js
Simple CRUD website by combining Laravel 11, React, and Inertia Frameworks.


## Prerequisite:

- Composer
- PHP >= 8.3
- Node >= 22


## Features

- Authentication: register & login
- Update & Delete Account
- CRUD Post


## Screenshots

<div style="display: flex; overflow: hidden; width: 100%; position: relative;">
  <div style="display: flex; transition: transform 0.5s ease-in-out;">
    <img src="./Documentation/Dashboard.png" alt="Login versi desktop" style="width: 100%; max-width: 100%;"/>
    <img src="./Documentation/Add Post.png" alt="Dashboard versi desktop" style="width: 100%; max-width: 100%;"/>
    <img src="./Documentation/List Post.png" alt="Halaman Exam Versi Desktop" style="width: 100%; max-width: 100%;"/>
  </div>
  <button onclick="moveCarousel(-1)" style="position: absolute; top: 50%; left: 0; background-color: rgba(0,0,0,0.5); color: white; border: none; padding: 10px;">&#10094;</button>
  <button onclick="moveCarousel(1)" style="position: absolute; top: 50%; right: 0; background-color: rgba(0,0,0,0.5); color: white; border: none; padding: 10px;">&#10095;</button>
</div>

<script>
  let currentIndex = 0;

  function moveCarousel(direction) {
    const carousel = document.querySelector('div > div');
    const images = carousel.querySelectorAll('img');
    const totalImages = images.length;
    currentIndex = (currentIndex + direction + totalImages) % totalImages;
    carousel.style.transform = `translateX(-${currentIndex * 100}%)`;
  }
</script>


## Run Locally

Clone the project

```bash
    git clone https://github.com/brianajiks123/Simple-CRUD-Post-Laravel11-React-Inertia.git
```

Go to the project directory

```bash
    cd Simple-CRUD-Post-Laravel11-React-Inertia
```

Install Dependencies (Laravel)

```bash
    composer install
```

Install Dependencies (Node)

```bash
    npm install
```

Migrate Database (make sure already setup your environment in the .env file)

```bash
    php artisan migrate
```

Running Runtime

```bash
    npm run dev
```

Running Development

```bash
    php artisan serve
```


## Tech Stack

**Client:** HTML, CSS (Tailwind), JavaScript (React & Inertia), Chrome

**Server:** Laravel 11, Breeze, MySQL, Git, Apache Web Server, VS Code, Windows 11


## Acknowledgements

 - [Laravel](https://laravel.com/docs/11.x)


## Authors

- [@brianajiks123](https://www.github.com/brianajiks123)
