
# ☕ Coffee Delivery - Full Stack 


---

## Tecnologias Utilizadas

### Front-end
- [React](https://reactjs.org/)
- [TypeScript](https://www.typescriptlang.org/)
- [Styled-components](https://styled-components.com/)
- [Axios](https://axios-http.com/)

### Back-end
- [NestJS](https://nestjs.com/)
- [Prisma ORM](https://www.prisma.io/)
- [PostgreSQL](https://www.postgresql.org/)

---

## 🛠Funcionalidades

### Principais
- [x] Listar todos os cafés disponíveis (dados reais via API)
- [x] Visualizar detalhes dos cafés (nome, descrição, preço, tags, imagem)
- [x] Adicionar itens ao carrinho com quantidade personalizada
- [x] Finalizar pedido e enviar para o back-end
- [x] Cálculo automático de entrega e taxa conforme forma de pagamento

### Adicionais
- [x] Favoritar cafés (persistido no `localStorage`)
- [x] Persistência do carrinho com `localStorage`
- [x] Remoção de itens diretamente do carrinho
- [x] Requisições otimizadas com Axios

---

## Estrutura de Diretórios

```
coffee-delivery/
├── backend/
│   ├── src/
│   │   ├── coffees/
│   │   ├── cart/
│   │   ├── order/
│   │   └── prisma/
│   └── prisma/schema.prisma
├── frontend/
│   ├── src/
│   │   ├── pages/
│   │   ├── components/
│   │   ├── contexts/
│   │   └── styles/
```

---

##  Como rodar o projeto localmente

### 1. Clone o repositório

```bash
git clone https://github.com/seu-usuario/coffee_delivery_fullstack.git
cd coffee-delivery
```

### 2. Instale as dependências, lembrando que são projetos com estruturas próprias

```bash
# Back-end
cd backend
npm install

# Front-end
cd ../frontend
npm install
```

### 3. Configure o banco de dados

Certifique-se de que você tem o PostgreSQL rodando, usei o neon.db pela praticidade. Crie um banco e configure o `.env`:

```env
# backend/.env
DATABASE_URL=postgresql://usuario:senha@localhost:5432/coffee_delivery
```

### 4. Execute as migrações

```bash
cd backend
npx prisma migrate dev
```

### 5. Rode o servidor

```bash
npm run start:dev
```

### 6. Rode o front-end

```bash
cd ../frontend
npm run dev
```




Desenvolvido por Ana Laressa
