# fleuriste
<!DOCTYPE html>
<html lang="fr">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Fleuriste Émeraude</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      background: #fff;
      color: #333;
    }
    header {
      background: #88b04b;
      color: white;
      padding: 2rem;
      text-align: center;
    }
    header h1 {
      margin: 0;
      font-size: 2.5rem;
    }
    nav {
      background: #6b8e23;
      padding: 1rem;
      text-align: center;
    }
    nav a {
      color: white;
      text-decoration: none;
      margin: 0 1rem;
      font-weight: bold;
    }
    nav a:hover {
      text-decoration: underline;
    }
    .hero {
      background: url("https://images.unsplash.com/photo-1509042239860-f550ce710b93") no-repeat center center/cover;
      height: 400px;
      display: flex;
      align-items: center;
      justify-content: center;
      color: white;
      text-shadow: 1px 1px 3px rgba(0,0,0,0.7);
    }
    .hero h2 {
      font-size: 2.5rem;
    }
    .section {
      padding: 3rem 1rem;
      max-width: 1000px;
      margin: auto;
    }
    .section h2 {
      text-align: center;
      color: #6b8e23;
      margin-bottom: 2rem;
    }
    .products {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 2rem;
    }
    .product {
      border: 1px solid #ddd;
      border-radius: 8px;
      overflow: hidden;
      text-align: center;
      box-shadow: 0 2px 6px rgba(0,0,0,0.1);
      padding-bottom: 1rem;
    }
    .product img {
      width: 100%;
      height: 200px;
      object-fit: cover;
    }
    .product h3 {
      margin: 0.5rem 0;
    }
    .product p {
      margin: 0.5rem;
      font-size: 0.9rem;
    }
    .paypal-btn {
      margin-top: 0.5rem;
    }
    .contact {
      text-align: center;
      background: #f9f9f9;
      padding: 2rem;
      border-top: 1px solid #ddd;
    }
    footer {
      text-align: center;
      background: #6b8e23;
      color: white;
      padding: 1rem;
      margin-top: 2rem;
    }
  </style>
</head>
<body>

  <header>
    <h1>Fleuriste Émeraude</h1>
    <p>Des fleurs fraîches pour toutes vos occasions 🌸</p>
  </header>

  <nav>
    <a href="#accueil">Accueil</a>
    <a href="#boutique">Boutique</a>
    <a href="#contact">Contact</a>
  </nav>

  <section class="hero" id="accueil">
    <h2>Égayez votre quotidien avec nos bouquets</h2>
  </section>

  <section class="section" id="boutique">
    <h2>Nos bouquets</h2>
    <div class="products">

      <!-- Produit 1 : Roses -->
      <div class="product">
        <img src="https://images.unsplash.com/photo-1526045612212-70caf35c14df" alt="Bouquet de roses">
        <h3>Bouquet de Roses</h3>
        <p>Un classique romantique, idéal pour offrir.</p>
        <p><strong>35 €</strong></p>
        <form action="https://www.paypal.com/cgi-bin/webscr" method="post" target="_top" class="paypal-btn">
          <input type="hidden" name="cmd" value="_xclick">
          <input type="hidden" name="business" value="ton-email-paypal@exemple.com">
          <input type="hidden" name="item_name" value="Bouquet de Roses">
          <input type="hidden" name="amount" value="35.00">
          <input type="hidden" name="currency_code" value="EUR">
          <input type="submit" value="Acheter avec PayPal">
        </form>
      </div>

      <!-- Produit 2 : Tulipes -->
      <div class="product">
        <img src="https://images.unsplash.com/photo-1464965911861-746a04b4bca6" alt="Bouquet de tulipes">
        <h3>Bouquet de Tulipes</h3>
        <p>Coloré et lumineux, parfait pour égayer la maison.</p>
        <p><strong>30 €</strong></p>
        <form action="https://www.paypal.com/cgi-bin/webscr" method="post" target="_top" class="paypal-btn">
          <input type="hidden" name="cmd" value="_xclick">
          <input type="hidden" name="business" value="ton-email-paypal@exemple.com">
          <input type="hidden" name="item_name" value="Bouquet de Tulipes">
          <input type="hidden" name="amount" value="30.00">
          <input type="hidden" name="currency_code" value="EUR">
          <input type="submit" value="Acheter avec PayPal">
        </form>
      </div>

      <!-- Produit 3 : Lys -->
      <div class="product">
        <img src="https://images.unsplash.com/photo-1592796942469-fc98c3a4d0d2" alt="Lys blanc">
        <h3>Lys à l’unité</h3>
        <p>Élégant et raffiné, pour un style minimaliste.</p>
        <p><strong>8 €</strong></p>
        <form action="https://www.paypal.com/cgi-bin/webscr" method="post" target="_top" class="paypal-btn">
          <input type="hidden" name="cmd" value="_xclick">
          <input type="hidden" name="business" value="ton-email-paypal@exemple.com">
          <input type="hidden" name="item_name" value="Lys à l’unité">
          <input type="hidden" name="amount" value="8.00">
          <input type="hidden" name="currency_code" value="EUR">
          <input type="submit" value="Acheter avec PayPal">
        </form>
      </div>

    </div>
  </section>

  <section class="contact" id="contact">
    <h2>Contactez-nous</h2>
    <p>📍 123 Rue des Fleurs, Paris</p>
    <p>📞 01 23 45 67 89</p>
    <p>✉️ contact@fleuriste-emeraude.com</p>
    <p><em>Commandez par téléphone ou directement en ligne !</em></p>
  </section>

  <footer>
    <p>&copy; 2025 Fleuriste Émeraude - Tous droits réservés</p>
  </footer>

</body>
</html>

