# DARKLAND
WEBSITE 
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>DALKLAND - Gateway to Digital Wonders</title>
  <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@400;600;700&display=swap" rel="stylesheet">
  <style>
    * { margin: 0; padding: 0; box-sizing: border-box; font-family: 'Montserrat', sans-serif; }
    body { background: linear-gradient(to right, #fdfcfb, #e2d1c3); color: #333; line-height: 1.6; transition: all 0.3s ease; }
    header {
      background-color: #2c3e50; color: white; position: relative; text-align: center;
    }
    header img.banner { width: 100%; height: auto; max-height: 180px; object-fit: cover; }
    .login-btn {
      position: absolute; top: 15px; right: 130px;
      background-color: #e67e22; color: white; border: none;
      padding: 0.5rem 1rem; border-radius: 8px; cursor: pointer;
    }
    .profile-display {
      position: absolute; top: 15px; right: 30px; display: flex; align-items: center;
    }
    .profile-display img {
      width: 40px; height: 40px; border-radius: 50%; margin-right: 8px;
    }
    .profile-display span {
      color: #fff; font-weight: bold;
    }
    nav {
      background-color: #34495e; padding: 1rem;
      display: flex; justify-content: center; gap: 1.5rem; flex-wrap: wrap;
    }
    nav a {
      color: white; text-decoration: none; font-weight: bold;
    }
    nav a:hover { text-decoration: underline; }
    .hero {
      padding: 3rem 2rem; background-color: #ecf0f1; text-align: center;
    }
    .hero h1 { font-size: 3rem; color: #2c3e50; }
    .hero p { font-size: 1.2rem; margin-top: 1rem; }
    .features, .profile, .contact-form, .blog, .admin-dashboard, .reviews {
      display: grid; grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
      gap: 1.5rem; padding: 2rem;
    }
    .feature-box, .contact-box, .profile-box, .blog-box, .admin-box, .review-box {
      background: white; padding: 1.5rem; border-radius: 10px;
      box-shadow: 0 4px 12px rgba(0,0,0,0.1); text-align: center;
    }
    .gallery { padding: 2rem; background-color: #f9f9f9; }
    .gallery-images {
      display: flex; flex-wrap: wrap; gap: 1rem; justify-content: center;
    }
    .gallery-images img {
      width: 260px; height: 180px; object-fit: cover; border-radius: 12px;
      box-shadow: 0 4px 8px rgba(0,0,0,0.2);
    }
    .music-player { text-align: center; margin: 2rem 0; }
    footer { background-color: #2c3e50; color: white; text-align: center; padding: 2rem; }
    .login-modal, .profile-modal {
      display: none; position: fixed; top: 0; left: 0;
      width: 100%; height: 100%; background: rgba(0,0,0,0.5);
      justify-content: center; align-items: center; z-index: 9999;
    }
    .modal-content {
      background: white; padding: 2rem; border-radius: 10px;
      width: 90%; max-width: 400px; text-align: center;
    }
    .modal-content input, textarea {
      width: 100%; padding: 0.7rem; margin: 0.5rem 0;
      border: 1px solid #ccc; border-radius: 6px;
    }
    .modal-content button {
      margin-top: 1rem; padding: 0.7rem 2rem;
      background: #2980b9; color: white; border: none;
      border-radius: 5px; cursor: pointer;
    }
    .dark-mode-toggle {
      position: fixed; bottom: 20px; right: 20px;
      background: #222; color: white; border: none;
      padding: 0.5rem 1rem; border-radius: 50px;
      cursor: pointer; z-index: 999;
    }
    #chat-box {
      background: white; border: 1px solid #ccc;
      padding: 1rem; max-width: 400px; margin: 2rem auto;
      border-radius: 10px;
    }
    #chat-box textarea {
      width: 100%; padding: 0.5rem; border-radius: 6px;
    }
  </style>
</head>
<body>
  <header>
    <img class="banner" src="https://www.metal-archives.com/images/1/0/5/8/105858_logo.jpg?3927" alt="DALKLAND Banner">
    <button class="login-btn" onclick="document.getElementById('loginModal').style.display='flex'">Login</button>
    <div class="profile-display">
      <img src="https://i.imgur.com/Tfbo3au.jpeg" alt="User">
      <span id="profileName">Guest</span>
    </div>
    <nav>
      <a href="#">Home</a>
      <a href="#features">Features</a>
      <a href="#gallery">Gallery</a>
      <a href="#chat-box">Chat</a>
      <a href="#contact">Contact</a>
      <a href="#profile">Profile</a>
      <a href="#blog">Blog</a>
      <a href="#admin">Admin</a>
      <a href="#reviews">Reviews</a>
    </nav>
  </header>

  <section class="hero">
    <h1>Welcome to DALKLAND</h1>
    <p>Your ultimate destination for digital creativity, community, and innovation.</p>
  </section>

  <section id="features" class="features">
    <div class="feature-box"><h3>Live Chat</h3><p>Instantly connect with others and get help in real-time.</p></div>
    <div class="feature-box"><h3>News Section</h3><p>Stay updated with the latest tech and world news.</p></div>
    <div class="feature-box"><h3>Media Uploads</h3><p>Share your favorite images and videos with the world.</p></div>
    <div class="feature-box"><h3>Theme Switcher</h3><p>Change your site's appearance with a click.</p></div>
    <div class="feature-box"><h3>Custom Profile</h3><p>Edit your display info and personalize your page.</p></div>
    <div class="feature-box"><h3>Blog Publishing</h3><p>Create, edit and share your own posts.</p></div>
  </section>

  <section id="gallery" class="gallery">
    <h2 style="text-align:center; padding-bottom: 1rem;">Gallery</h2>
    <div class="gallery-images">
      <img src="https://i.imgur.com/6ZZw0iT.jpeg" alt="Gallery 1">
      <img src="https://i.imgur.com/wRNq0YN.jpeg" alt="Gallery 2">
      <img src="https://i.imgur.com/MZUV4Bl.jpeg" alt="Gallery 3">
      <img src="https://i.imgur.com/Tfbo3au.jpeg" alt="Gallery 4">
    </div>
  </section>

  <div class="music-player">
    <h3>Background Music</h3>
    <audio controls><source src="https://www.soundhelix.com/examples/mp3/SoundHelix-Song-1.mp3" type="audio/mpeg"></audio>
  </div>

  <div id="chat-box">
    <h3>Live Chat</h3>
    <textarea placeholder="Type your message..."></textarea>
  </div>

  <section id="profile" class="profile">
    <div class="profile-box">
      <h3>Edit Profile</h3>
      <input type="text" id="editName" placeholder="Display Name">
      <input type="text" placeholder="Bio">
      <button onclick="updateProfileName()">Save Changes</button>
    </div>
  </section>

  <section id="contact" class="contact-form">
    <div class="contact-box">
      <h3>Contact Us</h3>
      <input type="text" placeholder="Your Name">
      <input type="email" placeholder="Your Email">
      <textarea placeholder="Message..."></textarea>
      <button onclick="alert('Message sent!')">Send</button>
    </div>
  </section>

  <section id="blog" class="blog">
    <div class="blog-box">
      <h3>Create Blog Post</h3>
      <input type="text" placeholder="Blog Title">
      <textarea placeholder="Write your blog here..."></textarea>
      <button onclick="alert('Blog posted!')">Publish</button>
    </div>
    <div class="blog-box">
      <h3>Latest Blog</h3>
      <p><strong>New Features Launched!</strong> – Check out our new chat, blog, dark mode, and admin section!</p>
    </div>
  </section>

  <section id="admin" class="admin-dashboard">
    <div class="admin-box">
      <h3>Admin Dashboard</h3>
      <p>Total Users: 120</p>
      <p>Total Posts: 35</p>
      <p>System Status: <strong>Online</strong></p>
      <button onclick="alert('Moderation Panel Opened')">Open Moderation Panel</button>
    </div>
  </section>

  <section id="reviews" class="reviews">
    <div class="review-box">
      <h3>User Review</h3>
      <textarea placeholder="Leave your review..."></textarea>
      <button onclick="alert('Review submitted!')">Submit Review</button>
    </div>
    <div class="review-box">
      <h3>Recent Reviews</h3>
      <p><strong>Anna:</strong> Amazing site with loads of features! ⭐⭐⭐⭐⭐</p>
      <p><strong>Mike:</strong> Love the gallery and music! ⭐⭐⭐⭐</p>
    </div>
  </section>

  <footer>
    <p>&copy; 2025 DALKLAND. All rights reserved.</p>
  </footer>

  <button class="dark-mode-toggle" onclick="toggleDarkMode()">Dark Mode</button>

  <div id="loginModal" class="login-modal">
    <div class="modal-content">
      <h2>Login to DALKLAND</h2>
      <input type="text" id="username" placeholder="Username">
      <input type="password" id="password" placeholder="Password">
      <button onclick="loginUser()">Login</button>
      <button onclick="registerUser()">Register</button>
      <p><a href="#" onclick="alert('Reset link sent to your email!')">Forgot password?</a></p>
    </div>
  </div>

  <script>
    const modal = document.getElementById('loginModal');
    window.onclick = function(event) { if (event.target === modal) modal.style.display = 'none'; }

    function loginUser() {
      const user = document.getElementById('username').value;
      const pass = document.getElementById('password').value;
      const savedUser = localStorage.getItem('dalkUser');
      const savedPass = localStorage.getItem('dalkPass');
      if (user === savedUser && pass === savedPass) {
        alert('Login successful!');
        document.getElementById('profileName').innerText = user;
        modal.style.display = 'none';
      } else alert('Invalid credentials. Try again or register.');
    }
    function registerUser() {
      const user = document.getElementById('username').value;
      const pass = document.getElementById('password').value;
      localStorage.setItem('dalkUser', user);
      localStorage.setItem('dalkPass', pass);
      alert('Registration successful!');
    }
    function toggleDarkMode() {
      document.body.classList.toggle('dark-mode');
      if (document.body.classList.contains('dark-mode')) {
        document.body.style.background = '#1e1e1e';
        document.body.style.color = 'white';
      } else {
        document.body.style.background = 'linear-gradient(to right, #fdfcfb, #e2d1c3)';
        document.body.style.color = '#333';
      }
    }
    function updateProfileName() {
      const name = document.getElementById('editName').value;
      if (name) document.getElementById('profileName').innerText = name;
    }
  </script>
</body>
</html>
