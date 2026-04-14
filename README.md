# ⌨️ ABNT2 Keyboard Fix on Linux (Resumo)

[🇧🇷 Português](#-português) | [🇺🇸 English](#-english)

---

## 🇧🇷 Português

### 📌 Sobre
Este projeto mostra como corrigir o layout do teclado ABNT2.

**Ambiente testado:**  
Linux Mint Cinnamon(Ubuntu-based) (Pode não funcionar em Wayland).

Para verificar seu ambiente grafico execute no terminal: 

```bash
echo $XDG_SESSION_TYPE
```

### ⚠️ Problema
Teclas como `ç`, acentos ou símbolos não funcionam corretamente.

---
   ---------------------------------------------------------
   ### ⚙️ Solução 1 (Recomendado Via Interface)

Antes de ir para o terminal, tente o caminho oficial

  Abra o Menu > Teclado.
  Vá na aba Layouts.
  Clique no botão + e adicione Português (Brasil).
  Use as setas para deixá-lo no topo da lista.
  (Apagar as outras opções é opcional contanto que o Português (Brasil) esteja em primeiro)
  ----------------------------------------------------------
  ### ⚙️ Solução 2 (Temporária - apenas sessão)
  
  Abra o terminal, execute e teste:
  
    ```bash setxkbmap -layout br -variant abnt2


 ###  ----------------------------------------------------------
   ### ⚙️ Solução 3 (Persistente via Script de Inicialização)
Abra o gerenciador de Aplicativos de Inicialização.

Clique em Adicionar > Comando Personalizado.

Preencha os campos:
    Nome: Fix Teclado ABNT2
    Comando: setxkbmap -model abnt2 -layout br -variant abnt2
    Atraso na inicialização: 2 segundos (ajuda a garantir que o servidor gráfico já carregou).
    
