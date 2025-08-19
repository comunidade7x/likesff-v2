🚀 Bot Likes FF - API Gratuita de Likes





Uma API gratuita para adicionar likes diários a jogadores de Free Fire usando apenas o uid.
✅ Não precisa mais de token.
💡 Simples, rápido e seguro.
🎯 Respostas completas em JSON com detalhes do jogador e status do envio.


---

📌 Endpoint

GET https://botlikesff.rexapi.com.br/api/v2/likes?uid=UID_DO_JOGADOR

🔹 Parâmetro

Parâmetro	Tipo	Obrigatório	Descrição

uid	number	Sim	ID do jogador Free Fire



---

💬 Exemplos de Respostas

1️⃣ Sucesso

{
  "status": "success",
  "dev": "@Regiis7x",
  "titulo": "❤️ LIKES DIÁRIOS ❤️",
  "player": {
    "nickname": "NOME_DO_JOGADOR",
    "region": "REGIÃO_DO_JOGADOR",
    "level": 50,
    "exp": "123.456",
    "uid": "123456789"
  },
  "likes": {
    "antes": "1.000",
    "depois": "1.100",
    "adicionados": "100",
    "limite_diario": "❌"
  },
  "status_envio": "🎉 Likes enviados com sucesso!",
  "agradecimento": "💖 Obrigado por usar nosso sistema! Continue jogando e se divertindo!",
  "dicas": [
    "• Este endpoint adiciona automaticamente 100 likes por dia.",
    "• UID é obrigatório e único por jogador.",
    "• Em caso de erro inesperado, tente novamente ou contate o suporte."
  ]
}


---

2️⃣ Jogador Não Encontrado

{
  "status": "not_found",
  "dev": "@Regiis7x",
  "title": "❌ JOGADOR NÃO ENCONTRADO ❌",
  "mensagem": "Não foi possível localizar o jogador com o UID fornecido.",
  "dicas": [
    "• Verifique se o UID está correto.",
    "• Evite espaços ou caracteres extras.",
    "• Tente outro UID caso o problema persista."
  ]
}


---

3️⃣ Sistema em Manutenção

{
  "status": "manutencao",
  "dev": "@Regiis7x",
  "title": "⚠️ SISTEMA EM MANUTENÇÃO ⚠️",
  "mensagem": "O sistema de likes está temporariamente indisponível.",
  "dica": "⏳ Tente novamente mais tarde ou entre em contato com o suporte se o problema persistir."
}


---

4️⃣ Erro Inesperado

{
  "status": "error",
  "dev": "@Regiis7x",
  "title": "❌ ERRO INESPERADO ❌",
  "mensagem": "Ocorreu um erro ao processar sua requisição.",
  "detalhes": [
    "• Verifique se o UID informado é válido.",
    "• Tente novamente mais tarde.",
    "• Contate o suporte se o problema persistir."
  ]
}


---

⚡ Vantagens

Sem necessidade de token ou autenticação complexa

Respostas JSON detalhadas e estruturadas

Sistema 100% gratuito e confiável

Mantido por @Regiis7x



---

💡 Exemplo rápido de uso com curl:

curl "https://botlikesff.rexapi.com.br/api/v2/likes?uid=123456789"
