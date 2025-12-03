# 🚀 Manual de Atualização Tasy EMR

[![GitHub Pages](https://img.shields.io/badge/GitHub-Pages-blue?logo=github)](https://seu-usuario.github.io/manual-tasy/)
[![Version](https://img.shields.io/badge/version-2.0-brightgreen)](https://github.com/seu-usuario/manual-tasy)
[![License](https://img.shields.io/badge/license-MIT-blue)](LICENSE)

## 📖 Sobre

Manual interativo e prático para atualização do sistema Tasy EMR, baseado em experiência real de atualização em ambiente de homologação.

**Versão coberta:** 5.01.1835.267 → 5.03.1842 SP80

## ✨ Características

- ✅ **Interativo**: Checklist com salvamento automático
- 📝 **Scripts SQL**: Prontos para copiar e usar
- 💾 **Registro**: Documentação automática do processo
- 📊 **Exportação**: Gere relatórios em TXT
- 🎨 **Design Moderno**: Interface amigável e responsiva
- 📱 **Mobile-Friendly**: Funciona em qualquer dispositivo
- 🔒 **Offline**: Funciona sem conexão com internet

## 🌐 Acesso Online

**Link do Manual:** [https://seu-usuario.github.io/manual-tasy/](https://seu-usuario.github.io/manual-tasy/)

## 📂 Estrutura do Projeto

```
manual-tasy/
├── index.html              # Manual interativo principal
├── scripts/
│   ├── desativar_jobs.sql  # Script pré-atualização
│   └── reativar_jobs.sql   # Script pós-atualização
├── README.md               # Este arquivo
└── LICENSE                 # Licença do projeto
```

## 🚀 Como Usar

### Online (Recomendado)

Acesse diretamente pelo navegador:
👉 [https://seu-usuario.github.io/manual-tasy/](https://seu-usuario.github.io/manual-Att-tasy/)

### Local

1. Clone o repositório:
```bash
git clone https://github.com/seu-usuario/manual-tasy.git
cd manual-tasy
```

2. Abra o arquivo `index.html` no navegador

## 📋 Seções do Manual

1. **📋 Preparação** - Requisitos e configurações iniciais
2. **💾 Scripts** - Scripts SQL para gerenciamento de jobs
3. **⚙️ Atualização** - Processo passo a passo (Download, Prepare, Update)
4. **✅ Pós-Atualização** - Validações e reativação do sistema
5. **📝 Checklist** - 15 itens para acompanhamento completo
6. **💡 Regras** - Regras de ouro e boas práticas
7. **📊 Registro** - Documentação e exportação do processo

## 🛠️ Scripts SQL Incluídos

### `desativar_jobs.sql`
- Captura valor de JOB_QUEUE_PROCESSES
- Desabilita processamento de jobs
- Quebra todas as jobs ativas
- Validação do estado

### `reativar_jobs.sql`
- Verifica objetos inválidos
- Restaura JOB_QUEUE_PROCESSES
- Reativa todas as jobs
- Validação final

## ⚠️ Regras de Ouro

### ✅ SEMPRE
- Backup completo antes de iniciar
- Testar em homologação primeiro
- Anotar JOB_QUEUE_PROCESSES
- Usar builds/SPs intermediários
- Aguardar 30s após desabilitar jobs

### ❌ NUNCA
- Atualizar sem backup
- Pular desativação de jobs
- Fechar navegador durante UPDATE DATABASE
- Usar Build = 0
- Usar último SP/build disponível

## 📊 Tempo Estimado

| Etapa | Tempo |
|-------|-------|
| Preparação | 15 min |
| Desativar jobs | 5 min |
| Download | 5 min |
| Prepare Update | 10 min |
| Update Database | 30 min - 2h |
| Reativar jobs | 5 min |
| Iniciar aplicações | 15 min |
| **TOTAL** | **1h30 - 3h** |

## 🤝 Contribuindo

Contribuições são bem-vindas! Para contribuir:

1. Fork o projeto
2. Crie uma branch para sua feature (`git checkout -b feature/NovaFeature`)
3. Commit suas mudanças (`git commit -m 'Adiciona NovaFeature'`)
4. Push para a branch (`git push origin feature/NovaFeature`)
5. Abra um Pull Request

## 📝 Changelog

### v2.0 (Dezembro 2025)
- ✨ Interface interativa completa
- 📝 Checklist com 15 itens
- 💾 Sistema de registro e exportação
- 🎨 Design moderno e responsivo
- 📱 Suporte mobile
- 💾 Salvamento automático no navegador

### v1.0 (Dezembro 2025)
- 📄 Manual básico em Markdown
- 📝 Scripts SQL iniciais

## 👨‍💻 Autor

**Sérgio**
- Especialista em Tasy EMR
- Experiência em ambientes de homologação e produção

## 📄 Licença

Este projeto está sob a licença MIT. Veja o arquivo [LICENSE](LICENSE) para mais detalhes.

## 🙏 Agradecimentos

- Baseado em atualização real Tasy 5.01.1835.267 → 5.03.1842 SP80
- Melhorias sobre manual oficial Philips
- Comunidade Tasy EMR

## 📞 Suporte

- 📧 Issues: [GitHub Issues](https://github.com/seu-usuario/manual-tasy/issues)
- 📚 Documentação Oficial: Portal do Cliente Philips
- 🌐 Portal: customerportal.sa1.hsdp.io

## ⚡ Quick Start

```bash
# Clone o repositório
git clone https://github.com/seu-usuario/manual-tasy.git

# Entre no diretório
cd manual-tasy

# Abra o manual
open index.html  # macOS
start index.html # Windows
xdg-open index.html # Linux
```

---

<div align="center">

**🌟 Se este manual foi útil, deixe uma estrela no repositório! 🌟**

[![Star on GitHub](https://img.shields.io/github/stars/seu-usuario/manual-tasy?style=social)](https://github.com/seu-usuario/manual-tasy)

</div>
