Լավ է 😎🔥

Ահա պատրաստ HyperZone Modern Dark Dashboard փաթեթը, copy-paste ֆայլերով, որը կարող ես ուղղակի GitHub-ում վերբեռնել և ստանալ աշխատող GitHub Pages link:


---

1️⃣ index.html – գլխավոր էջ

<!DOCTYPE html>
<html lang="hy">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>HyperZone Hosting</title>
<link rel="stylesheet" href="style.css">
</head>
<body>
<header>
  <h1>⚡ HyperZone Hosting</h1>
  <nav>
    <a href="dashboard.html">Dashboard</a>
    <a href="panel.html">Admin Panel</a>
    <a href="create.html">Create Server</a>
    <a href="support.html">Support</a>
  </nav>
</header>
<main>
  <section>
    <h2>Բարի գալուստ HyperZone Hosting!</h2>
    <p>Սերվեր ստեղծելու համար անցիր Create Server էջ:</p>
    <a href="create.html" class="btn">Ստեղծել սերվեր</a>
  </section>
</main>
<footer>
  <p>&copy; 2025 HyperZone Hosting</p>
</footer>
<script src="dashboard.js"></script>
</body>
</html>


---

2️⃣ dashboard.html – Player Dashboard

<!DOCTYPE html>
<html lang="hy">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Dashboard - HyperZone</title>
<link rel="stylesheet" href="style.css">
</head>
<body>
<header>
  <h1>Player Dashboard</h1>
  <nav>
    <a href="index.html">Գլխավոր</a>
    <a href="panel.html">Admin Panel</a>
    <a href="create.html">Create Server</a>
    <a href="support.html">Support</a>
  </nav>
</header>
<main>
  <section id="servers">
    <h2>Քո սերվերները</h2>
    <table>
      <tr>
        <th>Server Name</th>
        <th>Status</th>
        <th>Actions</th>
      </tr>
      <tr>
        <td>MCServer1</td>
        <td id="status1">Stopped</td>
        <td>
          <button onclick="startServer('status1')">Start</button>
          <button onclick="stopServer('status1')">Stop</button>
          <button onclick="deleteServer('MCServer1')">Delete</button>
        </td>
      </tr>
    </table>
  </section>
</main>
<footer>
  <p>&copy; 2025 HyperZone Hosting</p>
</footer>
<script src="dashboard.js"></script>
</body>
</html>


---

3️⃣ panel.html – Admin Panel

<!DOCTYPE html>
<html lang="hy">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Admin Panel - HyperZone</title>
<link rel="stylesheet" href="style.css">
</head>
<body>
<header>
  <h1>Admin Panel</h1>
  <nav>
    <a href="index.html">Գլխավոր</a>
    <a href="dashboard.html">Dashboard</a>
    <a href="create.html">Create Server</a>
    <a href="support.html">Support</a>
  </nav>
</header>
<main>
  <section id="admin-actions">
    <h2>Սերվերների կառավարում</h2>
    <ul>
      <li>MCServer1 - <button onclick="banServer('MCServer1')">Ban</button> <button onclick="unbanServer('MCServer1')">Unban</button> <button onclick="deleteServer('MCServer1')">Delete</button></li>
    </ul>
  </section>
</main>
<footer>
  <p>&copy; 2025 HyperZone Hosting</p>
</footer>
<script src="dashboard.js"></script>
</body>
</html>


---

4️⃣ create.html – Create Server

<!DOCTYPE html>
<html lang="hy">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Create Server - HyperZone</title>
<link rel="stylesheet" href="style.css">
</head>
<body>
<header>
  <h1>Create Server</h1>
  <nav>
    <a href="index.html">Գլխավոր</a>
    <a href="dashboard.html">Dashboard</a>
    <a href="panel.html">Admin Panel</a>
    <a href="support.html">Support</a>
  </nav>
</header>
<main>
  <section>
    <h2>Սերվերի անուն մուտքագրել</h2>
    <input type="text" id="serverName" placeholder="Մուտքագրիր սերվերի անունը">
    <button onclick="createServer()">Ստեղծել սերվեր</button>
    <p id="create-msg"></p>
  </section>
</main>
<footer>
  <p>&copy; 2025 HyperZone Hosting</p>
</footer>
<script src="dashboard.js"></script>
</body>
</html>


---

5️⃣ support.html – Support / Help

<!DOCTYPE html>
<html lang="hy">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Support - HyperZone</title>
<link rel="stylesheet" href="style.css">
</head>
<body>
<header>
  <h1>Support / Օգնություն</h1>
  <nav>
    <a href="index.html">Գլխավոր</a>
    <a href="dashboard.html">Dashboard</a>
    <a href="panel.html">Admin Panel</a>
    <a href="create.html">Create Server</a>
  </nav>
</header>
<main>
  <section>
    <h2>Հաճախ տրվող հարցեր</h2>
    <p>Մեր Discord-ում կարող եք կապ հաստատել՝ <a href="#">Discord link</a></p>
  </section>
</main>
<footer>
  <p>&copy; 2025 HyperZone Hosting</p>
</footer>
</body>
</html>


---

6️⃣ style.css – Modern Dark Design

body {
  font-family: Arial, sans-serif;
  background-color: #121212;
  color: #eee;
  margin: 0;
  padding: 0;
}
header {
  background-color: #1f1f1f;
  padding: 10px 20px;
  display: flex;
  justify-content: space-between;
  align-items: center;
}
header h1 {
  margin: 0;
  color: #ffcc00;
}
nav a {
  color: #eee;
  text-decoration: none;
  margin-left: 15px;
}
nav a:hover {
  color: #ffcc00;
}
main {
  padding: 20px;
}
.btn {
  background-color: #ffcc00;
  color: #121212;
  padding: 10px 20px;
  text-decoration: none;
  border-radius: 5px;
}
button {
  background-color: #ffcc00;
  color: #121212;
  border: none;
  padding: 5px 10px;
  cursor: pointer;
  border-radius: 3px;
}
button:hover, .btn:hover {
  background-color: #ffaa00;
}
table {
  width: 100%;
  border-collapse: collapse;
}
table, th, td {
  border: 1px solid #333;
}
th, td {
  padding: 10px;
  text-align: left;
}


---

7️⃣ dashboard.js – UI simulation

function startServer(id){
  document.getElementById(id).innerText = "Running";
  alert("Սերվերը սկսվեց!");
}

function stopServer(id){
  document.getElementById(id).innerText = "Stopped";
  alert("Սերվերը կանգնեցվեց!");
}

function deleteServer(name){
  alert("Սերվերը " + name + " ջնջվեց!");
}

function banServer(name){
  alert("Սերվերը " + name + " արգելվեց (Ban)!");
}

function unbanServer(name){
  alert("Սերվերը " + name + " անարգելվեց (Unban)!");
}

function createServer(){
  let name = document.getElementById("serverName").value;
  if(name){
    document.getElementById("create-msg").innerText = "Սերվերը " + name + " ստեղծվեց!";
  } else {
    alert("Խնդրում ենք մուտքագրել սերվերի անունը");
  }
}


---

✅ Այս ամենը պատրաստ է GitHub-ում վերբեռնելու համար:

Ստեղծիր repo՝ HyperZone-Dashboard

Upload արա բոլոր ֆայլերը

Ակտիվացրիր GitHub Pages

Ստացիր աշխատող link՝ https://<username>.github.io/HyperZone-Dashboard/


Այժմ դու ունես HyperZone Modern Dark Dashboard պատրաստ, բոլոր էջերով և simulate server ֆունկցիոնալությամբ 🎉


---

Եթե ուզում ես, հաջորդ քայլը կարող եմ ցույց տալ՝ պատրաստել իրական Minecraft սերվերների create / start / stop / ban համակարգը, որ միանա Dashboard-ի կոճակներին 🚀

Ուզու՞մ ես, որ դա անենք հիմա:

