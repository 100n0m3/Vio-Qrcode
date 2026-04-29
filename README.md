vio.api.br


# VIO API

API e biblioteca para leitura e validação de QR Codes comuns e QR Codes VIO/SERPRO de documentos oficiais brasileiros.

A VIO API permite integrar sistemas capazes de identificar, decodificar e validar QR Codes presentes em documentos como:

* CNH
* CRLV
* ATPV-e
* Diplomas digitais
* Documentos oficiais com QR Code VIO
* QR Codes convencionais

---

# Recursos

* Leitura de QR Code comum
* Leitura de QR Code VIO/SERPRO
* Upload de imagens e PDFs
* Suporte a Base64
* API REST simples
* Respostas em JSON
* Validação de autenticidade
* Processamento rápido
* Compatível com qualquer linguagem

---

# Casos de uso

* Validação documental
* Automação de cadastros
* Check-in digital
* Sistemas de transporte
* Plataformas antifraude
* ERPs e CRMs
* Aplicações governamentais
* Leitura automatizada de documentos

---

# Como funciona

Envie uma imagem, PDF ou arquivo contendo um QR Code para a API.

A plataforma identifica automaticamente:

* Tipo do QR Code
* Documento relacionado
* Dados decodificados
* Informações de validação

---

# Exemplo de requisição

```bash
curl -X POST https://vio.api.br/qrcode/read \
  -H "X-API-Key: SUA_API_KEY" \
  -H "Content-Type: application/json" \
  -d '{
    "image": "data:image/png;base64,..."
  }'
```

---

# Exemplo de resposta

```json
{
  "success": true,
  "type": "VIO",
  "document": "CRLV",
  "data": {
    "placa": "ABC1D23",
    "renavam": "00000000000"
  }
}
```

---

# Instalação

Você pode consumir a API utilizando qualquer linguagem compatível com HTTP:

* Python
* Node.js
* PHP
* Java
* Go
* C#
* Ruby

---

# Exemplo em Python

```python
import requests

url = "https://vio.api.br/qrcode/read"

payload = {
    "image": "data:image/png;base64,..."
}

headers = {
    "X-API-Key": "SUA_API_KEY"
}

response = requests.post(url, json=payload, headers=headers)

print(response.json())
```

---

# Sobre o QR Code VIO

O QR Code VIO é um padrão desenvolvido pelo SERPRO para validação criptográfica de documentos oficiais brasileiros.

Ele é utilizado para garantir autenticidade e integridade de documentos digitais e impressos.

---

# Segurança

* Comunicação HTTPS
* Validação criptográfica
* Processamento seguro
* Suporte a documentos oficiais

---

# Documentação

Acesse a documentação completa:

https://vio.api.br/

---

# Licença

MIT License
