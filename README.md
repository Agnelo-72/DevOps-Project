# DevOps Project 🚀

Meu primeiro projeto DevOps com CI/CD pipeline automatizado usando GitHub Actions, Java 21 e Gradle.

---

## 📋 Sobre o Projeto

Este projeto demonstra boas práticas de DevOps incluindo:
- ✅ Integração Contínua (CI) com GitHub Actions
- ✅ Build automatizado com Gradle
- ✅ Containerização com Docker
- ✅ Gerenciamento de versões JDK

---

## 🛠️ Tecnologias Utilizadas

| Tecnologia | Versão |
|---|---|
| **Java** | 21 |
| **JDK Distribution** | Temurin |
| **Build Tool** | Gradle |
| **CI/CD** | GitHub Actions |
| **Containerização** | Docker |

---

## 📁 Estrutura do Projeto

```
my-project/
├── .github/workflows/ci.yml      # Pipeline CI/CD automatizado
├── src/                          # Código fonte Java
├── gradle/                       # Gradle wrapper
├── build.gradle                  # Configurações de build
├── Dockerfile                    # Configuração Docker
├── gradlew                       # Gradle wrapper (Linux/Mac)
├── gradlew.bat                   # Gradle wrapper (Windows)
├── settings.gradle               # Configurações do projeto
└── README.md                     # Este arquivo
```

---

## ⚙️ Configuração do CI/CD

O projeto utiliza **GitHub Actions** para automação contínua:

### 🔄 Workflow: Java CI with Gradle

**Arquivo:** `.github/workflows/ci.yml`

**Triggers:**
- Push na branch `main`
- Pull Requests para a branch `main`

**Steps do Pipeline:**
1. ✅ Checkout do código
2. ✅ Setup JDK 21 (Temurin)
3. ✅ Cache do Gradle
4. ✅ Permissão de execução para gradlew
5. ✅ Build com Gradle

**Status:** [Veja os workflows](https://github.com/Agnelo-72/DevOps-Project/actions)

---

## 🏗️ Como Usar

### 1️⃣ Clonar o Repositório

```bash
git clone https://github.com/Agnelo-72/DevOps-Project.git
cd DevOps-Project/my-project
```

### 2️⃣ Build Local

Build da aplicação usando Gradle:

```bash
./gradlew build
```

### 3️⃣ Criar Imagem Docker

Build da imagem Docker chamada `java-app`:

```bash
docker build -t java-app .
```

### 4️⃣ Tagear Imagem

Atribuir tag à imagem para repositório:

```bash
docker tag java-app demo-app:java-1.0
```

### 5️⃣ Push para Repositório

```bash
docker push demo-app:java-1.0
```
---

## ✨ Próximos Passos

- [ ] Implementar testes unitários automatizados
- [ ] Adicionar coverage de código
- [ ] Deploy automatizado (CD)
- [ ] Monitoramento de performance

---

