#first webpage
#ABOUT
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>About Us</title>
 <link rel="stylesheet" href="style.css">
 
</head>
<body>
  <header><h1>About Us</h1></header>
  <nav>
    <a href="index.html">Home</a>
    <a href="about.html" class="active">About Us</a>
    <a href="services.html">Services</a>
    <a href="contact.html">Contact Us</a>
  </nav>
  <table>
    <tr><th>Name</th><th>Role</th><th>Contact</th></tr>
    <tr><td>Arsalan</td><td>WebDeveloper</td><td>arsalan242@gmail.com</td></tr>
    <tr><td>Saad</td><td>GraphicDesigner</td><td>saad125@gmail.com</td></tr>
  </table>

</body>
</html>


#contact
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Contact Us</title>

<link rel="stylesheet" href="style.css">

</head>
<body>
  <header><h1>Contact Us</h1></header>
  <nav>
    <a href="index.html">Home</a>
    <a href="about.html">About Us</a>
    <a href="services.html">Services</a>
    <a href="contact.html" class="active">Contact Us</a>
  </nav>
  <form>
    <label for="name">Name</label>
    <input type="text" id="name" name="name" required>
    
    <label for="email">Email</label>
    <input type="email" id="email" name="email" required>
    
    <label for="message">Message</label>
    <textarea id="message" name="message" rows="5" required></textarea>
    
    <button type="submit">Submit</button>
  </form>

</body>
</html>


#index
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Arsalan WEB</title>
 
<link rel="stylesheet" href="style.css">

</head>
<body>
  <header>
    <h1>Welcome to My Advanced CSS Website</h1>
  </header>
  <nav>
    <a href="index.html" class="active">Home</a>
    <a href="about.html">About Us</a>
    <a href="services.html">Services</a>
    <a href="contact.html">Contact Us</a>
  </nav>
  <section class="intro">
    <p>Welcome to our website a showcase of modern web design powered by advanced CSS techniques. This platform highlights the effective use of Flexbox layouts to create responsive and well-structured pages along with styled tables that present information in a clean and organized way. You will also find interactive forms designed to enhance user experience and improve accessibility across different devices. As you explore the site you will learn more about our dedicated team gain a deeper understanding of the services we provide and see how thoughtful design choices contribute to functional and visually appealing interfaces. This website demonstrates advanced CSS techniques including Flexbox layouts, styled tables and interactive forms. Explore the pages to learn more about our team services and how to contact us.</p>
  </section>

</body>
</html>



#services
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Services</title>


<link rel="stylesheet" href="style.css">

</head>
<body>
  <header><h1>Our Services</h1></header>
  <nav>
    <a href="index.html">Home</a>
    <a href="about.html">About Us</a>
    <a href="services.html" class="active">Services</a>
    <a href="contact.html">Contact Us</a>
  </nav>
  <section class="services">
    <div class="card">
      <img src="web1">
      <h3>Web Development</h3>
      <p>We build responsive and modern websites tailored to your needs.</p>
      <button>Learn More</button>
    </div>
    <div class="card">
      <img src="graphic1">
      <h3>Graphic Design</h3>
      <p>Creative designs that make your brand stand out visually.</p>
      <button>Learn More</button>
    </div>
    <div class="card">
      <img src="seo1">
      <h3>SEO Optimization</h3>
      <p>Boost your website’s visibility with our SEO strategies.</p>
      <button>Learn More</button>
    </div>
  </section>
</body>
</html>



#style
  /* Global Reset */
* { box-sizing: border-box; margin: 0; padding: 0; }

body {
  font-family: 'Segoe UI', Arial, sans-serif;
  background: #f8fafc;
  color: #0f172a;
}

header {
  background: linear-gradient(135deg, #1e293b, #334155);
  color: white;
  padding: 30px 20px;
  text-align: center;
}

nav {
  display: flex;
  justify-content: center;
  background: #1e293b;
}

nav a {
  color: white;
  padding: 15px 22px;
  text-decoration: none;
  font-weight: 500;
  transition: all 0.3s ease;
}

nav a:hover,
nav a.active {
  background: #38bdf8;
  color: #0f172a;
}

/* Intro Section */
.intro {
  padding: 80px 15%;
  text-align: center;
  line-height: 1.8;
  font-size: 18px;
}

/* Table Styling */
table {
  margin: 50px auto;
  border-collapse: collapse;
  width: 65%;
  background: white;
  border-radius: 10px;
  overflow: hidden;
  box-shadow: 0 10px 25px rgba(0,0,0,0.08);
}

th, td {
  padding: 15px;
  text-align: center;
}

th {
  background: #38bdf8;
  color: #0f172a;
}

tr:nth-child(even) {
  background: #f1f5f9;
}

/* Services Section */
.services {
  display: flex;
  justify-content: center;
  gap: 25px;
  padding: 50px;
  flex-wrap: wrap;
}

.card {
  background: white;
  width: 260px;
  padding: 25px;
  text-align: center;
  border-radius: 12px;
  box-shadow: 0 10px 25px rgba(0,0,0,0.08);
  transition: transform 0.3s, box-shadow 0.3s;
}

.card:hover {
  transform: translateY(-8px);
  box-shadow: 0 15px 35px rgba(0,0,0,0.15);
}

.card img {
  width: 100%;
  height: 130px;
  background: #e2e8f0;
  border-radius: 8px;
  margin-bottom: 15px;
}

.card button {
  background: #38bdf8;
  color: #0f172a;
  border: none;
  padding: 12px 18px;
  border-radius: 6px;
  cursor: pointer;
  font-weight: bold;
  transition: background 0.3s;
}

.card button:hover {
  background: #0ea5e9;
  color: white;
}

/* Contact Form */
form {
  width: 40%;
  margin: 50px auto;
  background: white;
  padding: 30px;
  border-radius: 12px;
  box-shadow: 0 10px 25px rgba(0,0,0,0.08);
}

label {
  font-weight: bold;
  margin-bottom: 6px;
  display: block;
}

input, textarea {
  width: 100%;
  padding: 12px;
  margin-bottom: 18px;
  border-radius: 6px;
  border: 1px solid #cbd5f5;
  font-size: 15px;
}

button[type="submit"] {
  background: #38bdf8;
  color: #0f172a;
  border: none;
  padding: 14px;
  font-size: 16px;
  border-radius: 6px;
  cursor: pointer;
  font-weight: bold;
}





