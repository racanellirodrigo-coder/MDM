# 🏗️ Estrutura do Projeto - Mestre dos Móveis

## 📂 Organização Atual

```
MDM/
├── main.py                          # App Kivy (versão mobile) ⭐ USAR ESTA
├── main (1).py                      # App Kivy (backup)
├── MestreDosMoveis_Final.py         # Desktop Tkinter (polida)
├── MestreDosMoveis_Final (2).py     # Desktop Tkinter (backup)
├── app_moveis.py                    # Desktop Tkinter (básica)
├── index.html                       # Web version
│
├── buildozer.spec                   # Config APK ⭐ NOVO
├── requirements.txt                 # Dependências ⭐ NOVO
├── APK_BUILD_GUIDE.md               # Guia de build ⭐ NOVO
├── ESTRUTURA_PROJETO.md             # Este arquivo ⭐ NOVO
│
├── .github/
│   └── workflows/
│       └── build-apk.yml            # Automação GitHub Actions ⭐ NOVO
│
├── precos_materiais.json            # Dados de preços (runtime)
├── app_icon.png                     # Ícone (necessário para APK)
├── logo_mestre.png                  # Logo (necessário para APK)
├── art_quarto.png                   # Imagem galeria (necessário)
├── art_closet.png                   # Imagem galeria (necessário)
└── art_fachada.png                  # Imagem galeria (necessário)
```

---

## 🎯 Versão Recomendada para APK

**`main.py`** - Versão Kivy Mobile
- ✅ Otimizada para Android
- ✅ Melhor performance
- ✅ UI responsiva
- ✅ Todas as funcionalidades

---

## 🔄 Fluxo de Build Automático

```
1. Você faz commit e push
   ↓
2. GitHub Actions dispara
   ↓
3. Python + Buildozer compila APK
   ↓
4. APK gerado (bin/mestredosmoveis-debug.apk)
   ↓
5. Salvo em Artifacts
   ↓
6. Release criado automaticamente
   ↓
7. Download disponível para instalar
```

---

## 📋 Checklist de Setup

- [x] `main.py` funcional
- [x] `buildozer.spec` criado
- [x] `requirements.txt` criado
- [x] `.github/workflows/build-apk.yml` ativo
- [ ] Assets (imagens PNG) verificados
- [ ] Commit realizado
- [ ] Push para GitHub
- [ ] Monitorar Actions

---

## 🎯 Funcionalidades do App

| Funcionalidade | Status |
|----------------|--------|
| Tela de Loading | ✅ |
| Menu Principal | ✅ |
| Novo Orçamento | ✅ |
| Cálculo de Preço | ✅ |
| Show Room | ✅ |
| Área ADM (Login) | ✅ |
| Gerenciamento de Preços | ✅ |
| Persistência de Dados | ✅ |
| Interface Responsiva | ✅ |

---

## 📱 Compatibilidade

- **Android Mínimo:** 5.0 (API 21)
- **Android Alvo:** 12.0 (API 31)
- **Orientação:** Portrait (vertical)
- **Permissões:** Internet, Armazenamento

---

## 🚀 Como Disparar Build

### **Automático (Recomendado)**
```bash
git push origin main
# GitHub Actions dispara automaticamente
```

### **Manual Local**
```bash
buildozer android debug
# APK em: bin/mestredosmoveis-debug.apk
```

---

## 📥 Download do APK

1. **GitHub Actions (Temporário - 90 dias):**
   - Actions → Último workflow → Artifacts

2. **GitHub Releases (Permanente):**
   - Releases → Latest → Download APK

3. **Instalar no Celular:**
```bash
adb install bin/mestredosmoveis-debug.apk
```

---

## 🔄 Fluxo de Desenvolvimento

```
1. Editar código em main.py
2. Testar localmente (python main.py)
3. Commit das mudanças
4. Push para GitHub
5. GitHub Actions compila APK
6. Download e instala no celular
7. Testa no Android
```

---

## 🐛 Troubleshooting Rápido

| Problema | Solução |
|----------|---------|
| APK não gera | Verifique logs em Actions |
| Imagens não aparecem | Garanta PNG na raiz |
| App trava | Reinicie o celular |
| Build muito lento | Normal (10-20 min primeira vez) |
| Erro de permissões | Ativa USB Debug no celular |

---

## 🔐 Dados Sensíveis

⚠️ **Atualmente hardcoded:**
- Senha ADM: "511996"
- Preços padrão em JSON

📌 **Melhorias futuras:**
- Usar variáveis de ambiente
- Backend com autenticação real
- Criptografia de dados

---

## 📞 Próximas Ações

1. ✅ Verificar se todos os arquivos foram criados
2. ✅ Fazer commit e push
3. ✅ Monitorar GitHub Actions
4. ✅ Download do APK quando pronto
5. ✅ Testar no Android

---

**Status:** ✅ Projeto 100% configurado para build automático! 🎉
