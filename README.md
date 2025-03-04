
# BoEngine - The Backend Engine for Ballads of Emeron

BoEngine is the core backend system powering **Ballads of Emeron**, a multiplayer idle RPG set in a fantasy world. It handles character progression, real-time combat, shared party systems, crafting, professions, and much more.

## 🚀 Features (WIP)

- Domain-Driven Design (DDD) architecture using Laravel 12
- Real-time and AFK combat systems
- Shared party progression across players
- Character progression from Novice to Class Specialist
- Advanced crafting and professions
- Fully open-source with potential premium features in the future

---

## ⚙️ Requirements

- Docker & Docker Compose
- PHP 8.3+ (only for tooling if not using Sail directly)
- Node.js 20+

---

## 🛠️ Getting Started with Laravel Sail

BoEngine uses **Laravel Sail** for local development, providing an easy-to-use Docker-based environment.

### 1. Clone the Repository

```bash
git clone https://github.com/BalladsOfEmeron/boengine.git
cd boengine
```

### 2. Environment Configuration

Duplicate the example environment file:

```bash
cp .env.example .env
```

### 3. Install Dependencies

Use Sail to install PHP and Node.js dependencies:

```bash
./vendor/bin/sail composer install
./vendor/bin/sail npm install
```

### 4. Start the Environment

```bash
./vendor/bin/sail up -d
```

### 5. Application Key & Database Setup

```bash
./vendor/bin/sail artisan key:generate
./vendor/bin/sail artisan migrate --seed
```

---

## ✅ Useful Commands

| Command | Description |
|---|---|
| `./vendor/bin/sail up -d` | Start the containers |
| `./vendor/bin/sail artisan migrate` | Run database migrations |
| `./vendor/bin/sail npm run dev` | Compile frontend assets (if needed) |
| `./vendor/bin/sail artisan` | Run Artisan commands |
| `./vendor/bin/sail tinker` | Interactive console |
| `./vendor/bin/sail test` | Run tests |

---

## 📚 Documentation

Technical documentation and architecture guidelines are (will be) available in the `boengine-docs` repository.

---

## 🌍 Contributing

Contributions are welcome! Please open issues or pull requests following our contribution guidelines.

---

## 📄 License

BoEngine is open-sourced software licensed under the [MIT license](LICENSE).

---

## ⚠️ Disclaimer

This project is under active development. Many features are work-in-progress and subject to major changes.
