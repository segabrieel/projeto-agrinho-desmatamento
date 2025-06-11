<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Projeto Agrinho: Desmatamento</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <header>
        <h1>Projeto Agrinho: Desmatamento</h1>
    </header>
    <main>
        <section>
            <h2>Sobre o Desmatamento</h2>
            <p>O desmatamento é um problema ambiental sério que afeta o Brasil e o mundo. Neste site, você vai aprender sobre suas causas, consequências e soluções.</p>
        </section>
        <section>
            <h2>Causas</h2>
            <p>As principais causas do desmatamento são a expansão agrícola, pecuária, queimadas e exploração ilegal de madeira.</p>
        </section>
        <section>
            <h2>Consequências</h2>
            <p>Perda de biodiversidade, mudanças climáticas e impactos sociais são algumas das consequências do desmatamento.</p>
        </section>
        <section>
            <h2>Soluções</h2>
            <p>Educação ambiental, fiscalização, leis eficazes e reflorestamento são formas de combater o desmatamento.</p>
        </section>
    </main>
    <footer>
        <p>Projeto Agrinho - Desmatamento | 2025</p>
    </footer>
    <script src="script.js"></script>
</body>
</html>
"""

css_content = """
body {
    font-family: Arial, sans-serif;
    line-height: 1.6;
    margin: 0;
    padding: 0;
    background-color: #f4f4f4;
}

header {
    background-color: #228B22;
    color: white;
    padding: 1em 0;
    text-align: center;
}

main {
    padding: 20px;
}

section {
    margin-bottom: 20px;
    background: white;
    padding: 15px;
    border-radius: 8px;
}

footer {
    text-align: center;
    padding: 1em 0;
    background-color: #ddd;
}
"""

js_content = """
// Nenhuma funcionalidade interativa por enquanto
console.log("Site Agrinho: Desmatamento carregado.");
"""

# Caminho para salvar os arquivos do site
site_dir = os.path.join(output_dir, "site")
os.makedirs(site_dir, exist_ok=True)

with open(os.path.join(site_dir, "index.html"), "w", encoding="utf-8") as f:
    f.write(html_content)

with open(os.path.join(site_dir, "style.css"), "w", encoding="utf-8") as f:
    f.write(css_content)

with open(os.path.join(site_dir, "script.js"), "w", encoding="utf-8") as f:
    f.write(js_content)

# Criar o README.md
readme_content = """
# 🌳 Projeto Agrinho: Desmatamento

Este repositório contém um projeto educacional desenvolvido para o programa **Agrinho**, com o tema **desmatamento**.

## 📁 Estrutura

- `site/`: Mini site com conteúdo educativo.
- `artigo-desmatamento.docx`: Artigo explicativo sobre o desmatamento.

## 🧠 Objetivo

Conscientizar sobre os impactos do desmatamento, suas causas e possíveis soluções para preservar o meio ambiente.

## 📅 Ano

2025

## 📎 Licença

Distribuído sob a licença MIT.
"""

with open(os.path.join(output_dir, "README.md"), "w", encoding="utf-8") as f:
    f.write(readme_content)

output_dir
