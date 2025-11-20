# Ex.07 Restuarant Website
## Date:

## AIM:
To develop a static Resturant website to display the menu and services provided by the resturant.

## DESIGN STEPS:

### Step 1:
Requirement collection.

### Step 2:
Creating the layout using HTML and CSS.

### Step 3:
Updating the sample content.

### Step 4:
Choose the appropriate style and color scheme.

### Step 5:
Validate the layout in various browsers.

### Step 6:
Validate the HTML code.

### Step 7:
Publish the website in the given URL.

## PROGRAM:

```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Chini Chaatka Kitchen | Restaurant</title>
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      font-family: 'Segoe UI', sans-serif;
    }

    body {
      line-height: 1.6;
      color: #6431dc;
      background-color: #fdfdfd;
    }

    header {
      background: url('bb.jpg') no-repeat center center/cover;
      height: 100vh;
      color: rgb(133, 60, 60);
      text-align: center;
      display: flex;
      flex-direction: column;
      justify-content: flex-start;
      align-items: center;
      padding-top: 40px;

    }

    header h1 {
      font-size: 4rem;
      margin: 0;
      font-style: italic;
      background-color: black;
      color: white;
      display: inline-block;
      padding: 5px 10px;
    }

    header p {
      font-size: 1.5rem;
    }

    nav {
      background-color: #141313;
      display: flex;
      justify-content: center;
      padding: 15px 0;
      position: sticky;
      top: 0;
      z-index: 100;
    }

    nav a {
      color: white;
      margin: 0 20px;
      text-decoration: none;
      font-weight: bold;
      transition: color 0.3s ease;
    }

    nav a:hover {
      color: #f4b400;
    }

    section {
      background: url('bb.jpg') no-repeat center center/cover;
      height: 100vh;
      color: white;
      text-align: center;
      display: flex;
      flex-direction: column;
      justify-content: center;
      padding: 0 20px;
    }

    .menu {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 20px;
    }

    .menu-item {
      background: rgb(29, 29, 28);
      border: 1px solid #111111;
      border-radius: 10px;
      padding: 20px;
      text-align: center;
      box-shadow: 0 2px 5px rgba(0,0,0,0.1);
    }

    .menu-item img {
      width: 100%;
      height: 200px;
      object-fit: cover;
      border-radius: 8px;
    }

    .chefs {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      gap: 40px;
      margin-top: 40px;
    }

    .chef-card {
      background: rgb(211, 39, 39);
      border: 1px solid #ddd;
      border-radius: 10px;
      text-align: center;
      padding: 20px;
      width: 250px;
      box-shadow: 0 2px 5px rgba(0,0,0,0.1);
    }

    .chef-card img {
      width: 150px;
      height: 150px;
      object-fit: cover;
      border-radius: 50%;
      margin-bottom: 15px;
    }

    .about, .contact, .book {
      background-color: #0f0202;
      border-radius: 10px;
      padding: 30px;
    }

    .book form {
      display: flex;
      flex-direction: column;
      gap: 15px;
    }

    .book input, .book textarea {
      padding: 10px;
      border: 1px solid #041017;
      border-radius: 5px;
    }

    .book button {
      background-color: #222;
      color: white;
      padding: 10px;
      border: none;
      border-radius: 5px;
      cursor: pointer;
      font-weight: bold;
    }

    .book button:hover {
      background-color: #f4b400;
      color: black;
    }

    footer {
      text-align: center;
      padding: 20px;
      background-color: #222;
      color: rgb(179, 173, 173);
    }

    @media (max-width: 600px) {
      header h1 {
        font-size: 2.5rem;
      }

      nav {
        flex-direction: column;
      }

      nav a {
        margin: 10px 0;
      }

      .chefs {
        flex-direction: column;
        align-items: center;
      }
    }
  </style>
</head>
<body>

  <header>
    <h1>Chini Chaatka Kitchen</h1>
    <h2><b>Vishagan RS 25002817</b></h2>
    <p>"Where every meal is a masterpiece, and every bite tells a story"</p>
  </header>

  <nav>
    <a href="#menu">Menu</a>
    <a href="#chefs">Chefs</a>
    <a href="#book">Book</a>
    <a href="#about">About</a>
    <a href="#contact">Contact</a>
  </nav>

  <section id="menu">
    <h2>Our Menu</h2>
    <div class="menu">
      <div class="menu-item"><img src="c:\Users\admin\Web\NearMe\bakkiya\mapapp\static\Cheese Balls.jpg"><h3>CHEESE BALL</h3></div>
      <div class="menu-item"><img src="c:\Users\admin\Web\NearMe\bakkiya\mapapp\static\Garlic bread.jpg"><h3>GARLIC BREAD</h3></div>
      <div class="menu-item"><img src="c:\Users\admin\Web\NearMe\bakkiya\mapapp\static\Momos.jpg"><h3>MOMOS</h3></div>
      <div class="menu-item"><img src="c:\Users\admin\Web\NearMe\bakkiya\mapapp\static\Noodles.jpg"><h3>NOODLES</h3></div>
      <div class="menu-item"><img src="c:\Users\admin\Web\NearMe\bakkiya\mapapp\static\Rice.jpg"><h3>SCHEZWAN RICE</h3></div>
      <div class="menu-item"><img src="c:\Users\admin\Web\NearMe\bakkiya\mapapp\static\Spring roll.jpg"><h3>SPRING ROLL</h3></div>
    </div>
  </section>

  <section id="chefs">
    <h2>Meet Our Chefs</h2>
    <div class="chefs">
      <div class="chef-card"><img src="c:\Users\admin\Web\NearMe\bakkiya\mapapp\static\Dhamu.jpg"><h3>Chef Damu</h3><p>Chef Damu is known for South Indian culinary expertise.</p></div>
    
      <div class="chef-card"><img src="c:\Users\admin\Web\NearMe\bakkiya\mapapp\static\Vikhas.jpg"><h3>Chef Vikas Khanna</h3><p>World-renowned Indian chef and author.</p></div>
    </div>
  </section>

  <section id="book" class="book">
    <h2>Book a Table</h2>
    <form>
      <input type="text" placeholder="Full Name" required>
      <input type="email" placeholder="Email Address" required>
      <input type="tel" placeholder="Phone Number" required>
      <input type="date" required>
      <input type="time" required>
      <input type="number" placeholder="Number of Guests" required>
      <textarea placeholder="Special Requests"></textarea>
      <button type="submit">Reserve Now</button>
    </form>
  </section>

  <section id="about" class="about">
    <h2>About Us</h2>
    <p>At Chini Chaatka Kitchen, we blend tradition with taste. Every dish is made with love and passion to give you the best culinary experience.</p>
  </section>

  <section id="contact" class="contact">
    <h2>Contact</h2>
    <p><strong>Address:</strong> Food Town, Tamil Nadu</p>
    <p><strong>Phone:</strong> +91 10987 65432</p>
    <p><strong>Email:</strong> chinichaatakakitchen@gmail.com</p>
  </section>

  <footer>
    <p>&copy; 2025 Chini Chaatka Kitchen. All rights reserved.</p>
  </footer>

</body>
</html>

```

## OUTPUT:

<img width="1900" height="1088" alt="image" src="https://github.com/user-attachments/assets/0b188c53-a404-4305-b5dc-7fa1633b4d54" />

<img width="1902" height="1062" alt="image" src="https://github.com/user-attachments/assets/c0bfa1c4-3266-49c4-8018-c2e1028bfe4a" />

<img width="1888" height="961" alt="image" src="https://github.com/user-attachments/assets/90095d2c-1e90-4a8b-ba7b-63031adcdb42" />

<img width="1902" height="993" alt="image" src="https://github.com/user-attachments/assets/05d53d60-2854-4912-9c47-43640d998031" />

<img width="1919" height="724" alt="image" src="https://github.com/user-attachments/assets/7b033850-0619-4b51-913b-f9cdf21654c8" />

<img width="1915" height="1015" alt="image" src="https://github.com/user-attachments/assets/c1ce18a9-596a-490b-bbdb-9b6b7bdf6ba0" />


## RESULT:
The program for designing software company website using HTML and CSS is completed successfully.
