# Sistema de Gestão da Qualidade — Braskim

Site: https://braskim-qualidade.web.app

- `public/index.html` — o sistema inteiro (arquivo único). A configuração do Firebase está no bloco `window.BRASKIM_FIREBASE`, no começo do arquivo.
- `.github/workflows/deploy.yml` — publica sozinho no Firebase Hosting a cada alteração na branch `main` (precisa do secret `FIREBASE_SERVICE_ACCOUNT`).
- `firebase.json` / `.firebaserc` — configuração do Hosting.
- `regras-firestore.txt` — regras de segurança: colar em Firebase › Firestore Database › Regras › Publicar.

Para atualizar o sistema: substitua `public/index.html` pelo arquivo novo (Add file › Upload files) e confirme o commit. Em 1–2 minutos o site é atualizado (aba Actions mostra o andamento).
