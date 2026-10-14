# Portal de Benefícios — Parceiros GEB

Hospedagem planejada: https://parceiro.compassrosesystems.com.br

- A raiz `/` é intencionalmente branca/vazia.
- `/modelo/` contém uma demonstração para empresas parceiras com benefícios por indicação, sem pagamento da empresa.
- `/404.html` é o erro personalizado; `.htaccess` o habilita em Apache/Locaweb.
- A página não coleta contatos nem dados médicos. O campo de curso apenas prepara mensagem para WhatsApp (62) 99205-3534.
- Telessaúde: assinaturas PF opcionais R$ 29,80/mês e PF + PIX Farma R$ 39,90/mês nos links fornecidos. Validar detalhes de cobertura com o fornecedor antes de divulgar como garantia.
- Educação: descontos **até** 83%, condicionados à disponibilidade e às regras do curso.
- Futuras páginas de parceiros podem ser copiadas de `modelo/` e personalizadas com nome, identidade, textos e referências reais.
- Associação institucional ao Selo G é distinta e não há concessão automática de reconhecimento por indicar serviços.

## Deploy

GitHub Actions envia os arquivos publicados à pasta `/public_html/parceiros/` via FTPS. Definir no repositório os Secrets: `LOCAWEB_FTP_SERVER`, `LOCAWEB_FTP_USERNAME`, `LOCAWEB_FTP_PASSWORD`. Ajustar `server-dir` caso a conta FTP já abra em `public_html`. Conferir o passo **Publicar na Locaweb** efetivamente executado; o workflow pode ter sucesso mesmo se a publicação foi pulada por falta de credenciais.
