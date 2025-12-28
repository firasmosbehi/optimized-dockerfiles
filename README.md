![Banner](https://github.com/user-attachments/assets/cf63120c-d365-404d-9343-c89400453fa9)

# 🚀 Optimized Dockerfiles Collection

A curated collection of **production-ready**, **DevOps-focused**, and **highly optimized Dockerfiles** for 25+ popular frameworks across 5 programming languages.

> **Learn Docker best practices through real-world examples**
> Each example demonstrates multi-stage builds, image optimization, security hardening, and production deployment patterns.

## 📊 Repository Statistics

- **25 Frameworks** across 5 languages
- **Average 70-85% image size reduction** vs basic builds
- **50+ Dockerfiles** (optimized + basic versions)
- **Production-ready** with health checks and security hardening
- **CI/CD automated** builds with GitHub Actions

## 🎯 Repository Goals

- ✅ Provide **real-world Dockerfile examples** for multiple technologies
- ✅ Demonstrate **multi-stage builds**, **image minimization**, and **secure production setups**
- ✅ Compare **optimized** vs **non-optimized** approaches with benchmarks
- ✅ Offer **DevOps patterns** for CI/CD, caching, static serving, and deployment
- ✅ Serve as a reference for building production-grade Docker images

---

## 📂 Repository Structure

```txt
optimized-dockerfiles/
│
├── javascript/              # JavaScript/TypeScript (8 frameworks)
│   ├── frontend/            # 5 frontend frameworks
│   │   ├── react/          # React + Vite (CSR)
│   │   ├── nextjs/         # Next.js 15 with App Router (SSR)
│   │   ├── angular/        # Angular Universal (SSR)
│   │   ├── vue/            # Vue 3 + Vite (CSR)
│   │   └── svelte/         # SvelteKit (SSR)
│   │
│   └── backend/            # 3 backend frameworks
│       ├── express/        # Express.js (classic REST)
│       ├── fastify/        # Fastify (high-performance)
│       └── nestjs/         # NestJS (enterprise TypeScript)
│
├── python/                 # Python (4 frameworks)
│   ├── fastapi/            # FastAPI (async API)
│   ├── flask/              # Flask (lightweight web)
│   ├── django/             # Django + DRF (full-featured)
│   └── streamlit/          # Streamlit (data apps)
│
├── java/                   # Java (4 frameworks)
│   ├── spring-boot/        # Spring Boot (enterprise)
│   ├── quarkus/            # Quarkus (Kubernetes-native)
│   ├── micronaut/          # Micronaut (compile-time DI)
│   └── vertx/              # Vert.x (reactive toolkit)
│
├── ruby/                   # Ruby (4 frameworks)
│   ├── rails/              # Ruby on Rails (full-stack MVC)
│   ├── sinatra/            # Sinatra (lightweight DSL)
│   ├── hanami/             # Hanami (modern architecture)
│   └── grape/              # Grape (REST API)
│
├── dotnet/                 # .NET/C# (4 frameworks)
│   ├── aspnet-core/        # ASP.NET Core Web API
│   ├── minimal-api/        # Minimal APIs
│   ├── blazor-server/      # Blazor Server (interactive UI)
│   └── grpc/               # gRPC (high-performance RPC)
│
└── .github/workflows/      # CI/CD pipelines
    └── docker-build.yml    # Automated build workflow
```

### What's in Each Directory?

Every framework directory contains:

- 📦 **Optimized Dockerfile** - Multi-stage build, production-ready
- 📦 **Dockerfile.basic** - Non-optimized version for comparison
- ⚙️ **Configuration files** - Framework-specific configs (Nginx, Poetry, pom.xml, etc.)
- 📚 **Comprehensive README.md** - Setup instructions, benchmarks, best practices
- 🚫 **.dockerignore** - Optimized build context

---

## 🚀 Quick Start

### Clone the Repository

```bash
git clone https://github.com/yourusername/optimized-dockerfiles.git
cd optimized-dockerfiles
```

### Build Any Framework

```bash
# Navigate to any framework
cd javascript/frontend/react

# Build optimized image
docker build -t my-app:optimized -f Dockerfile .

# Or build basic version for comparison
docker build -t my-app:basic -f Dockerfile.basic .

# Run the container
docker run -p 3000:3000 my-app:optimized
```

### Framework Quick Navigation

<details>
<summary><b>JavaScript/TypeScript Frameworks (8)</b></summary>

**Frontend (5)**
```bash
cd javascript/frontend/react      # React + Vite SPA
cd javascript/frontend/nextjs     # Next.js with SSR
cd javascript/frontend/angular    # Angular Universal
cd javascript/frontend/vue        # Vue 3 + Vite
cd javascript/frontend/svelte     # SvelteKit
```

**Backend (3)**
```bash
cd javascript/backend/express     # Express.js REST API
cd javascript/backend/fastify     # Fastify high-performance API
cd javascript/backend/nestjs      # NestJS enterprise TypeScript
```
</details>

<details>
<summary><b>Python Frameworks (4)</b></summary>

```bash
cd python/fastapi       # FastAPI async API
cd python/flask         # Flask lightweight web
cd python/django        # Django + DRF full-stack
cd python/streamlit     # Streamlit data apps
```
</details>

<details>
<summary><b>Java Frameworks (4)</b></summary>

```bash
cd java/spring-boot     # Spring Boot enterprise
cd java/quarkus         # Quarkus Kubernetes-native
cd java/micronaut       # Micronaut compile-time DI
cd java/vertx           # Vert.x reactive toolkit
```
</details>

<details>
<summary><b>Ruby Frameworks (4)</b></summary>

```bash
cd ruby/rails           # Ruby on Rails full-stack MVC
cd ruby/sinatra         # Sinatra lightweight DSL
cd ruby/hanami          # Hanami modern architecture
cd ruby/grape           # Grape REST API framework
```
</details>

<details>
<summary><b>.NET/C# Frameworks (4)</b></summary>

```bash
cd dotnet/aspnet-core   # ASP.NET Core Web API
cd dotnet/minimal-api   # Minimal APIs
cd dotnet/blazor-server # Blazor Server interactive UI
cd dotnet/grpc          # gRPC high-performance RPC
```
</details>

---

## 📊 Framework Comparison Matrix

### Image Size Comparison

| Language | Framework      | Optimized Size | Basic Size | Savings  | Startup Time |
|----------|----------------|----------------|------------|----------|--------------|
| **JS**   | React          | ~25 MB         | ~1.2 GB    | **~98%** | <1s          |
| **JS**   | Next.js        | ~180 MB        | ~1.5 GB    | **~88%** | 2-3s         |
| **JS**   | Express        | ~100 MB        | ~1.2 GB    | **~92%** | <1s          |
| **Python** | FastAPI      | ~50 MB         | ~1 GB      | **~95%** | 1-2s         |
| **Python** | Django       | ~80 MB         | ~1.2 GB    | **~93%** | 2-3s         |
| **Java** | Spring Boot    | ~200 MB        | ~600 MB    | **~66%** | 10-15s       |
| **Java** | Quarkus        | ~180 MB        | ~600 MB    | **~70%** | 1-3s         |
| **Ruby** | Rails          | ~150 MB        | ~1.2 GB    | **~88%** | 2-5s         |
| **Ruby** | Sinatra        | ~50 MB         | ~1 GB      | **~95%** | <1s          |
| **.NET** | ASP.NET Core   | ~110 MB        | ~700 MB    | **~84%** | 1-2s         |
| **.NET** | Minimal API    | ~105 MB        | ~700 MB    | **~85%** | <1s          |

### Performance Characteristics

| Framework Type | Avg Optimized Size | Avg Startup | Best For                        |
|----------------|-------------------|-------------|---------------------------------|
| **Frontend**   | ~25-180 MB        | <1-3s       | Static sites, SPAs              |
| **Backend API**| ~50-200 MB        | <1-5s       | Microservices, REST APIs        |
| **Full-Stack** | ~80-200 MB        | 2-10s       | Complete web applications       |
| **Enterprise** | ~150-200 MB       | 5-15s       | Large-scale production apps     |

---

## 📌 Complete Framework List

### JavaScript/TypeScript Frontend

| Framework     | Description                      | Status     | Path                          |
|---------------|----------------------------------|------------|-------------------------------|
| **React**     | React + Vite (CSR)               | ✅ DONE    | `javascript/frontend/react/`  |
| **Next.js**   | Next.js 15 (App Router + SSR)    | ✅ DONE    | `javascript/frontend/nextjs/` |
| **Angular**   | Angular Universal (SSR)          | ✅ DONE    | `javascript/frontend/angular/`|
| **Vue**       | Vue 3 + Vite (CSR)               | ✅ DONE    | `javascript/frontend/vue/`    |
| **SvelteKit** | SvelteKit (SSR)                  | ✅ DONE    | `javascript/frontend/svelte/` |

### JavaScript/TypeScript Backend

| Framework     | Description                      | Status     | Path                           |
|---------------|----------------------------------|------------|--------------------------------|
| **Express**   | Classic REST API framework       | ✅ DONE    | `javascript/backend/express/`  |
| **Fastify**   | High-performance API framework   | ✅ DONE    | `javascript/backend/fastify/`  |
| **NestJS**    | Enterprise TypeScript framework  | ✅ DONE    | `javascript/backend/nestjs/`   |

### Python Frameworks

| Framework     | Description                      | Status     | Path                 |
|---------------|----------------------------------|------------|----------------------|
| **FastAPI**   | Modern async API framework       | ✅ DONE    | `python/fastapi/`    |
| **Flask**     | Lightweight web framework        | ✅ DONE    | `python/flask/`      |
| **Django**    | Full-featured + DRF              | ✅ DONE    | `python/django/`     |
| **Streamlit** | Data apps & dashboards           | ✅ DONE    | `python/streamlit/`  |

### Java Frameworks

| Framework       | Description                      | Status     | Path                   |
|-----------------|----------------------------------|------------|------------------------|
| **Spring Boot** | Enterprise Java framework        | ✅ DONE    | `java/spring-boot/`    |
| **Quarkus**     | Kubernetes-native Java           | ✅ DONE    | `java/quarkus/`        |
| **Micronaut**   | Compile-time DI framework        | ✅ DONE    | `java/micronaut/`      |
| **Vert.x**      | Reactive toolkit                 | ✅ DONE    | `java/vertx/`          |

### Ruby Frameworks

| Framework       | Description                      | Status     | Path                   |
|-----------------|----------------------------------|------------|------------------------|
| **Rails**       | Full-stack MVC framework         | ✅ DONE    | `ruby/rails/`          |
| **Sinatra**     | Lightweight DSL web framework    | ✅ DONE    | `ruby/sinatra/`        |
| **Hanami**      | Modern architecture framework    | ✅ DONE    | `ruby/hanami/`         |
| **Grape**       | REST API framework               | ✅ DONE    | `ruby/grape/`          |

### .NET/C# Frameworks

| Framework          | Description                      | Status     | Path                      |
|--------------------|----------------------------------|------------|---------------------------|
| **ASP.NET Core**   | Full-featured Web API            | ✅ DONE    | `dotnet/aspnet-core/`     |
| **Minimal API**    | Lightweight HTTP APIs            | ✅ DONE    | `dotnet/minimal-api/`     |
| **Blazor Server**  | Interactive web UI with C#       | ✅ DONE    | `dotnet/blazor-server/`   |
| **gRPC**           | High-performance RPC framework   | ✅ DONE    | `dotnet/grpc/`            |

### Coming Soon

| Language      | Frameworks/Tools                 | Status     |
|---------------|----------------------------------|------------|
| **Go**        | Fiber, Gin, Echo                 | 🔜 Planned |
| **Rust**      | Axum, Actix-web                  | 🔜 Planned |
| **PHP**       | Laravel, Symfony                 | 🔜 Planned |

---

## 🔄 CI/CD Pipeline

This repository uses a **single, intelligent GitHub Actions workflow** that automatically:

✅ **Detects changed frameworks** using path filters
✅ **Builds only affected frameworks** for efficiency
✅ **Runs builds in parallel** when multiple frameworks change
✅ **Pushes to Docker Hub** with semantic tagging
✅ **Uses layer caching** for faster subsequent builds
✅ **Supports manual triggers** via workflow dispatch

### Workflow Features

- **Smart Detection**: Only builds what changed
- **Parallel Execution**: Multiple framework builds run concurrently
- **Layer Caching**: Pulls from Docker Hub for faster rebuilds
- **Dual Builds**: Creates both optimized and basic images
- **Commit Tagging**: Images tagged with `latest` and commit SHA
- **Build Summaries**: GitHub Actions summary with pushed images

### Docker Images

All images are pushed to Docker Hub with the following naming convention:

```
<username>/optimized-dockerfiles:<framework>-latest
<username>/optimized-dockerfiles:<framework>-<commit-sha>
<username>/optimized-dockerfiles:<framework>-basic-latest
```

**Examples:**
```
optimized-dockerfiles:react-latest
optimized-dockerfiles:fastapi-abc123
optimized-dockerfiles:spring-boot-basic-latest
```

### Manual Builds

Trigger builds manually via GitHub Actions:

```bash
# Via GitHub UI: Actions → Build and Push → Run workflow
# Specify framework path: javascript/frontend/react
```

---

## 🐳 Docker Best Practices Implemented

### ✔️ Multi-Stage Builds

Every optimized Dockerfile uses multi-stage builds:
- **Build stage**: Compile, install dependencies
- **Runtime stage**: Copy only necessary artifacts

**Benefits**: 60-95% smaller final images

### ✔️ Minimal Base Images

Strategic base image selection:
- **Alpine Linux**: Most frameworks (~5 MB base)
- **Distroless**: Java/Python options
- **Slim variants**: When Alpine isn't available

### ✔️ Layer Caching Optimization

Dependency installation before source code:
```dockerfile
# Copy dependency files first (rarely change)
COPY package.json package-lock.json ./
RUN npm ci --production

# Copy source code last (changes frequently)
COPY . .
```

### ✔️ Security Hardening

- ✅ **Non-root users**: All containers run as unprivileged users
- ✅ **Minimal attack surface**: Only runtime dependencies included
- ✅ **No secrets**: Credentials via environment variables
- ✅ **Read-only filesystem**: Where applicable

### ✔️ Production Optimizations

- Health checks for orchestration
- Proper signal handling
- Environment-based configuration
- Logging to stdout/stderr
- Graceful shutdown support

### ✔️ Static Asset Serving

Frontend frameworks use **Nginx** for production:
- Gzip/Brotli compression
- Proper caching headers
- SPA routing support
- Security headers

---

## 🛠️ Usage Examples

### Build and Run

```bash
# Build
docker build -t myapp:v1 .

# Run with port mapping
docker run -p 8080:8080 myapp:v1

# Run with environment variables
docker run -e NODE_ENV=production -p 8080:8080 myapp:v1

# Run in detached mode
docker run -d -p 8080:8080 myapp:v1
```

### Docker Compose

```yaml
version: '3.8'
services:
  app:
    build:
      context: ./javascript/frontend/react
      dockerfile: Dockerfile
    ports:
      - "3000:80"
    environment:
      - NODE_ENV=production
    restart: unless-stopped
```

### Kubernetes Deployment

```yaml
apiVersion: apps/v1
kind: Deployment
metadata:
  name: myapp
spec:
  replicas: 3
  selector:
    matchLabels:
      app: myapp
  template:
    metadata:
      labels:
        app: myapp
    spec:
      containers:
      - name: myapp
        image: username/optimized-dockerfiles:react-latest
        ports:
        - containerPort: 80
        livenessProbe:
          httpGet:
            path: /health
            port: 80
        readinessProbe:
          httpGet:
            path: /health
            port: 80
```

---

## 📚 Learning Resources

Each framework README includes:

- 📖 **Architecture explanations** - How the Dockerfile works
- 📊 **Performance benchmarks** - Size and speed comparisons
- 🔧 **Configuration options** - Customization guide
- 🚀 **Deployment examples** - Kubernetes, Docker Compose
- 💡 **Best practices** - Production tips and patterns
- 🐛 **Troubleshooting** - Common issues and solutions

---

## 🤝 Contributing

Contributions are welcome! Here's how you can help:

### Adding New Frameworks

1. Fork the repository
2. Create a new directory: `language/framework/`
3. Add optimized and basic Dockerfiles
4. Include comprehensive README.md
5. Update main README.md
6. Submit a pull request

### Improvements

- Optimize existing Dockerfiles
- Add better documentation
- Report issues or bugs
- Suggest new frameworks
- Improve CI/CD workflow

### Guidelines

- Follow existing structure and naming conventions
- Include both optimized and basic versions
- Add meaningful benchmarks
- Document all optimizations
- Test builds locally before submitting

---

## 📜 License

MIT License — free to use, modify, and learn from.

See [LICENSE](LICENSE) file for details.

---

## 🙏 Acknowledgments

- Inspired by Docker best practices from the community
- Framework-specific optimizations from official documentation
- CI/CD patterns from DevOps best practices

---

## 📬 Contact

**Firas Mosbahi**

- GitHub: [@yourusername](https://github.com/yourusername)
- Focus: DevOps excellence and reproducible builds

---

<div align="center">

**⭐ Star this repo if you find it helpful!**

**Made with ❤️ for the DevOps community**

</div>
