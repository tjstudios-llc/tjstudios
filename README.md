# TJ Studios

<p align="center">
  <strong>Build. Deploy. Manage. All in one place.</strong>
  <br />
  A self-hosted platform for managing the tools, infrastructure, and services behind your digital projects.
</p>

<p align="center">
  <a href="https://tjstudios.xyz"><img src="https://img.shields.io/badge/Website-tjstudios.xyz-111827?style=for-the-badge&logo=googlechrome&logoColor=white" alt="TJ Studios website" /></a>
  <img src="https://img.shields.io/badge/Status-In%20Development-f59e0b?style=for-the-badge" alt="In development" />
  <img src="https://img.shields.io/badge/Deployment-Self--Hosted-2563eb?style=for-the-badge&logo=docker&logoColor=white" alt="Self-hosted" />
  <img src="https://img.shields.io/badge/Runtime-Node.js%2022%2B-339933?style=for-the-badge&logo=nodedotjs&logoColor=white" alt="Node.js 22+" />
  <img src="https://img.shields.io/badge/Database-PostgreSQL-4169e1?style=for-the-badge&logo=postgresql&logoColor=white" alt="PostgreSQL" />
  <img src="https://img.shields.io/badge/Containerization-Docker-2496ed?style=for-the-badge&logo=docker&logoColor=white" alt="Docker" />
</p>

---

## What is TJ Studios?

**TJ Studios is building a unified, self-hosted platform for operating digital projects and infrastructure.**

Instead of jumping between disconnected control panels, hosting tools, dashboards, and command-line utilities, TJ Studios aims to bring the essential parts of a modern development and hosting workflow into one place.

From a central dashboard, users will be able to organize projects, deploy and manage applications, work with databases and files, monitor services, and access developer tools.

The goal is straightforward: give individuals, creators, and small teams more control over the services they build and run—with an architecture they can understand, operate, and grow.

> **One platform. Your infrastructure. Your projects. Your control.**

## What we're building

TJ Studios is being developed as a modular platform. Each capability is intended to work as part of a connected system while remaining independently maintainable.

| Platform area | What it is intended to provide |
| --- | --- |
| **Application hosting** | Create, deploy, configure, and manage application services. |
| **Website hosting** | Manage websites, domains, and deployment workflows. |
| **Container management** | Control Docker-based workloads, services, and deployments. |
| **Database management** | Provision and manage PostgreSQL databases and related resources. |
| **File and object storage** | Organize project files and application assets through a unified interface. |
| **Developer tools** | Access project utilities, integrations, and development workflows. |
| **Infrastructure management** | Monitor hosts, service health, resource usage, and connected infrastructure. |
| **APIs and integrations** | Connect platform capabilities to external tools and custom workflows. |
| **Business email** | Integrate managed email services and provide mailbox and domain management. |
| **AI-assisted development** | Explore tools that can help with development and project workflows. |

These are product goals, not a claim that every feature is currently available. TJ Studios is actively under development.

## Platform principles

- **Self-hosted first** — keep infrastructure and deployment under the operator's control.
- **One connected experience** — bring projects and services together through a central dashboard.
- **Real infrastructure, real data** — platform status and resource information should come from actual services, not placeholder or browser-only state.
- **Modular by design** — keep platform capabilities separated into maintainable services and components.
- **Security by default** — build around authentication, authorization, tenant isolation, validation, and auditable operations.
- **Practical and accessible** — make common infrastructure tasks manageable without requiring every user to work directly with server commands.

## Architecture direction

The intended architecture separates the user experience, application platform, and infrastructure execution responsibilities.

```text
                         TJ Studios
                              |
                    Central Dashboard
                              |
                       Platform API
                              |
             +----------------+----------------+
             |                |                |
         Identity         Projects          Platform
       & Access          & Workspaces       Services
             |                |                |
             +----------------+----------------+
                              |
                    Infrastructure Layer
                              |
             +----------------+----------------+
             |                |                |
           Docker          PostgreSQL         Redis
             |                |                |
       Applications       Platform Data     Queues &
       & Containers       & Metadata         Caching
                              |
                     Storage & Hosting Nodes
```

This is the target architecture and may evolve as implementation and operational requirements are validated.

### Core technology direction

| Layer | Current direction |
| --- | --- |
| Dashboard | Next.js App Router, React, and Tailwind CSS |
| Backend services | Node.js 22+ and Fastify |
| Data access | Prisma ORM |
| Primary database | PostgreSQL |
| Caching and queues | Redis |
| Infrastructure | Docker and Docker Compose |
| Routing and edge access | Nginx Proxy Manager and Cloudflare |
| Developer workflow | Git, GitHub, and command-line tooling |

Individual repositories may use additional technologies where they fit their specific responsibilities.

## Project ecosystem

TJ Studios is made up of focused projects that support the broader ecosystem.

| Project | Purpose |
| --- | --- |
| **TJ Studios Dashboard** | The planned central interface for managing the platform. |
| **Core Services** | The application backend foundation for identity, platform APIs, and shared services. |
| **TJ Studios CLI** | The planned command-line interface for interacting with TJ Studios. |
| **ForgeKit** | A separate local-first developer tool for generating application projects. |

The platform is designed to grow through independently developed components rather than forcing every tool into one large application.

## Development roadmap

TJ Studios is being built incrementally. Current priorities are:

- [ ] Establish and harden the central authentication and session system.
- [ ] Build the shared platform API and authorization model.
- [ ] Connect the dashboard to real backend services.
- [ ] Establish reliable PostgreSQL and Redis operations.
- [ ] Implement project, application, and container management.
- [ ] Add storage and deployment workflows.
- [ ] Improve infrastructure monitoring and operational visibility.
- [ ] Expand integrations, documentation, and developer tooling.

The roadmap may change as features are tested against the needs of a real self-hosted environment.

## Who is TJ Studios for?

TJ Studios is being designed for:

- Independent developers managing their own infrastructure.
- Creators and small teams running websites and applications.
- Developers who want a unified place to manage projects and services.
- Operators who prefer self-hosted tools and direct control over their deployments.

## Get started

TJ Studios is currently in development, so the complete platform is not yet available as a stable, one-command installation.

For now, explore the organization's repositories to follow individual components and their progress:

- **Website:** [tjstudios.xyz](https://tjstudios.xyz)
- **GitHub organization:** [github.com/tjstudios-llc](https://github.com/tjstudios-llc)
- **Dashboard:** [dashboard.tjstudios.xyz](https://dashboard.tjstudios.xyz)
- **Documentation:** [docs.tjstudios.xyz](https://docs.tjstudios.xyz)

For questions or project support, contact [support@tjstudios.xyz](mailto:support@tjstudios.xyz).

## Project status

TJ Studios is an actively developed project. Features, interfaces, APIs, and deployment workflows may change while the platform is being built. Check the relevant repository documentation before relying on a component in a production environment.

---

<p align="center">
  <strong>TJ Studios</strong>
  <br />
  Build with control. Operate with confidence.
  <br /><br />
  <a href="https://tjstudios.xyz">Website</a> ·
  <a href="https://github.com/tjstudios-llc">GitHub</a> ·
  <a href="https://docs.tjstudios.xyz">Documentation</a>
</p>
