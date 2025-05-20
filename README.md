# 🛒 CP3-ANDROID — Lista de Compras em Kotlin

Projeto Android feito em Kotlin que permite **adicionar**, **editar** e **exibir produtos** numa lista de compras de forma simples e prática.

## 📂 Estrutura dos arquivos Kotlin

### 📱 `MainActivity.kt`
Esse é o arquivo **principal**, o que bota tudo pra rodar.  
Aqui rola:
- A lista de produtos via **RecyclerView**.
- Ações como **adicionar**, **editar** ou **remover** um item.
- A conexão com o `Service.kt` pra puxar os dados.

💡 Resumo: mostra a lista, escuta os cliques e atualiza tudo em tempo real.

---

### 📦 `Model.kt`
Define a classe `Produto`, usada pra guardar os dados dos itens.

Campos:
- `id`: identifica cada produto (tipo CPF de item 🧾).
- `nome`: o que você quer comprar (arroz, feijão, batata frita...).
- `quantidade`: quantas unidades vai levar.

---

### 🛠️ `Service.kt`
Aqui fica a lógica do app, o famoso “faz-tudo”:
- Adiciona novos produtos
- Remove produtos
- Atualiza dados
- Lista geral da compra

---

### 🧪 `Factory.kt`
Responsável por criar e **reaproveitar instâncias** do `ProdutoService`.  
Evita criar o mesmo objeto várias vezes — **injeção de dependência** na moral.


## 📸 Evidências

### App rodando no emulador e código
![EvidenciaKotlinCp](https://github.com/user-attachments/assets/ebfa0756-eb3c-48ee-86d6-a12020f2cfda)




