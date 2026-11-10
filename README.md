# Shop API - TP NestJS

API REST construite avec NestJS, TypeORM et MySQL. Elle gère des catégories, produits, clients et commandes.

---

## Stack technique

- **NestJS** — framework Node.js
- **TypeORM** — ORM pour MySQL
- **MySQL 8.4** — base de données
- **Swagger** — documentation API auto-générée
- **Docker Compose** — environnement de développement

---

## Lancer le projet

### 1. Démarrer la base de données

```bash
docker compose up db -d
```

### 2. Installer les dépendances

```bash
npm install
```

### 3. Configurer les variables d'environnement

Créer un fichier `.env` à la racine :

```env
DB_HOST=localhost
DB_PORT=3307
DB_USERNAME=shopuser
DB_PASSWORD=shoppass
DB_DATABASE=shop_db
PORT=3000
```

### 4. Lancer l'application

```bash
npm run start:dev
```

### 5. Accéder à la documentation Swagger

```
http://localhost:3000/api
```

---

## Modules

| Module      | Endpoints          |
|-------------|--------------------|
| Categories  | GET, POST          |
| Products    | GET, POST          |
| Clients     | GET, POST          |
| Orders      | GET, POST          |

---

## Captures d'écran

### Swagger UI

![Swagger UI](src/capture/swagger.png)

### GET Categories

![GET Categories](src/capture/get-categories.png)

### POST Category

![POST Category](src/capture/post-category.png)

### GET Products

![GET Products](src/capture/get-products.png)

### POST Product

![POST Product](src/capture/post-product.png)

### GET Clients

![GET Clients](src/capture/get-clients.png)

### POST Client

![POST Client](src/capture/post-client.png)

### GET Orders

![GET Orders](src/capture/get-orders.png)

### POST Order

![POST Order](src/capture/post-order.png)

---

## Build

```bash
npm run build
```

## Tests

```bash
npm run test
```
