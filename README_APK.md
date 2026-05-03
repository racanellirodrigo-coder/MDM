# 📱 Mestre dos Móveis Gold - APK

App de orçamento de móveis planejados para Android.

## ✨ Funcionalidades

- ✅ **Novo Orçamento** - Calcule projetos com precisão
- ✅ **Show Room** - Galeria de projetos realizados
- ✅ **Área Administrativa** - Gerenciamento de preços
- ✅ **Interface Luxuosa** - Design Gold Edition
- ✅ **Cálculo Automático** - Baseado em metragem e materiais

## 🚀 Como Compilar

### Pré-requisitos
- Python 3.11+
- Java JDK 11+
- Android SDK
- Android NDK 25.x

### Build Local
```bash
# Instalar buildozer
pip install buildozer cython

# Compilar APK
buildozer android debug

# Resultado
# bin/mestredomoveis-debug.apk
```

### Build Automático (GitHub Actions)
1. Faça push do código
2. Acesse **Actions** → **Build Android APK**
3. Aguarde a compilação
4. Baixe em **Artifacts**

## 📥 Instalação

### Via GitHub Releases
1. Acesse: https://github.com/racanellirodrigo-coder/MDM/releases
2. Baixe `mestredomoveis-debug.apk`
3. Transfira para o Android
4. Abra e instale

### Via ADB (linha de comando)
```bash
adb install bin/mestredomoveis-debug.apk
```

## 🔐 Credenciais Padrão

- **Login:** `511996`
- **Senha:** `511996`

## 📋 Especificações

| Item | Valor |
|------|-------|
| **Versão** | 1.0.0 |
| **API Android** | 31 (mín. 21) |
| **Arquiteturas** | ARM64, ARMv7 |
| **Tamanho** | ~50MB |
| **Framework** | Kivy 2.3.0 |

## 🔧 Estrutura do Projeto

```
MDM/
├── main.py                    # App principal
├── buildozer.spec             # Configuração buildozer
├── requirements.txt           # Dependências
├── precos_materiais.json      # Base de preços
├── .github/workflows/
│   └── build-apk.yml          # CI/CD
└── README_APK.md              # Este arquivo
```

## 🛠️ Troubleshooting

### "Permission denied" ao compilar
```bash
chmod +x buildozer
```

### Erro do NDK
```bash
buildozer android clean
buildozer android debug --ndk-version=25b
```

### APK não instala
- Ative "Instalação de app desconhecidos" no Android
- Verifique se o dispositivo está em modo depuração

## 📞 Contato

Desenvolvido por **racanellirodrigo-coder**

---

**Status:** ✅ Pronto para produção v1.0.0
