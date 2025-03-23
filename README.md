# agnecy2
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>ExploreWorld Travel Agency</title>
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;700&display=swap" rel="stylesheet">
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      font-family: 'Inter', sans-serif;
    }
    body {
      line-height: 1.6;
      background-color: #ffffff;
      color: #003366;
    }
    header {
      background: url('https://source.unsplash.com/1600x600/?travel,beach') center/cover no-repeat;
      height: 600px;
      color: white;
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      text-shadow: 1px 1px 5px rgba(0,0,0,0.6);
    }
    header h1 {
      font-size: 4rem;
      margin-bottom: 10px;
      background-color: rgba(0, 51, 102, 0.6);
      padding: 10px 20px;
      border-radius: 5px;
    }
    header p {
      font-size: 1.5rem;
      background-color: rgba(255, 223, 0, 0.7);
      color: #003366;
      padding: 8px 16px;
      border-radius: 5px;
    }
    nav {
      background: #003366;
      padding: 15px 40px;
      display: flex;
      justify-content: space-between;
      align-items: center;
      position: sticky;
      top: 0;
      z-index: 1000;
    }
    nav a {
      margin: 0 15px;
      text-decoration: none;
      color: #ffdd00;
      font-weight: 500;
    }
    nav div:first-child {
      color: #ffffff;
      font-weight: bold;
    }
    section {
      padding: 60px 40px;
    }
    .services, .destinations {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 30px;
    }
    .card {
      background: #e6f0ff;
      border-radius: 10px;
      padding: 20px;
      box-shadow: 0 5px 15px rgba(0,0,0,0.05);
      text-align: center;
    }
    .card h3 {
      color: #003366;
    }
    .cta {
      text-align: center;
      background-color: #ffdd00;
      color: #003366;
      padding: 40px 20px;
      border-radius: 10px;
      margin: 60px auto;
    }
    .cta h2 {
      margin-bottom: 15px;
    }
    .cta button {
      margin-top: 20px;
      padding: 12px 25px;
      font-size: 1rem;
      background: #003366;
      color: #ffffff;
      border: none;
      border-radius: 5px;
      cursor: pointer;
    }
    footer {
      background: #003366;
      color: white;
      padding: 30px 40px;
      display: flex;
      justify-content: space-between;
      flex-wrap: wrap;
    }
    footer div {
      margin-bottom: 20px;
    }
    footer a {
      color: #ffdd00;
      text-decoration: none;
      display: block;
      margin-top: 5px;
    }
    .carousel {
      display: flex;
      overflow-x: auto;
      scroll-snap-type: x mandatory;
      gap: 20px;
      padding: 20px 0;
    }
    .carousel img {
      height: 300px;
      border-radius: 10px;
      scroll-snap-align: start;
    }
    form {
      background: #e6f0ff;
      padding: 40px;
      border-radius: 10px;
      max-width: 600px;
      margin: 0 auto;
    }
    form input, form textarea, form button {
      display: block;
      width: 100%;
      margin-bottom: 20px;
      padding: 10px;
      border: 1px solid #ccc;
      border-radius: 5px;
      font-size: 1rem;
    }
    form button {
      background-color: #003366;
      color: white;
      font-weight: bold;
      cursor: pointer;
    }
    #map {
      height: 300px;
      width: 100%;
      border-radius: 10px;
      margin-top: 40px;
    }
  </style>
</head>
<body>
  <nav>
    <div><strong>ExploreWorld</strong></div>
    <div>
      <a href="#about">About</a>
      <a href="#destinations">Destinations</a>
      <a href="#packages">Packages</a>
      <a href="#contact">Contact</a>
    </div>
  </nav>

  <header>
    <h1>Discover Your Next Adventure</h1>
    <p>Tailor-made tours and experiences worldwide</p>
  </header>

  <section id="about">
    <h2>Who We Are</h2>
    <p>ExploreWorld is a trusted tourism agency with a passion for helping travelers discover new cultures, beautiful landscapes, and unforgettable memories. From planning to booking, we handle everything.</p>
  </section>

  <section id="carousel">
    <h2>Gallery</h2>
    <div class="carousel">
      <img src="https://source.unsplash.com/600x300/?travel1" alt="slide 1">
      <img src="https://source.unsplash.com/600x300/?travel2" alt="slide 2">
      <img src="https://source.unsplash.com/600x300/?travel3" alt="slide 3">
    </div>
  </section>

  <section id="destinations">
    <h2>Top Destinations</h2>
    <div class="destinations">
      <div class="card">
        <h3>Paris</h3>
        <p>Romantic getaways and historical tours in the City of Light.</p>
      </div>
      <div class="card">
        <h3>Bali</h3>
        <p>Tropical paradise with spiritual vibes and white-sand beaches.</p>
      </div>
      <div class="card">
        <h3>Morocco</h3>
        <p>Explore the colorful souks and majestic deserts of North Africa.</p>
      </div>
    </div>
  </section>

  <section id="packages">
    <h2>Popular Packages</h2>
    <div class="services">
      <div class="card">
        <h3>7-Day Europe Highlights</h3>
        <p>Paris, Amsterdam, and Rome – a whirlwind tour with everything included.</p>
      </div>
      <div class="card">
        <h3>Family Fun in Dubai</h3>
        <p>Desert safaris, theme parks, and luxury hotels for all ages.</p>
      </div>
      <div class="card">
        <h3>Greek Island Cruise</h3>
        <p>Hop between Santorini, Mykonos, and Crete in style and comfort.</p>
      </div>
    </div>
  </section>

  <div class="cta">
    <h2>Ready to Plan Your Trip?</h2>
    <p>Contact our travel experts now for a custom quote and itinerary!</p>
    <button>Get Started</button>
  </div>

  <section id="contact">
    <h2>Contact Us</h2>
    <form>
      <input type="text" placeholder="Your Name" required>
      <input type="email" placeholder="Your Email" required>
      <textarea rows="5" placeholder="Tell us about your dream trip..." required></textarea>
      <button type="submit">Send Message</button>
    </form>
    <div id="map"></div>
  </section>

  <footer>
    <div>
      <h3>ExploreWorld</h3>
      <p>Your gateway to global adventures.</p>
    </div>
    <div>
      <h4>Quick Links</h4>
      <a href="#about">About</a>
      <a href="#destinations">Destinations</a>
      <a href="#packages">Packages</a>
      <a href="#contact">Contact</a>
    </div>
    <div>
      <h4>Contact Info</h4>
      <p>Email: info@exploreworld.com</p>
      <p>Phone: +1 234 567 890</p>
    </div>
  </footer>

  <!-- Google Maps Embed -->
  <script>
    function initMap() {
      var location = { lat: 40.7128, lng: -74.0060 };
      var map = new google.maps.Map(document.getElementById('map'), {
        zoom: 10,
        center: location
      });
      var marker = new google.maps.Marker({position: location, map: map});
    }
  </script>
  <script async defer src="https://maps.googleapis.com/maps/api/js?key=YOUR_API_KEY&callback=initMap"></script>

  <!-- Simple Chatbot Widget -->
  <script>
    window.addEventListener('load', function() {
      var chatbot = document.createElement('div');
      chatbot.style.position = 'fixed';
      chatbot.style.bottom = '20px';
      chatbot.style.right = '20px';
      chatbot.style.background = '#003366';
      chatbot.style.color = 'white';
      chatbot.style.padding = '15px';
      chatbot.style.borderRadius = '10px';
      chatbot.style.cursor = 'pointer';
      chatbot.textContent = 'Need help? Chat with us!';
      chatbot.onclick = function() {
        alert('Chatbot coming soon!');
      };
      document.body.appendChild(chatbot);
    });
  </script>
</body>
</html>
