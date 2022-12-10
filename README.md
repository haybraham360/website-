<!DOCTYPE html>
<html>
<head>
  <title>E-Commerce Website</title>
  <style>
    /* Use a responsive grid layout to make the website look good on all devices */
    .row {
      display: flex;
      flex-wrap: wrap;
    }
    .column {
      flex: 25%;
      padding: 10px;
    }
    /* Style the search bar and search button */
    .search-container {
      display: flex;
      justify-content: center;
      align-items: center;
    }
    .search-bar {
      width: 60%;
      padding: 10px;
      border: 1px solid #ccc;
    }
    .search-button {
      width: 30%;
      padding: 10px;
      background-color: #4CAF50;
      color: white;
      border: 1px solid #ccc;
    }
  </style>
</head>
<body>
  <h1>E-Commerce Website</h1>

  <div class="row">
    <div class="column">
      <h2>Products</h2>
      <ul>
        <li>Product 1: $10</li>
        <li>Product 2: $20</li>
        <li>Product 3: $30</li>
      </ul>
    </div>
    <div class="column">
      <h2>Store Locations</h2>
      <ul>
        <li>Store 1: 123 Main St, Anytown USA</li>
        <li>Store 2: 456 Main St, Anytown USA</li>
        <li>Store 3: 789 Main St, Anytown USA</li>
      </ul>
    </div>
    <div class="column">
      <h2>About Our Stores</h2>
      <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Duis mollis lectus non lorem placerat, eu euismod ante dictum. Mauris sed suscipit dolor.</p>
    </div>
    <div class="column">
      <h2>Search</h2>
      <div class="search-container">
        <input type="text" class="search-bar" placeholder="Search for products...">
        <button class="search-button">Search</button>
      </div>
    </div>
  </div>

  <script>
    // Add a click event listener to the search button that redirects to a Google search
    const searchButton = document.querySelector('.search-button');
    searchButton.addEventListener('click', () => {
      const searchQuery = document.querySelector('.search-bar').value;
      window.location.href = `https://google.com/search?q=${searchQuery}`;
    });
  </script>
</body>
</html>
