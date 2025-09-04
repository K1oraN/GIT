# 🚀 Guia Completo do Git e GitHub: Do Início ao Avançado  

Um guia passo a passo para aprender **Git** e **GitHub** do zero até o nível avançado.  
Aqui você encontrará desde a instalação, configuração inicial e criação de repositórios, até fluxos de trabalho colaborativos, boas práticas e comandos avançados.  

> 🎯 Objetivo: Ajudar iniciantes e desenvolvedores a dominarem Git e GitHub de forma prática e organizada.  

---

## 🔰 Introdução  

- **Git** → Sistema de controle de versão distribuído, permitindo rastrear alterações no código, voltar a versões anteriores e trabalhar em funcionalidades isoladas.  
- **GitHub** → Plataforma online para hospedar repositórios Git, colaborar em projetos, revisar código e gerenciar equipes.  

---

## ⚙️ Instalação e Configuração Inicial  

### Instalando o Git  
- **Windows** → [Baixar Git](https://git-scm.com/download/win)  
- **MacOS** → Verifique com `git --version` (se não estiver instalado, será solicitado pelo Xcode).  
- **Linux (Ubuntu/Debian)** →  
```bash
sudo apt-get install git
```  

### Configurando suas Informações  
```bash
git config --global user.name "Seu Nome"
git config --global user.email "seu@email.com"
```  

> ℹ️ Essas informações são associadas a cada *commit*.  

---

## 📂 Criando e Conectando um Repositório  

### Criando Repositório Local (`git init`)  
```bash
cd /caminho/para/projeto
git init
```  

### Criando Repositório no GitHub  
1. Vá em **New Repository**  
2. Dê um nome e descrição  
3. Defina como público ou privado  
4. Não adicione arquivos extras (README, .gitignore, license) se já iniciou localmente.  

### Conectando ao Repositório Remoto  
```bash
git remote add origin https://github.com/usuario/repositorio.git
git branch -M main
git push -u origin main
```  

---

## 🛠️ O Fluxo Básico do Git: Mexendo, Alterando e Salvando  

**Etapas do Git:**  
1. 📁 Working Directory → Onde você edita os arquivos  
2. 📦 Staging Area → Onde adiciona arquivos para commit  
3. 🗃️ Local Repository → Onde ficam os commits salvos  

### Exemplos:  
```bash
git status         # Verifica mudanças
git add .          # Adiciona todos os arquivos
git commit -m "mensagem clara"
git push origin main
```  

---

## 🌿 Trabalhando com Branches (Ramos)  

Criando e alternando entre branches:  
```bash
git checkout -b nova-feature
```  

Mesclando de volta para a `main`:  
```bash
git checkout main
git merge nova-feature
```  

> ⚠️ Caso haja conflitos, edite os arquivos manualmente e finalize com `git commit`.  

---

## 🔄 Mantendo o Repositório Atualizado  

```bash
git fetch origin    # Baixa alterações sem mesclar
git pull origin main # Baixa e mescla automaticamente
```  

---

## 🧹 Desfazendo Alterações  

- Descartar mudanças em arquivo:  
```bash
git checkout -- arquivo.txt
```  

- Remover da staging area:  
```bash
git reset HEAD arquivo.txt
```  

- Reverter commit:  
```bash
git revert HEAD
```  

---

## 🧰 Comandos Úteis  

- Histórico detalhado:  
```bash
git log
git log --oneline
```  

- Clonar repositório existente:  
```bash
git clone https://github.com/usuario/repositorio.git
```  

- Arquivo `.gitignore`:  
```
node_modules/
.env
*.log
```  

---

## 📌 Boas Práticas  

- Escreva mensagens de commit curtas e claras.  
- Use branches para cada feature ou correção.  
- Sincronize sempre com `git pull` antes de iniciar alterações.  
- Mantenha o repositório limpo com `.gitignore`.  

---

## 📚 Recursos Adicionais  

- 📖 [Documentação Oficial do Git](https://git-scm.com/doc)  
- 🎥 [Git e GitHub para Iniciantes - Curso em Vídeo](https://www.youtube.com/watch?v=UBAX-13g8OM)  
- 📘 [Pro Git Book (gratuito)](https://git-scm.com/book/pt-br/v2)  

---

## 🤝 Contribuição  

Contribuições são bem-vindas!  
1. Faça um **fork** do repositório  
2. Crie uma **branch** para sua feature (`git checkout -b minha-feature`)  
3. Faça commit das alterações (`git commit -m 'Adicionei minha feature'`)  
4. Faça push para a branch (`git push origin minha-feature`)  
5. Abra um **Pull Request** 🎉  

---

✨ **Agora você tem um guia organizado e visual para dominar Git e GitHub!** 🚀  
