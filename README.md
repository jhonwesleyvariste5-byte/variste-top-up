<!DOCTYPE html>
<html lang="fr">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Variste Top Up</title>
<style>
*{box-sizing:border-box}
body{
  margin:0;
  font-family:Arial,sans-serif;
  background:#0b1020;
  color:white;
}
header{
  background:#151d35;
  padding:25px 15px;
  text-align:center;
}
header h1{margin:0;font-size:30px}
header p{margin:8px 0 0;color:#b9c2d9}
.container{
  max-width:500px;
  margin:auto;
  padding:20px;
}
.card{
  background:#151d35;
  border-radius:18px;
  padding:20px;
  margin-bottom:18px;
}
h2{margin-top:0}
label{
  display:block;
  margin:15px 0 7px;
}
input,select{
  width:100%;
  padding:14px;
  border-radius:10px;
  border:1px solid #394565;
  background:#0d1428;
  color:white;
  font-size:16px;
}
button{
  width:100%;
  margin-top:20px;
  padding:15px;
  border:0;
  border-radius:10px;
  background:#16c784;
  color:white;
  font-size:17px;
  font-weight:bold;
}
.info{
  line-height:1.6;
  color:#d5dbea;
}
footer{
  text-align:center;
  padding:25px;
  color:#8993ad;
}
</style>
</head>

<body>

<header>
  <h1>💎 VARISTE TOP UP</h1>
  <p>Recharge Free Fire rapidement et facilement</p>
</header>

<div class="container">

  <div class="card">
    <h2>🔥 Recharge Free Fire</h2>

    <label>ID du joueur</label>
    <input type="text" id="player" placeholder="Entre ton ID Free Fire">

    <label>Choisir les diamants</label>
    <select id="diamonds">
      <option>100 Diamants</option>
      <option>310 Diamants</option>
      <option>520 Diamants</option>
      <option>1060 Diamants</option>
      <option>2180 Diamants</option>
      <option>5600 Diamants</option>
    </select>

    <label>Nom du client</label>
    <input type="text" id="name" placeholder="Ton nom">

    <button onclick="order()">Commander maintenant</button>
  </div>

  <div class="card">
    <h2>📌 Comment ça marche ?</h2>
    <div class="info">
      1. Entre ton ID Free Fire.<br>
      2. Choisis le nombre de diamants.<br>
      3. Entre ton nom.<br>
      4. Envoie ta commande pour confirmation.
    </div>
  </div>

</div>

<footer>
  © 2026 Variste Top Up — Tous droits réservés
</footer>

<script>
function order(){
  let player = document.getElementById("player").value;
  let diamonds = document.getElementById("diamonds").value;
  let name = document.getElementById("name").value;

  if(player === "" || name === ""){
    alert("Veuillez remplir votre ID Free Fire et votre nom.");
    return;
  }

  alert(
    "Commande enregistrée !\n\n" +
    "Client : " + name + "\n" +
    "ID : " + player + "\n" +
    "Diamants : " + diamonds
  );
}
</script>

</body>
</html>
