<html lang="vi">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>PId - Trang Chủ</title>
  <style>
    body {
      margin: 0;
      font-family: 'Segoe UI', sans-serif;
      background-color: #fff9f9;
    }
    header {
      background-color: #ffffff;
      padding: 1rem 2rem;
      display: flex;
      justify-content: space-between;
      align-items: center;
      box-shadow: 0 2px 8px rgba(0,0,0,0.1);
      position: sticky;
      top: 0;
      z-index: 1000;
    }
    .logo {
      font-size: 1.7rem;
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
      padding: 0.6rem 1.2rem;
      border-radius: 30px;
      cursor: pointer;
      font-size: 1rem;
      transition: background-color 0.3s ease;
    }
    .menu-button:hover {
      background-color: #ff4f6e;
    }
    .dropdown-content {
      display: none;
      position: absolute;
      right: 0;
      background-color: white;
      box-shadow: 0 8px 16px rgba(0,0,0,0.15);
      border-radius: 8px;
      margin-top: 0.5rem;
      z-index: 100;
      min-width: 160px;
    }
    .dropdown-content a {
      display: block;
      padding: 0.75rem 1rem;
      text-decoration: none;
      color: #333;
      font-weight: 500;
    }
    .dropdown-content a:hover {
      background-color: #ffecef;
    }
    .show {
      display: block;
    }
    main {
      text-align: center;
      padding: 5rem 2rem;
    }
    h1 {
      font-size: 2.7rem;
      color: #333;
      margin-bottom: 1rem;
    }
    p {
      font-size: 1.2rem;
      color: #555;
      max-width: 600px;
      margin: 0 auto;
    }
    footer {
      background-color: #fef2f2;
      padding: 1rem 2rem;
      text-align: center;
      font-size: 0.95rem;
      color: #888;
      margin-top: 4rem;
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
    <p>Nền tảng kết nối và chăm sóc thú cưng toàn diện tại Việt Nam. Tại đây, bạn có thể tìm kiếm dịch vụ, sản phẩm và cộng đồng cho thú cưng của mình một cách dễ dàng và tiện lợi.</p>
  </main>

  <footer>
    © 2025 PId Platform. Tất cả các quyền được bảo lưu.
  </footer>

  <script>
    function toggleDropdown() {
      document.getElementById("dropdown").classList.toggle("show");
    }
    window.onclick = function(event) {
      if (!event.target.matches('.menu-button')) {
        var dropdowns = document.getElementsByClassName("dropdown-content");
        for (var i = 0; i < dropdowns.length; i++) {
          var openDropdown = dropdowns[i];
          if (openDropdown.classList.contains('show')) {
            openDropdown.classList.remove('show');
          }
        }
      }
    }
  </script>
</body>
</html>
