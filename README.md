# ABNT2 Keyboard Fix on Linux (Resumo) ⌨
 
[🇧🇷 Português](#português) | [🇺🇸 English](#english)

---

## 🇧🇷 Português

### 👉 Sobre
Este projeto mostra como corrigir o layout do `teclado ABNT2`.⌨️

**Ambiente testado:**  
Linux Mint Cinnamon(Ubuntu-based) (Pode não funcionar corretamente em Wayland).

Para verificar seu ambiente gráfico execute no terminal:
 
```bash
echo $XDG_SESSION_TYPE

```

### 📌 Problema
Teclas como `ç`, `acentos` ou `símbolos` não funcionam corretamente.

---
   ### ⚒️ Solução 1 (Recomendado Via Interface)

✨ Antes de ir para o terminal, tente o caminho oficial ✨

1. Abra o menu **Teclado**  
2. Vá até a aba **Modelos**  
3. Clique no botão **Adicionar** e adicione **Português (Brasil)**  
4. Use as setas para colocá-lo no topo da lista  
5. (Opcional) Remova outros layouts
---
  ### ⚒️ Solução 2 (Temporária - apenas sessão)
  
Abra o terminal, execute e teste:
  
```bash
setxkbmap -layout br -variant abnt2
```
---
   ### ⚒️ Solução 3 (Persistente via Script de Inicialização)
   
 ✦︎Abra o menu **Aplicativos de Inicialização**    
 ✦︎Clique no botão **✚** > Comando personalizado.
 
- Nome: `Teclado ABNT2`
- Comando: `setxkbmap -model abnt2 -layout br -variant abnt2`
- Atraso: `2 segundos` (ajuda a garantir que o servidor gráfico já carregou)
---
---
 
## 🇺🇸 English
👉 About

This project shows how to fix issues with the ABNT2 keyboard layout on Linux.

Tested environment:
Linux Mint Cinnamon (Ubuntu-based)
⚠️ May not work properly on Wayland sessions.

To check your session type:
```bash
echo $XDG_SESSION_TYPE
```

📌 Problem

Keys like ç, accents, or symbols don’t work correctly.

---

⚒️ Solution 1 (Recommended - GUI)

✨ Before using the terminal, try the official method ✨

Open Keyboard settings  
Go to the Layouts tab  
Click Add and select Portuguese (Brazil)  
Move it to the top  
(Optional) Remove other layouts  
⚒️ Solution 2 (Temporary - session only)

Run in terminal:
```bash
setxkbmap -layout br -variant abnt2
```
---

⚒️ Solution 3 (Persistent - Startup)
Open Startup Applications
Click ✚ → Custom command

Fill in:

Name: ABNT2 Keyboard  
Command: setxkbmap -model abnt2 -layout br -variant abnt2  
Delay: 2 seconds  

    
