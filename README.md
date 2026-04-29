# Vio-Qrcode

## Sobre o site vio.api.br

O **VIO** (Validação de Identidade Offline) é uma plataforma da [SERPRO](https://www.serpro.gov.br/) que fornece **QR Codes seguros** para documentos oficiais brasileiros. Ao ser escaneado, o QR Code VIO revela os dados originais do documento, garantindo **autenticidade** e **não-repúdio** por meio de criptografia com chaves privadas do emissor.

A API permite que organizações:
- **Emitam** QR Codes VIO para seus documentos (encoder)
- **Decodifiquem e validem** QR Codes VIO (decoder)
- Realizem verificações **online e offline** via app ou integração direta

### Endpoints principais

| Ambiente | Encoder | Decoder |
|---|---|---|
| Produção | `https://gateway.apiserpro.serpro.gov.br/vioenc/v1/encode` | `https://gateway.apiserpro.serpro.gov.br/viodec` |
| Homologação | `https://gateway.apiserpro.serpro.gov.br/vio-encoder-default/v1/encode` | `https://gateway.apiserpro.serpro.gov.br/viodec-trial/v1/decode` |

---

## Tipos de Documentos Suportados

| Sigla | Documento |
|---|---|
| **CNH** | Carteira Nacional de Habilitação |
| **CRLV** | Certificado de Registro e Licenciamento de Veículo |
| **ATPV-e** | Autorização para Transferência de Propriedade de Veículo Eletrônica |
| **DNI** | Documento Nacional de Identidade |
| **CIN** | Carteira de Identidade Nacional (em implantação) |
| **PIV** | Placa de Identificação Veicular |
| **RG Digital** | Identidade Digital (a depender do estado emissor) |
| **Credencial PcD/Idoso** | Credencial de Estacionamento para Pessoas com Deficiência ou Idosos |

> **Observação:** A lista de documentos é ampliada progressivamente pelo SERPRO conforme novos tipos de documentos oficiais adotam o padrão VIO. Consulte sempre a [documentação oficial](https://vio.api.br/) para a versão mais atualizada.

