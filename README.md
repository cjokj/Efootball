<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>eFootball League Results</title>
    <style>
        body { font-family: Arial, sans-serif; text-align: center; }
        table { width: 80%; margin: auto; border-collapse: collapse; }
        th, td { border: 1px solid black; padding: 10px; }
        input, button { margin: 10px; padding: 10px; }
    </style>
</head>
<body>
    <h1>Bangladesh Air Force Shaheen College Chattagram eFootball League</h1>
    <h2>Match Results</h2>
    <table>
        <tr>
            <th>Team 1</th>
            <th>Team 2</th>
            <th>Score</th>
        </tr>
        <tr>
            <td><input type="text" id="team1"></td>
            <td><input type="text" id="team2"></td>
            <td><input type="text" id="score"></td>
        </tr>
    </table>
    <button onclick="saveResult()">Submit Result</button>
    <h2>Qualified Teams</h2>
    <ul id="qualifiedTeams"></ul>

    <script>
        function saveResult() {
            let team1 = document.getElementById('team1').value;
            let team2 = document.getElementById('team2').value;
            let score = document.getElementById('score').value;
            let result = document.createElement('li');
            result.innerText = `${team1} vs ${team2} - Score: ${score}`;
            document.getElementById('qualifiedTeams').appendChild(result);
        }
    </script>
</body>
</html>
# Efootball
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Football Tournament</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <header>
        <h1>Football Tournament</h1>
        <nav>
            <ul>
                <li><a href="#">Home</a></li>
                <li><a href="#">Teams</a></li>
                <li><a href="#">Fixtures</a></li>
                <li><a href="#">Results</a></li>
                <li><a href="#">Contact</a></li>
            </ul>
        </nav>
    </header>

    <section id="intro">
        <h2>Welcome to the Football Tournament</h2>
        <p>Get ready for an exciting football competition among the school teams!</p>
    </section>

    <section id="teams">
        <h2>Teams</h2>
        <div class="team" id="team1">
            <h3>Team 1</h3>
            <button class="view-info">View Info</button>
        </div>
        <div clas
body {
    font-family: Arial, sans-serif;
    background-color: #f4f4f4;
    margin: 0;
    padding: 0;
}

header {
    background-color: #333;
    color: white;
    padding: 10px 0;
    text-align: center;
}

header nav ul {
    list-style: none;
    padding: 0;
}

header nav ul li {
    display: inline;
    margin: 0 10px;
}

header nav ul li a {
    color: white;
    text-decoration: none;
}

section {
    padding: 20px;
    margin: 10px;
}

h2 {
    color: #333;
}

.team {
    background-color: #fff;
    padding: 10px;
    margin: 10px 0;
    border-radius: 8px;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
}

button.view-info {
    background-color: #007BFF;
    color: white;
    border: none;
    padding: 10px 20px;
    cursor: pointer;
}

button.view-info:hover {
    background-color: #0056b3;
}

footer {
    text-align: center;
    background-color: #333;
    color: white;
    padding: 10px;
    position: absolute;
    bottom: 0;
    width: 100%;
}
