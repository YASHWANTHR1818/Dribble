# Project Responsive Web Design using Bootstrap
## Date:17/11/2025

## AIM:
To create a simplified clone of Dribbble (https://dribbble.com/) landing page.


## DESIGN STEPS:

### Step 1:
Clone the repository from GitHub.

### Step 2:
Create Django Admin project.

### Step 3:
Create a New App under the Django Admin project.

### Step 4:
Insert the necessary CSS and JavaScript files as external in order to use Bootstrap.

### Step 5:
Create a HTML file and include the needed Bootstrap components.

### Step 6:
Publish the website in the LocalHost.


## PROGRAM :

```
login.html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Login | Car Booking</title>

    <!-- Bootstrap CSS -->
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/css/bootstrap.min.css" rel="stylesheet">

    <style>
        body {
            background: #f1f3f4;
        }
        .login-box {
            margin-top: 80px;
            background: #fff;
            padding: 30px;
            border-radius: 12px;
            box-shadow: 0 0 20px rgba(0,0,0,0.1);
        }
    </style>
</head>
<body>

<!-- Navbar -->
<nav class="navbar navbar-expand-lg navbar-dark bg-dark">
  <div class="container">
    <a class="navbar-brand fw-bold" href="index.html">CarBooking</a>
  </div>
</nav>

<!-- Login Box -->
<div class="container">
    <div class="row justify-content-center">
        <div class="col-md-4">

            <div class="login-box">
                <h3 class="text-center mb-4 fw-bold">Login</h3>

                <form>
                    <label class="form-label">Email</label>
                    <input type="email" class="form-control mb-3" placeholder="Enter your email" required>

                    <label class="form-label">Password</label>
                    <input type="password" class="form-control mb-3" placeholder="Enter your password" required>

                    <button class="btn btn-primary w-100 mt-2">Login</button>
                </form>

                <p class="text-center mt-3">
                    <small>Don't have an account? <a href="#">Register</a></small>
                </p>
            </div>

        </div>
    </div>
</div>

<!-- Bootstrap JS -->
<script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/js/bootstrap.bundle.min.js"></script>

</body>
</html>

index.html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Car Booking | Home</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/css/bootstrap.min.css" rel="stylesheet">
</head>
<body>

<!-- Navbar -->
<nav class="navbar navbar-expand-lg navbar-dark bg-dark">
  <div class="container">
    <a class="navbar-brand fw-bold" href="index.html">CarBooking</a>
    <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav">
      <span class="navbar-toggler-icon"></span>
    </button>
    <div class="collapse navbar-collapse" id="navbarNav">
      <ul class="navbar-nav ms-auto">
        <li class="nav-item"><a class="nav-link active" href="index.html">Home</a></li>
        <li class="nav-item"><a class="nav-link" href="cars.html">Cars</a></li>
        <li class="nav-item"><a class="nav-link" href="booking.html">Booking</a></li>
        <li class="nav-item"><a class="nav-link" href="contact.html">Contact</a></li>
        <li class="nav-item"><a class="nav-link" href="login.html">Login</a></li>
      </ul>
    </div>
  </div>
</nav>

<!-- Hero Section -->
<section class="bg-dark text-light text-center p-5">
  <div class="container">
    <h1 class="display-4 fw-bold">Book Your Dream Car Today</h1>
    <p class="lead">Best prices. Best quality. Trusted service.</p>
    <a href="cars.html" class="btn btn-primary btn-lg">View Cars</a>
  </div>
</section>

<!-- Features -->
<div class="container my-5">
  <div class="row text-center">
    <div class="col-md-4">
      <h3 class="fw-bold">Wide Car Collection</h3>
      <p>Choose from economy, luxury, SUVs and more.</p>
    </div>
    <div class="col-md-4">
      <h3 class="fw-bold">Affordable Pricing</h3>
      <p>Best price guaranteed across all categories.</p>
    </div>
    <div class="col-md-4">
      <h3 class="fw-bold">24/7 Support</h3>
      <p>Dedicated team always ready to assist.</p>
    </div>
  </div>
</div>

<!-- Footer -->
<footer class="bg-dark text-center text-light p-3">
  <p class="mb-0">© 2025 CarBooking. All Rights Reserved.</p>
</footer>

<script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/js/bootstrap.bundle.min.js"></script>
</body>
</html>

contact.html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Contact | Car Booking</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/css/bootstrap.min.css" rel="stylesheet">
</head>
<body>

<nav class="navbar navbar-expand-lg navbar-dark bg-dark">
  <div class="container">
    <a class="navbar-brand fw-bold" href="index.html">CarBooking</a>
    <div class="collapse navbar-collapse">
      <ul class="navbar-nav ms-auto">
        <li><a class="nav-link" href="index.html">Home</a></li>
        <li><a class="nav-link" href="cars.html">Cars</a></li>
        <li><a class="nav-link" href="booking.html">Booking</a></li>
        <li><a class="nav-link active" href="contact.html">Contact</a></li>
        <li><a class="nav-link" href="login.html">Login</a></li>
      </ul>
    </div>
  </div>
</nav>

<div class="container my-5">
  <h2 class="fw-bold text-center mb-4">Contact Us</h2>

  <form class="mx-auto" style="max-width: 600px;">
    <label>Name</label>
    <input type="text" class="form-control mb-3" required>

    <label>Email</label>
    <input type="email" class="form-control mb-3" required>

    <label>Message</label>
    <textarea class="form-control mb-3" rows="4" required></textarea>

    <button class="btn btn-primary w-100">Send Message</button>
  </form>
</div>

<footer class="bg-dark text-center text-light p-3">
  <p class="mb-0">© 2025 CarBooking. All Rights Reserved.</p>
</footer>

</body>
</html>

cars.html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Cars | Car Booking</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/css/bootstrap.min.css" rel="stylesheet">
</head>
<body>

<!-- Navbar -->
<nav class="navbar navbar-expand-lg navbar-dark bg-dark">
  <div class="container">
    <a class="navbar-brand fw-bold" href="index.html">CarBooking</a>
    <div class="collapse navbar-collapse">
      <ul class="navbar-nav ms-auto">
        <li class="nav-item"><a class="nav-link" href="index.html">Home</a></li>
        <li class="nav-item"><a class="nav-link active" href="cars.html">Cars</a></li>
        <li class="nav-item"><a class="nav-link" href="booking.html">Booking</a></li>
        <li class="nav-item"><a class="nav-link" href="contact.html">Contact</a></li>
        <li class="nav-item"><a class="nav-link" href="login.html">Login</a></li>
      </ul>
    </div>
  </div>
</nav>

<div class="container my-5">
  <h2 class="text-center fw-bold mb-4">Available Cars</h2>
  <div class="row g-4">
    
    <!-- Car Card -->
    <div class="col-md-4">
      <div class="card shadow">
        <img src="https://th.bing.com/th/id/OIP.kHWtLpBhqmpUfCY9E7NOmQHaEh?o=7rm=3&rs=1&pid=ImgDetMain&o=7&rm=3" class="card-img-top" alt="Car">
        <div class="card-body">
          <h5 class="card-title">Toyota Fortuner</h5>
          <p class="card-text">₹2500/day</p>
          <a href="booking.html" class="btn btn-primary w-100">Book Now</a>
        </div>
      </div>
    </div>

    <!-- Repeat cards -->
    <div class="col-md-4">
      <div class="card shadow">
        <img src="https://th.bing.com/th/id/OIP.YQ2hx3afy7XC7QNjcGxIFAHaEo?o=7rm=3&rs=1&pid=ImgDetMain&o=7&rm=3" class="card-img-top">
        <div class="card-body">
          <h5 class="card-title">BMW X5</h5>
          <p class="card-text">₹6500/day</p>
          <a href="booking.html" class="btn btn-primary w-100">Book Now</a>
        </div>
      </div>
    </div>

    <div class="col-md-4">
      <div class="card shadow">
        <img src="https://images.hgmsites.net/med/2019-bmw-x4_100656587_m.jpg" class="card-img-top">
        <div class="card-body">
          <h5 class="card-title">BMW X4</h5>
          <p class="card-text">₹4500/day</p>
          <a href="booking.html" class="btn btn-primary w-100">Book Now</a>
        </div>
      </div>
    </div>

    <div class="col-md-4">
      <div class="card shadow">
        <img src="https://tse2.mm.bing.net/th/id/OIP.0ESxbpqrS9Unsz97Qs0WowHaEK?rs=1&pid=ImgDetMain&o=7&rm=3" class="card-img-top">
        <div class="card-body">
          <h5 class="card-title"> MS Ertiga</h5>
          <p class="card-text">₹1500/day</p>
          <a href="booking.html" class="btn btn-primary w-100">Book Now</a>
        </div>
      </div>
    </div>

    <div class="col-md-4">
      <div class="card shadow">
        <img src="https://wallpapercave.com/wp/wp4555947.jpg" class="card-img-top">
        <div class="card-body">
          <h5 class="card-title">Mahindra Thar</h5>
          <p class="card-text">₹10000/day</p>
          <a href="booking.html" class="btn btn-primary w-100">Book Now</a>
        </div>
      </div>
    </div>

    <div class="col-md-4">
      <div class="card shadow">
        <img src="https://www.bing.com/th/id/OIP.P9mOJWAHL-YNTUC5_M8cZQHaEK?w=225&h=211&c=8&rs=1&qlt=90&o=6&dpr=1.3&pid=3.1&rm=2" class="card-img-top">
        <div class="card-body">
          <h5 class="card-title">Audi R8</h5>
          <p class="card-text">₹9000/day</p>
          <a href="booking.html" class="btn btn-primary w-100">Book Now</a>
        </div>
      </div>
    </div>

  </div>
</div>

<footer class="bg-dark text-center text-light p-3">
  <p class="mb-0">© 2025 CarBooking. All Rights Reserved.</p>
</footer>

</body>
</html>

booking.html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Booking | Car Booking</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/css/bootstrap.min.css" rel="stylesheet">
</head>
<body>

<nav class="navbar navbar-expand-lg navbar-dark bg-dark">
  <div class="container">
    <a class="navbar-brand fw-bold" href="index.html">CarBooking</a>
    <div class="collapse navbar-collapse">
      <ul class="navbar-nav ms-auto">
        <li><a class="nav-link" href="index.html">Home</a></li>
        <li><a class="nav-link" href="cars.html">Cars</a></li>
        <li><a class="nav-link active" href="booking.html">Booking</a></li>
        <li><a class="nav-link" href="contact.html">Contact</a></li>
        <li><a class="nav-link" href="login.html">Login</a></li>
      </ul>
    </div>
  </div>
</nav>

<div class="container my-5">
  <h2 class="text-center fw-bold">Car Booking Form</h2>

  <form class="mt-4 mx-auto" style="max-width: 600px;">
    <label class="form-label">Full Name</label>
    <input type="text" class="form-control mb-3" required>

    <label class="form-label">Phone</label>
    <input type="text" class="form-control mb-3" required>

    <label class="form-label">Select Car</label>
    <select class="form-select mb-3">
      <option>Toyota Fortuner</option>
      <option>BMW X5</option>
      <option>Audi R8</option>
    </select>

    <label class="form-label">Pick-up Date</label>
    <input type="date" class="form-control mb-3" required>

    <label class="form-label">Drop-off Date</label>
    <input type="date" class="form-control mb-3" required>

    <button class="btn btn-primary w-100">Submit Booking</button>
  </form>
</div>

<footer class="bg-dark text-center text-light p-3">
  <p class="mb-0">© 2025 CarBooking. All Rights Reserved.</p>
</footer>

</body>
</html>
```



## OUTPUT:
![alt text](<Screenshot 2025-11-17 092023.png>)
![alt text](<Screenshot 2025-11-17 092047.png>)
![alt text](<Screenshot 2025-11-17 092103.png>)
![alt text](<Screenshot 2025-11-17 092115.png>)
![alt text](<Screenshot 2025-11-17 092126.png>)

## RESULT:
The Project for responsive web design using Bootstrap is completed successfully.
