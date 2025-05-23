<!DOCTYPE html> 
<html lang="pt-BR">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Inclusão de Imigrantes</title>
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;600;700&display=swap" rel="stylesheet">
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.0/css/all.min.css" />
  <link rel="stylesheet" href="https://unpkg.com/leaflet@1.9.3/dist/leaflet.css" />
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      font-family: 'Inter', sans-serif;
    }
    body {
      background-color: #fefefe;
      color: #333;
    }
    header {
      background: linear-gradient(to right, #f06292, #ba68c8);
      color: white;
      padding: 40px 20px;
      text-align: center;
    }
    header h1 {
      font-size: 2.5rem;
      margin-bottom: 10px;
    }
    nav {
      background-color: #fff;
      box-shadow: 0 2px 6px rgba(0,0,0,0.1);
      display: flex;
      justify-content: center;
      flex-wrap: wrap;
      gap: 10px;
      padding: 15px;
      position: sticky;
      top: 0;
      z-index: 1000;
    }
    nav a {
      margin: 0 10px;
      text-decoration: none;
      color: #ba68c8;
      font-weight: bold;
      font-size: 1rem;
    }
    section {
      padding: 40px 20px;
      max-width: 1000px;
      margin: 0 auto;
    }
    section img {
      max-width: 100%;
      border-radius: 10px;
      margin: 20px 0;
    }
    .btn {
      background-color: #ba68c8;
      color: white;
      padding: 10px 20px;
      border: none;
      border-radius: 20px;
      font-size: 1rem;
      cursor: pointer;
      transition: 0.3s;
      display: inline-block;
      margin: 10px 0;
    }
    .btn:hover {
      background-color: #ab47bc;
    }
    footer {
      background-color: #f06292;
      color: white;
      text-align: center;
      padding: 20px;
      margin-top: 40px;
    }
    .relato {
      background-color: #f3e5f5;
      padding: 20px;
      margin: 20px 0;
      border-left: 5px solid #ba68c8;
      border-radius: 10px;
    }
    .icones {
      font-size: 1.5rem;
      margin-right: 10px;
      color: #f06292;
    }
    #mapa {
      height: 400px;
      margin-top: 20px;
      border-radius: 10px;
    }
    #guia-documentos {
      background-color: #f9f9f9;
      padding: 20px;
      border-radius: 10px;
      margin-top: 20px;
    }
  </style>
</head>
<body>
  <div id="google_translate_element"></div>
  <script type="text/javascript">
    function googleTranslateElementInit() {
      new google.translate.TranslateElement({pageLanguage: 'pt', layout: google.translate.TranslateElement.InlineLayout.SIMPLE}, 'google_translate_element');
    }
  </script>
  <script type="text/javascript" src="//translate.google.com/translate_a/element.js?cb=googleTranslateElementInit"></script>

  <header>
    <h1>Inclusão e Apoio a Imigrantes</h1>
    <p>Ajuda real, informações acessíveis e acolhimento seguro</p>
  </header>

  <nav>
    <a href="#documentos">Documentos</a>
    <a href="#capacitação">Capacitação</a>
    <a href="#denuncia">Denúncia</a>
    <a href="#relatos">Relatos</a>
    <a href="#nucleos">Núcleos de Apoio</a>
    <a href="#vulnerabilidade">Vulnerabilidade Social</a>
    <a href="#sobre">Sobre Nós</a>
  </nav>

  <section id="documentos">
    <h2><i class="fa-solid fa-id-card icones"></i>Como emitir documentos</h2>
    <p>Passo a passo para emitir seus documentos básicos:</p>
    <div id="guia-documentos">
      <ol>
        <li><strong>Registro Civil:</strong> Cartório com identidade do país de origem, tradução juramentada e comprovante de residência.</li>
        <li><strong>CPF:</strong> <a href="https://www.gov.br/receitafederal/pt-br/assuntos/cadastro-cpf" target="_blank">Site da Receita Federal</a>.</li>
        <li><strong>Cartão SUS:</strong> UBS com identidade, CPF e comprovante de residência.</li>
        <li><strong>Carteira de Trabalho Digital:</strong> <a href="https://www.gov.br/pt-br/temas/carteira-de-trabalho-digital" target="_blank">Acesse aqui</a>.</li>
        <li><strong>Currículo Profissional:</strong> <a href="https://www.canva.com/pt_br/criar/curriculos/" target="_blank">Canva</a>.</li>
      </ol>
    </div>
    <img src="https://images.unsplash.com/photo-1581092334428-fd7b8a788db1?ixlib=rb-4.0.3&auto=format&fit=crop&w=1000&q=80" alt="documentos" />
  </section>

  <section id="capacitação">
    <h2><i class="fa-solid fa-chalkboard-user icones"></i>Capacitação e Geração de Renda</h2>
    <ul>
      <li><a href="https://www.sebrae.com.br/sites/PortalSebrae/cursosonline" target="_blank">Sebrae</a></li>
      <li><a href="https://loja.mundosenai.com.br" target="_blank">Senai</a></li>
      <li><a href="https://www.coursera.org" target="_blank">Coursera</a></li>
    </ul>
    <div id="mapa"></div>
  </section>

  <section id="denuncia">
    <h2><i class="fa-solid fa-triangle-exclamation icones"></i>Canal de Denúncia</h2>
    <p>Denuncie abusos de forma segura e anônima através do Disque 100:</p>
    <a href="https://www.gov.br/mdh/pt-br/navegue-por-temas/ouvidoria" class="btn" target="_blank">Preciso de Ajuda</a>
    <p>Chat com atendimento humanizado também está disponível por ONGs parceiras.</p>
  </section>

  <section id="relatos">
    <h2><i class="fa-solid fa-heart icones"></i>Histórias Inspiradoras</h2>
    <div class="relato">
      <p><strong>Rosa, 34 anos (Venezuela)</strong>: "Cheguei ao Brasil sem nada. Consegui regularizar meus documentos com ajuda de uma ONG, fiz um curso de confeitaria e hoje tenho meu próprio negócio!"</p>
    </div>
    <div class="relato">
      <p><strong>Mariam, 28 anos (Senegal)</strong>: "Fui acolhida por uma casa para mulheres migrantes. Hoje trabalho com artesanato e ajudo outras mulheres a se fortalecerem."</p>
    </div>
    <img src="https://s2.glbimg.com/hcYDD-R-lmSZ2qfO7_ecN7A8BFs=/s.glbimg.com/jo/g1/f/original/2016/07/18/fotos-pra-gabi-28.jpg" alt="mulheres inspiradoras" />
  </section>

  <section id="nucleos">
    <h2><i class="fa-solid fa-people-roof icones"></i>Núcleos de Apoio a Refugiados na Bahia</h2>
    <ul>
      <li><strong><a href="https://www.unijorge.edu.br/noticias/nucleo-de-apoio-a-migrantes-e-refugiados" target="_blank">Unijorge:</a></strong> Núcleo de Apoio a Migrantes e Refugiados com atendimentos jurídicos e sociais.</li>
      <li><strong><a href="https://www.ufba.br/noticias/ufba-acolhe-migrantes-e-refugiados" target="_blank">UFBA:</a></strong> Projeto de Extensão com apoio a refugiados, oficinas de integração e pesquisa sobre mobilidade humana.</li>
    </ul>
  </section>

  <section id="vulnerabilidade">
    <h2><i class="fa-solid fa-house-crack icones"></i>Vulnerabilidade Social</h2>
    <p>Mulheres refugiadas enfrentam grandes desafios como falta de moradia, alimentação e rede de apoio. Este site também indica:</p>
    <ul>
      <li><a href="https://www.crb.org.br/portal/noticia/ongs-que-ajudam-refugiados-no-brasil" target="_blank">ONGs que oferecem cestas básicas, kits de higiene e apoio psicológico</a></li>
      <li><a href="https://www.gov.br/pt-br/servicos/inscrever-se-no-cadastro-unico-para-programas-sociais-do-governo-federal" target="_blank">Locais para cadastro em programas sociais como Bolsa Família</a></li>
      <li><a href="https://www.sescbahia.com.br" target="_blank">Espaços que promovem oficinas de geração de renda (como o SESC)</a></li>
    </ul>
  </section>

  <section id="sobre">
    <h2><i class="fa-solid fa-circle-info icones"></i>Sobre Nós</h2>
    <p>Este site foi desenvolvido com o objetivo de apoiar mulheres imigrantes e refugiadas, fornecendo informações acessíveis sobre documentos, capacitação, canais de denúncia e acolhimento.</p>
    <p>Projeto desenvolvido por <strong>Anna Luísa Queiroz, Brenda Cerqueira, Karina Almeida, Rone Filho, Samille Cardoso e Talita Vieira</strong> da <strong>escola SESI Djalma Pessoa</strong>.</p>
  </section>

  <footer>
    <p>© 2025 | Desenvolvido por Anna Luísa Queiroz, Brenda Cerqueira, Karina Almeida, Rone Filho, Samille Cardoso e Talita Vieira — 3°N EQUIPE 5</p>
  </footer>

  <script src="https://unpkg.com/leaflet@1.9.3/dist/leaflet.js"></script>
  <script>
    var mapa = L.map('mapa').setView([-23.5505, -46.6333], 12);
    L.tileLayer('https://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png', {
      attribution: 'Map data © OpenStreetMap contributors'
    }).addTo(mapa);

    L.marker([-23.5505, -46.6333]).addTo(mapa)
      .bindPopup('ONG de Apoio à Mulher Imigrante')
      .openPopup();
  </script>
</body>
</html>
