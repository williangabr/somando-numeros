# ➕ Somando Números

Uma calculadora simples de soma feita com **HTML, CSS e JavaScript puro**. O usuário digita dois números, clica no botão **Somar** e o resultado aparece na tela.

![Prévia do projeto](./preview.png)

> 💡 Dica: tire um print da página, salve como `preview.png` na raiz do repositório e a imagem acima aparecerá aqui.

---

## 📋 Funcionalidades

- Entrada de dois números (inteiros ou decimais)
- Soma realizada ao clicar no botão
- Resultado exibido em um campo somente leitura
- Layout centralizado na tela, com card de bordas arredondadas e sombra

## 🛠️ Tecnologias utilizadas

- **HTML5**: estrutura da página
- **CSS3**: estilização (Flexbox, `box-shadow`, `border-radius`)
- **JavaScript**: lógica da soma e manipulação do DOM

## 🚀 Como executar

Não é preciso instalar nada.

1. Clone o repositório:

   ```bash
   git clone https://github.com/seu-usuario/somando-numeros.git
   ```

2. Entre na pasta do projeto:

   ```bash
   cd somando-numeros
   ```

3. Abra o arquivo `index.html` no seu navegador (dois cliques no arquivo ou botão direito > *Abrir com* > navegador).

## 📁 Estrutura do projeto

```
somando-numeros/
├── index.html
└── README.md
```

## ⚙️ Como funciona

A função `somar()` é chamada quando o botão é clicado. Ela busca os campos pelo `id`, converte os valores para número e exibe a soma no campo de resultado:

```javascript
function somar() {
    var tn1 = window.document.getElementById('txtn1')
    var tn2 = window.document.getElementById('txtn2')
    var res = window.document.getElementById('res')
    var n1 = Number(tn1.value)
    var n2 = Number(tn2.value)
    var s = n1 + n2
    res.value = s
}
```

O uso de `Number()` é importante: sem ele, o JavaScript trataria os valores dos inputs como texto e faria uma **concatenação** (`"2" + "3" = "23"`) em vez de uma soma.

## 🔮 Possíveis melhorias

- [ ] Adicionar as outras operações (subtração, multiplicação e divisão)
- [ ] Validar campos vazios e exibir uma mensagem de erro
- [ ] Permitir calcular ao pressionar a tecla **Enter**
- [ ] Separar o CSS e o JavaScript em arquivos próprios (`style.css` e `script.js`)
- [ ] Melhorar o layout para telas pequenas (responsividade)

## 👤 Autor

Feito por **Seu Nome**.

- GitHub: [@seu-usuario](https://github.com/seu-usuario)

## 📄 Licença

Este projeto está sob a licença MIT. Sinta-se à vontade para usar, estudar e modificar.
