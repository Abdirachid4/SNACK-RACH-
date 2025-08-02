<!DOCTYPE html>
<html lang="fr">
<head>
  <meta charset="UTF-8">
  <title>Restaurant Djiboutien</title>
  <style>
    body { font-family: Arial; padding: 20px; background: #f7f7f7; }
    h1 { text-align: center; }
    .menu-item { border: 1px solid #ccc; margin: 10px; padding: 10px; background: #fff; }
    img { width: 150px; height: 100px; object-fit: cover; }
    .menu { display: flex; flex-wrap: wrap; justify-content: space-around; }
    .btn { margin-top: 20px; display: block; padding: 10px; background: green; color: #fff; text-align: center; text-decoration: none; }
  </style>
</head>
<body>

<h1>Restaurant Djiboutien</h1>

<form id="orderForm">
  <div class="menu" id="menuList"></div>
  <a id="whatsappLink" class="btn" href="#" target="_blank">Commander via WhatsApp</a>
</form>

<script>
  const menuItems = [
    { name: 'Skoudehkaris', price: 1000, img: 'https://via.placeholder.com/150?text=Skoudehkaris' },
    { name: 'Fah-fah', price: 1200, img: 'https://via.placeholder.com/150?text=Fah-Fah' },
{ name: 'Laxoox', price: 700, img: 'https://via.placeholder.com/150?text=Laxoox' },
    { name: 'Canjeero', price: 600, img: 'https://via.placeholder.com/150?text=Canjeero' },
    { name: 'Sambusa', price: 500, img: 'https://via.placeholder.com/150?text=Sambusa' },
    { name: 'Bariis', price: 900, img: 'https://via.placeholder.com/150?text=Bariis' },
    { name: 'Maraq', price: 950, img: 'https://via.placeholder.com/150?text=Maraq' },
    { name: 'Cambuulo', price: 800, img: 'https://via.placeholder.com/150?text=Cambuulo' },
    { name: 'Suqaar', price: 1300, img: 'https://via.placeholder.com/150?text=Suqaar' },
    { name: 'Kac-kac', price: 400, img: 'https://via.placeholder.com/150?text=Kac-kac' },
    { name: 'Mishari', price: 950, img: 'https://via.placeholder.com/150?text=Mishari' },
    { name: 'Anjero malab', price: 650, img: 'https://via.placeholder.com/150?text=Anjero' },
    { name: 'Buskud', price: 450, img: 'https://via.placeholder.com/150?text=Buskud' },
    { name: 'Hilib ari', price: 1500, img: 'https://via.placeholder.com/150?text=Hilib+Ari' },
    { name: 'Digaag duban', price: 1400, img: 'https://via.placeholder.com/150?text=Digaag' },
    { name: 'Macsharo', price: 1000, img: 'https://via.placeholder.com/150?text=Macsharo' },
{ name: 'Soor', price: 850, img: 'https://via.placeholder.com/150?text=Soor' },
    { name: 'Couscous', price: 1100, img: 'https://via.placeholder.com/150?text=Couscous' },
    { name: 'Chips viande', price: 1000, img: 'https://via.placeholder.com/150?text=Chips+Viande' },
    { name: 'Pizza djiboutienne', price: 1600, img: 'https://via.placeholder.com/150?text=Pizza' },
    { name: 'Coca-Cola', price: 300, img: 'https://via.placeholder.com/150?text=Coca' },
    { name: 'Fanta', price: 300, img: 'https://via.placeholder.com/150?text=Fanta' },
    { name: 'Sprite', price: 300, img: 'https://via.placeholder.com/150?text=Sprite' },
    { name: 'Boisson Dimi', price: 250, img: 'https://via.placeholder.com/150?text=Dimi' },
    { name: 'Jus naturel', price: 400, img: 'https://via.placeholder.com/150?text=Jus' }
  ];

  const menuList = document.getElementById("menuList");

  menuItems.forEach((item, index) => {
    const div = document.createElement("div");
    div.className = "menu-item";
    div.innerHTML = `
      <img src="item.img" alt="{item.name}">
      <h3>item.name</h3>
      <p>Prix:{item.price} FDJ</p>
      <label>Quantité: <input type="number" min="0" value="0" id="qty-${index}" /></label>
    `;
    menuList.appendChild(div);
  });document.getElementById("whatsappLink").addEventListener("click", function () 
    let message = "Commande du client:
    let total = 0;
    menuItems.forEach((item, i) => 
      const qty = parseInt(document.getElementById(`qty-{i}`).value);
      if (qty > 0) {
        message += `- item.name x{qty} = qty * item.price FDJ
        total += qty * item.price;
      );
    message += `{total} FDJ`;
    const phone = "25377552642";
    this.href = `https://wa.me/phone?text={message}`;
  });
</script>

</body>
</html>
```# RESTOWA
QUALITÉS,RAPIDITÉ,EFFICACITÉ 
