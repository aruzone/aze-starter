# Aze Starter

🚀 Starter template with **Nx, Next.js, NestJS, Prisma, Docker, Kubernetes, Helm & ArgoCD** — production-ready monorepo for modern full-stack apps.

# 🚀 Full-Stack Starter Template

A production-ready **starter template** built with cutting-edge tools and frameworks to accelerate modern full-stack application development. Designed for scalability, developer productivity, and cloud-native deployments.

---

## ✨ Features

- **Monorepo with Nx** – Efficiently manage multiple apps and shared libraries in a single workspace.  
- **Frontend: Next.js** – React-based framework with SSR, SSG, API routes, and full TypeScript support.  
- **Backend: NestJS** – Scalable server-side framework for building reliable APIs and microservices.  
- **Database: Prisma ORM** – Type-safe database client with schema-driven migrations.  
- **Containerization: Docker** – Seamless local development and environment parity.  
- **Orchestration: Kubernetes** – Scalable deployments across clusters.  
- **Helm Charts** – Declarative configuration management for Kubernetes apps.  
- **GitOps with ArgoCD** – Continuous Delivery with version-controlled Kubernetes deployments.  

---

## 📂 Project Structure

```

.
├── apps/
│   ├── frontend/        # Next.js app
│   └── backend/         # NestJS app
├── libs/                # Shared libraries
├── prisma/              # Prisma schema & migrations
├── charts/              # Helm charts for K8s deployments
├── docker/              # Dockerfiles and Compose setup
└── infra/               # Kubernetes manifests & ArgoCD configs

````

---

## ⚡ Getting Started

### 1️⃣ Prerequisites
- Node.js (>=18)
- Docker & Docker Compose
- Kubernetes cluster (local: Minikube / Kind / k3d or cloud provider)
- Helm
- ArgoCD (optional for GitOps workflow)

### 2️⃣ Clone & Install
```bash
git clone https://github.com/<your-org>/<repo-name>.git
cd <repo-name>
npm install
````

### 3️⃣ Run Locally with Docker

```bash
docker-compose up --build
```

Frontend → [http://localhost:3000](http://localhost:3000)
Backend → [http://localhost:4000](http://localhost:4000)

### 4️⃣ Deploy to Kubernetes

```bash
helm install my-app ./charts
```

### 5️⃣ Continuous Delivery with ArgoCD

* Push your manifests to the `infra/` directory.
* ArgoCD will automatically sync and deploy.

---

## 🚀 Roadmap

* [ ] Add authentication (JWT / OAuth2)
* [ ] Integrate caching (Redis)
* [ ] Add CI/CD pipeline (GitHub Actions / GitLab CI)
* [ ] Expand Helm charts with configurable values

---

## 🤝 Contributing

Contributions are welcome! Please open an issue or submit a pull request.

---

## 📜 License

MIT License – feel free to use this template for your own projects.
