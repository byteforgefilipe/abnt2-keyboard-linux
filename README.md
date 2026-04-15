# ⌨️ ABNT2 Keyboard Fix on Linux (Resumo) ⌨
 
[🇧🇷 Português](#-português) | [🇺🇸 English](#-english)

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

✨Antes de ir para o terminal, tente o caminho oficial✨

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
 





    
