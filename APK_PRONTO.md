# 📱 Guia Rápido - APK Pronto para Usar

## 🚀 3 Formas de Gerar o APK

### **FORMA 1: Mais Rápida (GitHub Actions) ⚡**

```bash
git push origin main
```

✅ Automático
✅ Sem instalações
✅ APK em 15-20 min
✅ Download em: GitHub Actions → Artifacts

---

### **FORMA 2: Local com Python 🐍**

**Pré-requisitos:**
- Python 3.11+
- Java JDK 11+
- Android SDK

**Comando:**
```bash
python build_apk_quick.py
```

✅ Rápido
✅ Customizável
✅ APK em `bin/`

---

### **FORMA 3: Local com Bash 🔧**

**Apenas Linux/Mac:**
```bash
chmod +x build.sh
./build.sh
```

---

## 📲 Instalar no Celular

### **Com USB (Recomendado)**

```bash
# 1. Conecte o celular via USB
# 2. Ative "Modo Desenvolvedor" e "Depuração USB"

# 3. Instale o APK:
adb install bin/mestredosmoveis-debug.apk
```

### **Sem USB (Manual)**

```bash
# 1. Transfira o APK para o celular
# 2. Abra o gerenciador de arquivos
# 3. Toque no APK
# 4. Permita instalação de fontes desconhecidas
# 5. Instale!
```

---

## ⏱️ Tempo Estimado

| Método | Tempo | Notas |
|--------|-------|-------|
| GitHub Actions | 15-20 min | Primeira vez mais lenta |
| Local (Python) | 10-15 min | Requer setup local |
| Bash | 10-15 min | Apenas Linux/Mac |

---

## 🎯 Checklist Antes de Build

- [ ] `main.py` existe e funciona
- [ ] Imagens (PNG) estão na raiz
- [ ] `buildozer.spec` está configurado
- [ ] `requirements.txt` tem as dependências
- [ ] Conexão internet estável

---

## 🔧 Troubleshooting Rápido

| Problema | Solução |
|----------|---------|
| "buildozer not found" | `pip install buildozer cython` |
| "Java not found" | Instale JDK 11 |
| "APK muito grande" | Normal (40-60 MB) |
| "Build travou" | Reinicie ou aumente RAM |
| "Permissão negada (build.sh)" | `chmod +x build.sh` |

---

## 📊 Tamanho do APK

- Usual: 40-60 MB
- Com imagens: Até 100 MB
- Instalado: 120-180 MB

---

## 🎉 Depois de Gerar

1. ✅ APK está em `bin/mestredosmoveis-debug.apk`
2. ✅ Transfira para celular
3. ✅ Instale (pode levar uns segundos)
4. ✅ Abra o app!
5. ✅ Aproveite! 🚀

---

## 🔐 Credenciais do App

**Login ADM:**
- Usuário: `511996`
- Senha: `511996`

---

## 🚀 Próximas Ações

1. Escolha a forma de build (recomendo Form 1 - GitHub)
2. Gere o APK
3. Instale no celular
4. Teste todas as funcionalidades
5. Se precisar mexer, edite `main.py` e repita

---

**Status:** ✅ Pronto para usar agora mesmo! 🎊
