# Vio-Qrcode

## Sobre o Site — vio.api.br

O **VIO** é uma solução desenvolvida pelo **SERPRO** (Serviço Federal de Processamento de Dados) para certificação de autenticidade de documentos de identificação por meio de **QR Code VIO**.

O QR Code VIO carrega dados compactados e criptografados fornecidos pela própria entidade emissora do documento, garantindo:
- Segurança contra fraudes
- Não-repúdio das informações
- Validação online e offline (via app)

A API VIO oferece dois serviços principais:
- **VIO ENCODE** — Usada por entidades emissoras para gerar o QR Code VIO a partir dos dados do documento.
- **VIO DECODE** — Permite que sistemas automatizados e aplicativos façam a leitura, validação e consumo dos dados armazenados no QR Code VIO.

A validação também pode ser realizada pelo aplicativo **Vio: QR Seguro**, disponível para Android e iOS.

---

## Tipos de Documentos Suportados

| Documento | Descrição |
|-----------|-----------|
| **CNH** | Carteira Nacional de Habilitação (física e digital) |
| **CRLV Digital** | Certificado de Registro e Licenciamento de Veículo |
| **DNI** | Documento Nacional de Identidade |
| **RG Digital** | Registro Geral Digital (modelos estaduais e forças armadas/segurança) |
| **ATPV-e** | Autorização para Transferência de Propriedade de Veículo eletrônica |
| **Placa Veicular** | Placas de Identificação Veicular — PIV (padrão Mercosul) |
| **Credencial de Estacionamento** | Credencial para uso de vagas especiais de estacionamento |
| **PROID** | Documentos profissionais emitidos pelo sistema ProID |
| **Controle de Armamento** | Certificados de registro e documentos de controle e tráfego de armas |

> A lista de documentos compatíveis está em constante expansão conforme novas entidades emissoras se integram ao sistema VIO.

---

## Links Úteis

- [Portal SERPRO VIO](https://servicos.serpro.gov.br/vio/)
- [Documentação API VIO DECODE](https://apicenter.estaleiro.serpro.gov.br/documentacao/vio-decode/pt/)
- [Documentação API VIO ENCODE](https://apicenter.estaleiro.serpro.gov.br/documentacao/vio-encode/pt/)
