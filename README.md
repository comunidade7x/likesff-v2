🎮 Bot Likes FF - API Gratuita de Likes





API grátis e simplificada para adicionar likes diários a jogadores de Free Fire usando apenas o uid.
✅ Sem necessidade de token
🎯 Respostas completas em JSON com informações detalhadas do jogador
💡 Fácil de integrar e usar


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

🌟 Gratuito e sem token

📝 Respostas JSON detalhadas

🎯 Fácil integração

🔧 Mantido por @Regiis7x



---

💡 Exemplo rápido de uso com curl:

curl "https://botlikesff.rexapi.com.br/api/v2/likes?uid=123456789"


---

🔹 Observações

Este endpoint adiciona 100 likes diários automaticamente.

UID é obrigatório e único por jogador.

Em caso de erro inesperado, tente novamente ou contate o suporte.

Respostas incluem status, detalhes do jogador e informações sobre os likes.
