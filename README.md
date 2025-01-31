```
<!DOCTYPE html>
<html>
<head>
<title>Dribbble Clone</title>
<style>
body {
  font-family: sans-serif;
  margin: 0;
}

header {
  background-color: #333;
  color: #166361;
  padding: 1em;
}

nav {
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.logo {
  font-size: 2em;
  font-weight: bold;
  text-decoration: none;
  color: #230404d6;
}

.nav-links {
  display: flex;
  list-style: none;
  margin: 0;
  padding: 0;
}

.nav-links li {
  margin-right: 1em;
}

.nav-links a {
  color: #e5e0e0;
  text-decoration: none;
}

.nav-links a:hover {
  text-decoration: underline;
}

.search-bar {
  display: flex;
  align-items: center;
}

.search-bar input {
  padding: 0.5em;
  border: none;
  border-radius: 5px;
}

.search-bar button {
  padding: 0.5em 1em;
  border: none;
  border-radius: 5px;
  background-color: #fff;
  color: #333;
  cursor: pointer;
}

.hero {
  background-color: #eb3a3a;
  padding: 2em;
  text-align: center;
}

.hero h1 {
  font-size: 2em;
}

.hero p {
  font-size: 1.2em;
  margin-bottom: 1em;
}

.hero button {
  padding: 0.8em 1.5em;
  border: none;
  border-radius: 5px;
  background-color: #333;
  color: #e7f1ef;
  cursor: pointer;
}

.content {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  padding: 2em;
}

.card {
  width: 200px;
  margin: 1em;
  background-color: #b3c2d3;
  border-radius: 5px;
  overflow: hidden;
  box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
  cursor: pointer;
  position: relative; /* For the overlay */
}

.card img {
  width: 100%;
  height: 150px;
  object-fit: cover;
}

.card-content {
  padding: 1em;
}

.card-title {
  font-weight: bold;
  margin-bottom: 0.5em;
}

.card-stats {
  display: flex;
  justify-content: space-between;
  align-items: center;
  color: #5c5858;
  font-size: 0.8em;
}

.card-stats i {
  margin-right: 0.5em;
}

.overlay {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background-color: rgba(0, 0, 0, 0.5);
  color: #fff;
  display: flex;
  justify-content: center;
  align-items: center;
  opacity: 0;
  transition: opacity 0.3s ease-in-out;
}

.card:hover .overlay {
  opacity: 1;
}

.overlay-text {
  font-size: 1.2em;
  font-weight: bold;
}

.pagination {
  display: flex;
  justify-content: center;
  margin-top: 2em;
}

.pagination button {
  padding: 0.5em 1em;
  border: none;
  border-radius: 5px;
  background-color: #333;
  color: #fff;
  cursor: pointer;
  margin: 0 0.5em;
}

.pagination button.active {
  background-color: #fff;
  color: #333;
}

.footer {
  background-color: #333;
  color: #743636;
  padding: 1em;
  text-align: center;
}
</style>
</head>
<body>

<header>
  <nav>
    <a href="#" class="logo">Dribbble</a>
    <ul class="nav-links">
      <li><a href="#">Shots</a></li>
      <li><a href="#">Designers</a></li>
      <li><a href="#">Teams</a></li>
      <li><a href="#">Community</a></li>
      <li><a href="#">Jobs</a></li>
    </ul>
    <div class="search-bar">
      <input type="text" placeholder="Search">
      <button>Search</button>
    </div>
    <div>
      <button>Sign up</button>
      <button>Sign in</button>
    </div>
  </nav>
</header>

<div class="hero">
  <h1>What are you working on?</h1>
  <p>Dribbble is show and tell for designers.</p>
  <button>Learn more</button>
  <button>Sign up</button>
</div>

<div class="content">
  <div class="card">
    <img src="cssadv1.png">
    <div class="card-content">
      <h2 class="card-title">Train</h2>
      <div class="card-stats">
        <i class="fas fa-eye"></i> 4,044
        <i class="fas fa-comments"></i> 14
        <i class="fas fa-heart"></i> 290
      </div>
    </div>
    <div class="overlay">
      <p class="overlay-text">View Project</p>
    </div>
  </div>
  <div class="card">
    <img src="img/cssadv2.png">
    <div class="card-content">
      <h2 class="card-title">Attitude</h2>
      <div class="card-stats">
        <i class="fas fa-eye"></i> 2,404
        <i class="fas fa-comments"></i> 13
        <i class="fas fa-heart"></i> 236
      </div>
    </div>
    <div class="overlay">
      <p class="overlay-text">View Project</p>
    </div>
  </div>
  <div class="card">
    <img src="img/cssadv3.png">
    <div class="card-content">
      <h2 class="card-title">Rum</h2>
      <div class="card-stats">
        <i class="fas fa-eye"></i> 3,985
        <i class="fas fa-comments"></i> 17
        <i class="fas fa-heart"></i> 264
      </div>
    </div>
    <div class="overlay">
      <p class="overlay-text">View Project</p>
    </div>
  </div>
  <div class="card">
    <img src="img/cssadv4.png" alt="Card Image">
    <div class="card-content">
      <h2 class="card-title">Plough</h2>
      <div class="card-stats">
        <i class="fas fa-eye"></i> 2,602
        <i class="fas fa-comments"></i> 23
        <i class="fas fa-heart"></i> 186
      </div>
    </div>
    <div class="overlay">
      <p class="overlay-text">View Project</p>
    </div>
  </div>
  <div class="card">
    <img src="img/cssadv5.png">
    <div class="card-content">
      <h2 class="card-title">Shine</h2>
      <div class="card-stats">
        <i class="fas fa-eye"></i> 2,369
        <i class="fas fa-comments"></i> 8
        <i class="fas fa-heart"></i> 178
      </div>
    </div>
    <div class="overlay">
      <p class="overlay-text">View Project</p>
    </div>
  </div>
  <div class="card">
    <img src="img/cssadv6.png">
    <div class="card-content">
      <h2 class="card-title">Bird</h2>
      <div class="card-stats">
        <i class="fas fa-eye"></i> 2,025
        <i class="fas fa-comments"></i> 6
        <i class="fas fa-heart"></i> 160
      </div>
    </div>
    <div class="overlay">
      <p class="overlay-text">View Project</p>
    </div>
  </div>
  <div class="card">
    <img src="img/cssadv7.png">
    <div class="card-content">
      <h2 class="card-title">Elusive</h2>
      <div class="card-stats">
        <i class="fas fa-eye"></i> 1,841
        <i class="fas fa-comments"></i> 6
        <i class="fas fa-heart"></i> 158
      </div>
    </div>
    <div class="overlay">
      <p class="overlay-text">View Project</p>
    </div>
  </div>
  <div class="card">
    <img src="img/cssadv8.png">
    <div class="card-content">
      <h2 class="card-title">Olympic</h2>
      <div class="card-stats">
        <i class="fas fa-eye"></i> 2,179
        <i class="fas fa-comments"></i> 4
        <i class="fas fa-heart"></i> 158
      </div>
    </div>
    <div class="overlay">
      <p class="overlay-text">View Project</p>
    </div>
  </div>
  <div class="card">
    <img src="img/cssadv9.png">
    <div class="card-content">
      <h2 class="card-title">Interior</h2>
      <div class="card-stats">
        <i class="fas fa-eye"></i> 1,872
        <i class="fas fa-comments"></i> 8
        <i class="fas fa-heart"></i> 148
      </div>
    </div>
    <div class="overlay">
      <p class="overlay-text">View Project</p>
    </div>
  </div>
  <div class="card">
    <img src="img/cssadv10.png">
    <div class="card-content">
      <h2 class="card-title">Routine</h2>
      <div class="card-stats">
        <i class="fas fa-eye"></i> 2,167
        <i class="fas fa-comments"></i> 9
        <i class="fas fa-heart"></i> 134
      </div>
    </div>
    <div class="overlay">
      <p class="overlay-text">View Project</p>
    </div>
  </div>
  <div class="card">
    <img src="img/cssadv11.png">
    <div class="card-content">
      <h2 class="card-title">Vacation</h2>
      <div class="card-stats">
        <i class="fas fa-eye"></i> 1,371
        <i class="fas fa-comments"></i> 9
        <i class="fas fa-heart"></i> 127
      </div>
    </div>
    <div class="overlay">
      <p class="overlay-text">View Project</p>
    </div>
  </div>
  <div class="card">
    <img src="img/cssadv12.png">
    <div class="card-content">
      <h2 class="card-title">SIMMS</h2>
      <div class="card-stats">
        <i class="fas fa-eye"></i> 728
        <i class="fas fa-comments"></i> 3
        <i class="fas fa-heart"></i> 118
      </div>
    </div>
    <div class="overlay">
      <p class="overlay-text">View Project</p>
    </div>
  </div>
  <div class="card">
    <img src="img/cssadv13.png">
    <div class="card-content">
      <h2 class="card-title">landscape</h2>
      <div class="card-stats">
        <i class="fas fa-eye"></i> 1,027
        <i class="fas fa-comments"></i> 6
        <i class="fas fa-heart"></i> 129
      </div>
    </div>
    <div class="overlay">
      <p class="overlay-text">View Project</p>
    </div>
  </div>
  <div class="card">
    <img src="img/cssadv14.png">
    <div class="card-content">
      <h2 class="card-title">Man</h2>
      <div class="card-stats">
        <i class="fas fa-eye"></i> 1,553
        <i class="fas fa-comments"></i> 9
        <i class="fas fa-heart"></i> 112
      </div>
    </div>
    <div class="overlay">
      <p class="overlay-text">View Project</p>
    </div>
  </div>
  <div class="card">
    <img src="img/cssadv15.png">
    <div class="card-content">
      <h2 class="card-title">Super Women</h2>
      <div class="card-stats">
        <i class="fas fa-eye"></i> 940
        <i class="fas fa-comments"></i> 9
        <i class="fas fa-heart"></i> 107
      </div>
    </div>
    <div class="overlay">
      <p class="overlay-text">View Project</p>
    </div>
  </div>
  <div class="card">
    <img src="img/cssadv16.png">
    <div class="card-content">
      <h2 class="card-title">Car</h2>
      <div class="card-stats">
        <i class="fas fa-eye"></i> 1,177
        <i class="fas fa-comments"></i> 4
        <i class="fas fa-heart"></i> 102
      </div>
    </div>
    <div class="overlay">
      <p class="overlay-text">View Project</p>
    </div>
  </div>
  <div class="card">
    <img src="img/cssadv17.png">
    <div class="card-content">
      <h2 class="card-title">Puppy</h2>
      <div class="card-stats">
        <i class="fas fa-eye"></i> 1,100
        <i class="fas fa-comments"></i> 6
        <i class="fas fa-heart"></i> 93
      </div>
    </div>
    <div class="overlay">
      <p class="overlay-text">View Project</p>
    </div>
  </div>
  <div class="card">
    <img src="img/cssadv18.png">
    <div class="card-content">
      <h2 class="card-title">Violin</h2>
      <div class="card-stats">
        <i class="fas fa-eye"></i> 1,445
        <i class="fas fa-comments"></i> 5
        <i class="fas fa-heart"></i> 101
      </div>
    </div>
    <div class="overlay">
      <p class="overlay-text">View Project</p>
    </div>
  </div>
</div>

<div class="pagination">
  <button class="active">1</button>
  <button>2</button>
  <button>3</button>
  <button>4</button>
  <button>5</button>
</div>

<footer class="footer">
  <p>&copy; 2023 Dribbble</p>
</footer>

<script src="https://kit.fontawesome.com/your-fontawesome-kit-id.js" crossorigin="anonymous"></script>
</body>
</html>
```
