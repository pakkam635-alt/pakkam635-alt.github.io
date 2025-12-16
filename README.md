<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>School CAS Hub</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>

  <!-- Header -->
  <header>
    <h1>Welcome to Our School CAS Hub</h1>
    <nav>
      <a href="#home">Home</a>
      <a href="#chat">Chat</a>
      <a href="#games">Games</a>
      <a href="#progress">Progress</a>
    </nav>
  </header>

  <!-- Home Section -->
  <section id="home">
    <h2>About the Project</h2>
    <p>This platform showcases student achievements, activities, and engagement through interactive features.</p>
  </section>

  <!-- Chat Section -->
  <section id="chat">
    <h2>Student Chat</h2>
    <div id="chat-box">
      <!-- Messages will appear here -->
    </div>
    <input type="text" id="chat-input" placeholder="Type a message...">
    <button onclick="sendMessage()">Send</button>
  </section>

  <!-- Games Section -->
  <section id="games">
    <h2>Games / Challenges</h2>
    <p>Mini-games and quizzes coming soon!</p>
  </section>

  <!-- Progress Section -->
  <section id="progress">
    <h2>Student Progress</h2>
    <p>Track your activities and achievements here!</p>
  </section>

  <!-- Footer -->
  <footer>
    <p>&copy; 2025 Your School Name. CAS Project.</p>
  </footer>

  <!-- Basic JS for placeholder chat -->
  <script>
    const chatBox = document.getElementById('chat-box');
    const chatInput = document.getElementById('chat-input');

    function sendMessage() {
      const text = chatInput.value.trim();
      if(text === '') return;

      const msg = document.createElement('p');
      msg.textContent = text;
      chatBox.appendChild(msg);

      chatInput.value = '';
      chatBox.scrollTop = chatBox.scrollHeight;
    }
  </script>
</body>
</html>
