# Barbearia Pires — site de agendamentos

Site responsivo em HTML, CSS e JavaScript puro, com identidade preta e dourada, usando a logomarca fornecida.

## Publicar no GitHub Pages
1. Crie um repositório no GitHub.
2. Envie `index.html`, `style.css`, `app.js` e a pasta `assets` para a raiz.
3. Em **Settings > Pages**, escolha **Deploy from a branch**, `main` e `/ (root)`.
4. Aguarde a URL do GitHub Pages aparecer.

## Demonstração
- Painel Administração: PIN inicial `1234`.
- Serviços, preços, duração, nomes, fotos por URL, expediente e dias são editáveis.
- Agendamentos, cancelamentos, conclusão, indicadores, exportação CSV e backup JSON funcionam localmente.
- Reservas sem preferência são atribuídas ao primeiro barbeiro disponível.
- Os horários são calculados para evitar sobreposição de reservas **dentro do mesmo navegador**.

## ATENÇÃO — antes de usar com clientes reais
Esta é uma **demonstração front-end**, sem servidor. Os dados são gravados em `localStorage` **de cada dispositivo/navegador**. Reservas feitas em celulares diferentes NÃO são compartilhadas. O PIN no front-end NÃO fornece autenticação segura. O GitHub Pages apenas hospeda arquivos estáticos e NÃO substitui um banco de dados.

Para operar de verdade, é necessário integrar banco de dados central (por exemplo Firebase Firestore), autenticação de administradores (Firebase Authentication), regras de segurança e operações atômicas no servidor para evitar agendamentos duplicados. Também é recomendável configurar consentimento e política de privacidade LGPD, limites de cancelamento, notificações e política de faltas.

## Arquivos
- `index.html`: estrutura do site
- `style.css`: visual e responsividade
- `app.js`: agendamentos e administração demonstrativa
- `assets/logo.jpeg`: logo fornecida pelo cliente
