<!DOCTYPE html>
<html>
<head>
  <title>Smart Task Manager</title>
  <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" />
  <link rel="stylesheet" href="style.css" />
</head>
<body>
  <div class="container mt-5">
    <h1 class="text-center mb-4">Smart Task Manager</h1>
    <div id="authSection">
      <input type="email" id="email" placeholder="Email" class="form-control mb-2" />
      <input type="password" id="password" placeholder="Password" class="form-control mb-2" />
      <button onclick="signUp()" class="btn btn-primary me-2">Sign Up</button>
      <button onclick="login()" class="btn btn-success">Log In</button>
    </div>

    <div id="taskSection" class="d-none mt-4">
      <input type="text" id="taskInput" placeholder="Enter task" class="form-control mb-2" />
      <button onclick="addTask()" class="btn btn-secondary mb-3">Add Task</button>
      <ul id="taskList" class="list-group"></ul>
      <button onclick="logout()" class="btn btn-danger mt-3">Log Out</button>
    </div>
  </div>

  <!-- Firebase -->
  <script src="https://www.gstatic.com/firebasejs/8.6.8/firebase-app.js"></script>
  <script src="https://www.gstatic.com/firebasejs/8.6.8/firebase-auth.js"></script>
  <script src="https://www.gstatic.com/firebasejs/8.6.8/firebase-database.js"></script>
  <script src="script.js"></script>
</body>
</html>
