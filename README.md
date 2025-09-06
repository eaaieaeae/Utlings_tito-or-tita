<!DOCTYPE html>
<html>
<head>
  <title>Utling Match</title>
  <style>
    body { 
      font-family: Arial, sans-serif; 
      text-align: center; 
      margin-top: 50px; 
      background: #f5f5f5;
    }
    h2 { color: #333; }
    input, button {
      padding: 10px;
      margin: 5px;
      font-size: 1em;
    }
    #result {
      margin-top: 20px;
      font-size: 1.3em;
      font-weight: bold;
      color: #2c3e50;
    }
  </style>
</head>
<body>
  <h2>Find Your Tito/Tita</h2>
  <p>Enter your password to reveal your match:</p>
  <input type="password" id="password" placeholder="Enter password">
  <button onclick="checkPassword()">Submit</button>

  <div id="result"></div>

  <script>
    const pairs = {
      "acusar123": "Cherry Mae A. Acusar → Loyloy, Keven B.",
      "aurora123": "Cathy A. Aurora → Gaila, Kristine Dianale S.",
      "ayala123": "Joy S. Ayala → Amolat, Trexie Dace M.",
      "bual123": "Mary Kyla Odchimar Bual → Suba, Frances Nicole M.",
      "balaan123": "Andy Christian J. Bala-an → Beros, Dareen Joseph J.",
      "bonggo123": "Alexelaine J. Bonggo → Cordova, Jadeail Grace",
      "butac123": "Ritchel C. Butac → Peñaranda, Breanne Chei M.",
      "coronel123": "Dennis Patrick F. Coronel → Cordova, Jadeail Grace",
      "delaserna123": "Arwyn Gabrielle M. Dela Serna → Alutaya, Korfa Anne",
      "egay123": "Jermaine Remone U. Egay → Tabamo, Daphne Jasmine L.",
      "ello123": "Queen Olive F. Ello → Bacasmot, Jezril S.",
      "esteban123": "Jayanna Isabel V. Esteban → Loma, Jhanica Kyle T.",
      "famenia123": "Amabelle Ann S. Famenia → Pamplona, Maria Marsha Angela H.",
      "gagno123": "Guinevere E. Gagno → Maisog, Gerilde D.",
      "gido123": "Jesse Jhane T. Gido → Garcia, Sara Fatima Lynn D.",
      "gocong123": "Sophia Abegail G. Goc-ong → Galapin, Karylle Mae L.",
      "guerrero123": "Angel Yeisha G. Guerrero → Ablir, Ken Cydric F.",
      "jabien123": "Robee Gwyneth P. Jabien → Tan, Yyannah Kiss S.",
      "jalop123": "Alexa Denise G. Jalop → Pawang, Yvonne G.",
      "jamen123": "Ciffryl Josh C. Jamen → Adaya, Larrence Angelou",
      "lua123": "Melody Grace K. Lua → Rodrigo, Jasmine Bridgette H.",
      "lusica123": "John Nestor B. Lusica → Macarayon, Ian Van P.",
      "martizano123": "Kyle Jahazeil S. Martizano → Pador, Kerwyn Rhoy S.",
      "micayabas123": "Yesha Nicole L. Micayabas → Cabahug, Simone Famille L.",
      "nuneza123": "Franz Khate F. Nuñeza → Tablon, Kyle Ian",
      "obre123": "Jessie Claire A. Obre → Espinosa, MJ",
      "pantonial123": "Janine D. Pantonial → Cornell, Christian Aaron",
      "quinanahan123": "Jusse Nathalie O. Quinanahan → Cantero, Ma. Karen",
      "rosal123": "Edrian B. Rosal → Cadungog, Novelles Anne P.",
      "saligue123": "Vince Jeffrey P. Saligue → Punay, Jan Nico O.",
      "salinasal123": "Jhocel Jean Salinasal → Dinopol, Neil Mari A.",
      "silbano123": "Lensam Mae S. Silbano → Prepose, Danna Trisha",
      "tanawon123": "Sakura Tan-awon → Peresores, Yves Francis Dion",
      "vilo123": "JC Fel Anthonia A. Vilo → Amancio, Charm L."
    };

    function checkPassword() {
      const pw = document.getElementById("password").value.toLowerCase();
      const result = document.getElementById("result");
      if (pairs[pw]) {
        result.textContent = pairs[pw];
      } else {
        result.textContent = "❌ Invalid password. Try again.";
      }
    }
  </script>
</body>
</html>
