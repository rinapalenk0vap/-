
<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<meta name="theme-color" content="#ffe5f0">
<title>୨୧ Aplicaciones Coquettes ୨୧</title>

<style>
* { box-sizing: border-box; }

body {
  margin: 0;
  padding: 22px 15px;
  background: #fff4f8;
  color: #80546a;
  font-family: Georgia, serif;
  background-image: radial-gradient(#f2c4d7 1px, transparent 1px);
  background-size: 19px 19px;
}

header {
  background: #ffe2ee;
  border: 2px solid #edbfd3;
  border-radius: 25px;
  text-align: center;
  padding: 28px 12px;
  box-shadow: 0 5px 15px #e8b8ce66;
}

h1 {
  color: #bd7195;
  font-size: 27px;
}

header p { font-style: italic; }

.decor {
  color: #cf8cab;
  letter-spacing: 7px;
  font-size: 22px;
}

h2 {
  color: #bd7195;
  font-size: 19px;
}

main {
  max-width: 650px;
  margin: auto;
}

.card {
  background: #fffafd;
  border: 1px solid #edc5d8;
  border-radius: 19px;
  padding: 18px;
  margin: 17px 0;
  box-shadow: 0 4px 12px #eac5d644;
}

.card button {
  background: #f5d4e3;
  color: #995a7b;
  border: 1px solid #e9b9d0;
  border-radius: 25px;
  padding: 10px 19px;
  font-weight: bold;
  cursor: pointer;
  margin: 5px 5px 0 0;
}

.card button:hover { background: #edc0d5; }

.description {
  font-family: Arial, sans-serif;
  font-size: 14px;
  line-height: 1.6;
}

.details { display: none; }

footer {
  text-align: center;
  padding: 25px;
  color: #c17e9f;
}
</style>
</head>

<body>
<main>

<header>
  <div class="decor">୨୧ ♡ 🎀 ♡ ୨୧</div>
  <h1>APLICACIONES COQUETTES</h1>
  <p>Welcome to my little pink world ♡</p>
  <div class="decor">✧ ˚ · . ⋆｡°✩</div>
</header>

<div id="apps"></div>

<footer>
  ♡ made with love ♡<br>
  ୨୧ your aesthetic collection ୨୧
</footer>

</main>

<script>
const applications = [
  {
    name: "୨୧ Cutiora",
    description: "Edita fotografías con filtros Y2K, efectos Webcore, marcos y stickers.",
    url: "https://cutiora.com/tools/"
  },
  {
    name: "♡ PFP Vibes",
    description: "Crea fotos de perfil, wallpapers, marcos y usernames aesthetic.",
    url: "https://pfpvibes.com/"
  },
  {
    name: "✧ Y2K Photo Collage",
    description: "Crea collages y photcards con detalles de los años 2000.",
    url: "https://y2kphotocollage.com/"
  },
  {
    name: "୨୧ visualOS",
    description: "Organiza imágenes, colores y textos para hacer moodboards.",
    url: "https://visualos.app/moodboard-maker.html"
  },
  {
    name: "♡ Moodboard Fit",
    description: "Organiza ideas de outfits, accesorios y combinaciones.",
    url: "https://moodboardfit.com/"
  },
  {
    name: "✿ MiniMuse",
    description: "Crea personajes, combina prendas y diseña escenas.",
    url: "https://minimuse.online/"
  },
  {
    name: "♡ Fashion Game",
    description: "Diseña ropa, elige telas, colores y estampados.",
    url: "https://dinogame.gg/games/fashion-game/"
  },
  {
    name: "✧ DressUp",
    description: "Explora juegos de moda y estilos alternativos.",
    url: "https://www.dressup.com/fashion"
  }
];

const container = document.getElementById("apps");

applications.forEach((app, index) => {
  const card = document.createElement("section");
  card.className = "card";

  const title = document.createElement("h2");
  title.textContent = app.name;

  const description = document.createElement("p");
  description.className = "description";
  description.textContent = app.description;

  const button = document.createElement("button");
  button.textContent = "♡ VER PARA QUÉ SIRVE";

  const details = document.createElement("div");
  details.className = "details";

  const open = document.createElement("button");
  open.textContent = "✧ ABRIR PÁGINA";
  open.addEventListener("click", () => {
    window.open(app.url, "_blank", "noopener");
  });

  button.addEventListener("click", () => {
    details.style.display =
      details.style.display === "block" ? "none" : "block";
  });

  details.appendChild(description);
  details.appendChild(open);

  card.appendChild(title);
  card.appendChild(button);
  card.appendChild(details);

  container.appendChild(card);
});
</script>

</body>
</html>
