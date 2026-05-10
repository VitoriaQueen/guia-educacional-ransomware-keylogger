# Exemplo Educacional de Criptografia de Arquivos

**Exemplos apresentados com propósito educucativo.**

### Bibliotecas

from cryptography.fernet import Fernet

chave = Fernet.generate_key()

fernet = Fernet(chave)

mensagem = b"arquivo de teste"

criptografado = fernet.encrypt(mensagem)

print(criptografado)

Explicação:

- Demonstra uso de criptografia
- Não altera arquivos reais
- Simula conceito utilizado por ransomwares

<br>

---

# Exemplo de código de keyloggers

### Bibliotecas

from pynput import keyboard

def ao_pressionar(tecla):

    print(f"Tecla pressionada: {tecla}")

with keyboard.Listener(on_press=ao_pressionar) as listener:
   
    listener.join()

Explicação:

- O script monitora teclas pressionadas
- Exibe as teclas no terminal
- Não envia dados pela rede
    

