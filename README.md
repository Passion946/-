:root {
  --primary-purple: #a34f9c;
  --primary-blue: #393d96;
  --primary-yellow: #f5ed29;
  --font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
}

* {
  box-sizing: border-box;
}

body {
  margin: 0;
  font-family: var(--font-family);
  background-color: #fff;
  color: var(--primary-blue);
  line-height: 1.6;
}

.container {
  width: 90%;
  max-width: 1200px;
  margin: auto;
}

header {
  background-color: var(--primary-purple);
  color: white;
  padding: 15px 0;
}

header .container {
  display: flex;
  align-items: center;
  justify-content: space-between;
}

.logo {
  font-size: 1.8rem;
  font-weight: bold;
}

nav ul {
  list-style: none;
  padding: 0;
  margin: 0;
  display: flex;
}

nav ul li {
  margin-left: 20px;
}

nav ul li a {
  color: white;
  text-decoration: none;
  font-weight: 600;
  transition: color 0.3s ease;
}

nav ul li a:hover,
nav ul li a.active {
  color: var(--primary-yellow);
}

.lang-switcher button {
  background: none;
  border: none;
  color: white;
  font-weight: 600;
  margin-left: 10px;
  cursor: pointer;
  padding: 5px 10px;
  border-radius: 3px;
  transition: background-color 0.3s ease;
}

.lang-switcher button:hover,
.lang-switcher button.active {
  background-color: var(--primary-yellow);
  color: var(--primary-purple);
}

main {
  padding: 30px 0;
}

h1, h2, h3 {
  color: var(--primary-purple);
}

.hero {
  text-align: center;
  padding: 60px 20px;
  background-color: #f7f7f7;
  border-radius: 8px;
}

.services-overview {
  margin-top: 50px;
}

.services-list {
  display: flex;
  justify-content: space-between;
  flex-wrap: wrap;
  gap: 20px;
}

.service-item {
  flex: 1 1 30%;
  background-color: #fafafa;
  border: 1px solid #ddd;
  padding: 20px;
  border-radius: 6px;
  text-align: center;
  transition: box-shadow 0.3s ease;
}

.service-item:hover {
  box-shadow: 0 0 15px rgba(163, 79, 156, 0.4);
}

.service-item h3 {
  margin-top: 0;
  margin-bottom: 15px;
}

.service-item a {
  color: var(--primary-yellow);
  font-weight: bold;
  text-decoration: none;
}

.service-item a:hover {
  text-decoration: underline;
}

.clients-preview {
  margin-top: 60px;
  text-align: center;
}

.clients-logos img {
  max-height: 60px;
  margin: 0 15px;
  vertical-align: middle;
}

.news-preview {
  margin-top: 60px;
}

.news-preview ul {
  list-style: none;
  padding: 0;
}

.news-preview ul li {
  margin-bottom: 10px;
}

.news-preview ul li a {
  color: var(--primary-blue);
  text-decoration: none;
  font-weight: 600;
}

.news-preview ul li a:hover {
  color: var(--primary-purple);
}

.behind-scenes-preview {
  margin-top: 60px;
  text-align: center;
}

.behind-images img {
  max-width: 150px;
  margin: 10px;
  border-radius: 6px;
  transition: transform 0.3s ease;
  cursor: pointer;
}

.behind-images img:hover {
  transform: scale(1.05);
}

footer {
  background-color: var(--primary-purple);
  color: white;
  text-align: center;
  padding: 15px 0;
  margin-top: 40px;
  font-size: 0.9rem;
}

/* Responsive */

@media (max-width: 768px) {
  nav ul {
    flex-direction: column;
    align-items: flex-start;
  }

  nav ul li {
    margin: 10px 0;
  }

  .services-list {
    flex-direction: column;
  }

  .service-item {
    flex: 1 1 100%;
  }
}
# -
