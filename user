<!DOCTYPE html>
<html lang="vi">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>PId - Trang Chủ</title>
  <style>
    body {
      margin: 0;
      font-family: 'Segoe UI', sans-serif;
      background-color: #fefefe;
    }
    header {
      background-color: #fff;
      padding: 1rem 2rem;
      display: flex;
      justify-content: space-between;
      align-items: center;
      box-shadow: 0 2px 4px rgba(0,0,0,0.1);
    }
    .logo {
      font-size: 1.5rem;
      font-weight: bold;
      color: #ff6b81;
    }
    .menu {
      position: relative;
    }
    .menu-button {
      background-color: #ff6b81;
      color: white;
      border: none;
      padding: 0.5rem 1rem;
      border-radius: 5px;
      cursor: pointer;
      font-size: 1rem;
    }
    .dropdown-content {
      display: none;
      position: absolute;
      right: 0;
      background-color: white;
      box-shadow: 0 4px 8px rgba(0,0,0,0.15);
      border-radius: 6px;
      margin-top: 0.5rem;
      z-index: 100;
    }
    .dropdown-content a {
      display: block;
      padding: 0.75rem 1rem;
      text-decoration: none;
      color: #333;
    }
    .dropdown-content a:hover {
      background-color: #f5f5f5;
    }
    .dropdown-content.show {
      display: block;
    }
    main {
      text-align: center;
      padding: 4rem 2rem;
    }
    h1 {
      font-size: 2.5rem;
      color: #333;
    }
    p {
      font-size: 1.1rem;
      color: #555;
      margin-top: 1rem;
    }
  </style>
</head>
<body>
  <header>
    <div class="logo">🐾 PId</div>
    <div class="menu">
      <button class="menu-button" onclick="toggleDropdown()">Menu ▾</button>
      <div id="dropdown" class="dropdown-content">
        <a href="#about">Thông tin</a>
        <a href="#contact">Liên hệ</a>
        <a href="#download">Tải App</a>
      </div>
    </div>
  </header>

  <main>
    <h1>Chào mừng đến với PId</h1>
    <p>Nền tảng kết nối và chăm sóc thú cưng toàn diện tại Việt Nam.</p>
  </main>

  <script>
    function toggleDropdown() {
      const dropdown = document.getElementById("dropdown");
      dropdown.classList.toggle("show");
    }

    window.addEventListener("click", function(event) {
      const isMenuButton = event.target.closest(".menu-button");
      const dropdown = document.getElementById("dropdown");
      if (!isMenuButton && dropdown.classList.contains("show")) {
        dropdown.classList.remove("show");
      }
    });
  </script>
</body>
</html>
