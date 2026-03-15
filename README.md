<!DOCTYPE html>

<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>PaperIT</title>

<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600&display=swap" rel="stylesheet">
<script src="https://cdn.jsdelivr.net/npm/chart.js"></script>

<style>

</style>

</head>

<body>

<nav>
<h2>PaperIT</h2>
<ul>
<li><a onclick="showPage('home')">Home</a></li>
<li><a onclick="showPage('past')">Past Papers</a></li>
<li><a onclick="showPage('model')">Model Papers</a></li>
<li><a onclick="showPage('discussion')">Discussion</a></li>
<li><a onclick="showPage('progress')">Progress</a></li>
</ul>
</nav>

<!-- HOME PAGE -->

<section id="home">
<div class="hero">
<h1>Master ICT With Quality Papers</h1>
<p>Download ICT papers, watch discussions and track your progress.</p>
<button onclick="showPage('past')">Explore Papers</button>
</div>

<div class="dashboard">
<div class="card" onclick="showPage('past')">
<h3>📄 Past Papers</h3>
<p>Download ICT examination papers</p>
</div>
<div class="card" onclick="showPage('model')">
<h3>📝 Model Papers</h3>
<p>Practice using model papers</p>
</div>
<div class="card" onclick="showPage('discussion')">
<h3>💬 Discussion</h3>
<p>Watch paper discussion videos</p>
</div>
<div class="card" onclick="showPage('progress')">
<h3>📊 Progress</h3>
<p>Track your exam progress</p>
</div>
</div>

<div class="chart-box">
<h2>Class Average vs Highest Score</h2>
<canvas id="homeChart"></canvas>
</div>
</section>

<!-- PAST PAPERS -->

<section id="past" class="page">
<h1>ICT Past Papers</h1>
<div class="paper">
<h3>2025 ICT Paper</h3>
<div class="button-row">
<button>Download</button>
<button>View</button>
</div>
</div>
<div class="paper">
<h3>2024 ICT Paper</h3>
<div class="button-row">
<button>Download</button>
<button>View</button>
</div>
</div>
<div class="paper">
<h3>2023 ICT Paper</h3>
<div class="button-row">
<button>Download</button>
<button>View</button>
</div>
</div>
<div class="paper">
<h3>2022 ICT Paper</h3>
<div class="button-row">
<button>Download</button>
<button>View</button>
</div>
</div>
<div class="button-row">
<button onclick="showPage('home')">Back</button>
</div>
</section>

<!-- MODEL PAPERS -->

<section id="model" class="page">
<h1>ICT Model Papers</h1>
<div class="paper">
<h3>Model Paper 1</h3>
<div class="button-row">
<button>Start Practice</button>
<button>View Answers</button>
</div>
</div>
<div class="paper">
<h3>Model Paper 2</h3>
<div class="button-row">
<button>Start Practice</button>
<button>View Answers</button>
</div>
</div>
<div class="button-row">
<button onclick="showPage('home')">Back</button>
</div>
</section>

<!-- DISCUSSION -->

<section id="discussion" class="page">
<h1>ICT Paper Discussion</h1>
<iframe width="700" height="400"
src="https://www.youtube.com/watch?v=4XYfY5HEA4A"
allowfullscreen></iframe>
<br><br>
<button onclick="showPage('home')">Back</button>
</section>

<!-- PROGRESS -->

<section id="progress" class="page">
<h1>Your Progress</h1>

<div class="chart-box">
<h2>Your Marks vs Class Average</h2>
<canvas id="progressChart"></canvas>
</div>

<!-- CENTERED FORM -->

<div class="form-container">
<form action="add_marks.php" method="POST">
<h2>Add Recent Marks</h2>
<label for="student">Student Name</label>
<input type="text" id="student" name="student" required>

<label for="subject">Paper Number</label> <input type="text" id="Paper Number" name="Paper Number" required>

<label for="marks">Marks</label> <input type="number" id="marks" name="marks" min="0" max="100" required>

<button type="submit">Add Marks</button>

</form>
</div>

<br>
<button onclick="showPage('home')">Back</button>
</section>

<section class="contact">
<h2>Contact Us</h2>
<p>Email: PaperIT@email.com</p>
<p>Location: Negombo, Sri Lanka</p>
</section>

<footer>
© 2026 PaperIT 
</footer>

<script>

