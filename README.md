<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Ashyra Reddick – Photography</title>
  <style>
    :root {
      --bg-color: #ffffff;
      --text-color: #000000;
      --accent-color: #d4af37;
      --marble-bg: url('https://www.transparenttextures.com/patterns/marble.png');
    }
    [data-theme="dark"] {
      --bg-color: #121212;
      --text-color: #f5f5f5;
      --accent-color: #d4af37;
    }
    body {
      margin: 0;
      font-family: 'Helvetica Neue', sans-serif;
      background: var(--bg-color) var(--marble-bg);
      color: var(--text-color);
      transition: background 0.3s, color 0.3s;
    }
    header {
      padding: 2rem;
      text-align: center;
      background: var(--bg-color);
      border-bottom: 1px solid #eee;
    }
    header h1 {
      margin: 0;
      font-size: 2.5rem;
      color: var(--accent-color);
    }
    nav {
      margin-top: 1rem;
    }
    nav a {
      margin: 0 1rem;
      text-decoration: none;
      color: var(--text-color);
      font-weight: bold;
    }
    .theme-toggle {
      position: absolute;
      top: 20px;
      right: 20px;
      background: none;
      border: 2px solid var(--accent-color);
      padding: 0.5rem 1rem;
      border-radius: 5px;
      cursor: pointer;
      color: var(--accent-color);
      font-weight: bold;
    }
    section {
      padding: 3rem 2rem;
      max-width: 900px;
      margin: auto;
    }
    .bio, .portfolio, .contact {
      margin-bottom: 3rem;
    }
    .portfolio img {
      max-width: 100%;
      height: auto;
      border: 4px solid var(--accent-color);
      margin-bottom: 1rem;
    }
    form {
      display: flex;
      flex-direction: column;
    }
    form input, form textarea {
      padding: 1rem;
      margin-bottom: 1rem;
      border: 1px solid #ccc;
      border-radius: 5px;
    }
    form button {
      padding: 1rem;
      background: var(--accent-color);
      border: none;
      color: white;
      font-weight: bold;
      cursor: pointer;
    }
    footer {
      text-align: center;
      padding: 2rem;
      font-size: 0.9rem;
      position: relative;
    }
    .camera-sticker {
      width: 60px;
      height: 60px;
      background-image: url('https://cdn-icons-png.flaticon.com/512/3039/3039396.png');
      background-size: cover;
      position: absolute;
      bottom: 10px;
      right: 10px;
      animation: bounce 2s infinite;
    }
    @keyframes bounce {
      0%, 100% { transform: translateY(0); }
      50% { transform: translateY(-10px); }
    }
  </style>
</head>
<body>
  <button class="theme-toggle" onclick="toggleTheme()">Toggle Theme</button>

  <header>
    <h1>Ashyra Reddick</h1>
    <nav>
      <a href="#bio">About</a>
      <a href="#portfolio">Portfolio</a>
      <a href="#contact">Contact</a>
    </nav>
  </header>

  <section id="bio" class="bio">
    <h2>About Me</h2>
    <p>Hello! I'm Ashyra, a passionate photographer who finds beauty in everyday moments. My photography captures mood, light, and authenticity. I specialize in lifestyle and creative portrait work. Welcome to my visual space.</p>
  </section>

  <section id="portfolio" class="portfolio">
    <h2>Portfolio</h2>
    <p>Explore my latest photo work and stories on my blog below:</p>
    <p><a href="https://yourbloglink.com" target="_blank" style="color: var(--accent-color); font-weight: bold;">Visit My Blog →</a></p>
    <img src="https://images.unsplash.com/photo-1519681393784-d120267933ba" alt="Sample Photography"/>
    <img src="https://images.unsplash.com/photo-1504198453319-5ce911bafcde" alt="Sample Photography"/>
  </section>

  <section id="contact" class="contact">
    <h2>Contact Me</h2>
    <form action="mailto:Ashyrareddick04@gmail.com" method="POST" enctype="text/plain">
      <input type="text" name="name" placeholder="Your Name" required />
      <input type="email" name="email" placeholder="Your Email" required />
      <textarea name="message" rows="5" placeholder="Your Message" required></textarea>
      <button type="submit">Send Message</button>
    </form>
  </section>

  <footer>
    <p>&copy; 2025 Ashyra Reddick. All rights reserved. | Email: <a href="mailto:Ashyrareddick04@gmail.com">Ashyrareddick04@gmail.com</a></p>
    <div class="camera-sticker"></div>
  </footer>

  <script>
    function toggleTheme() {
      const html = document.documentElement;
      const current = html.getAttribute('data-theme');
      if (current === 'dark') {
        html.removeAttribute('data-theme');
      } else {
        html.setAttribute('data-theme', 'dark');
      }
    }
  </script>
</body>
</html>