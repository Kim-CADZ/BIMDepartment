<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>BIM Department</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background: #f8f9fa;
      color: #333;
      margin: 0;
      display: flex;
      align-items: center;
      justify-content: center;
      height: 100vh;
    }
    .card {
      background: white;
      padding: 30px 40px;
      border-radius: 12px;
      box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
      text-align: center;
    }
    .main-button {
      background-color: #0077b6;
      color: white;
      padding: 12px 20px;
      font-size: 18px;
      border: none;
      border-radius: 8px;
      cursor: pointer;
      margin-bottom: 20px;
      transition: background-color 0.3s;
    }
    .main-button:hover {
      background-color: #005f87;
    }
    .members {
      display: none;
      flex-direction: column;
      gap: 10px;
      margin-top: 10px;
    }
    .member-button {
      background-color: #90e0ef;
      border: none;
      padding: 10px;
      border-radius: 6px;
      font-size: 16px;
      cursor: pointer;
      transition: background-color 0.3s;
    }
    .member-button:hover {
      background-color: #48cae4;
    }
  </style>
</head>
<body>
  <div class="card">
    <button class="main-button" onclick="toggleMembers()">BIM Department</button>
    <div class="members" id="memberButtons">
      <button class="member-button">Hakim</button>
      <button class="member-button">Ingo</button>
      <button class="member-button">Anne-Shirley</button>
    </div>
  </div>

  <script>
    function toggleMembers() {
      const members = document.getElementById('memberButtons');
      members.style.display = (members.style.display === 'flex') ? 'none' : 'flex';
    }
  </script>
</body>
</html>
