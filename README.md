# TJ Studios

<p align="center">
  <strong>Build. Deploy. Manage. All in one place.</strong>
  <br />
  A self-hosted platform for managing the tools, infrastructure, and services behind your digital projects.
</p>

<p align="center">
  <img src="./badges/tj-studios.svg" alt="TJ Studios" width="260" height="64" />
  <br /><br />
  <img src="./badges/coming-soon.svg" alt="Coming Soon" />
  <img src="./badges/in-development.svg" alt="In Development" />
  <img src="./badges/self-hosted.svg" alt="Self-Hosted" />
  <img src="./badges/docker-ready.svg" alt="Docker Ready" />
</p>

---

## What is TJ Studios?

**TJ Studios is building a unified, self-hosted platform for operating digital projects and infrastructure.**

Instead of jumping between disconnected control panels, hosting tools, dashboards, and command-line utilities, TJ Studios aims to bring the essential parts of a modern development and hosting workflow into one place.

Through a central dashboard and connected services, users will be able to organize projects, deploy and manage applications, work with databases and files, monitor infrastructure, and access developer tools.

The goal is to give individuals, creators, and small teams more control over the services they build and run—with an architecture they can understand, operate, and grow.

> **One platform. Your infrastructure. Your projects. Your control.**

## Coming soon

TJ Studios is under active development. The following capabilities are planned for the platform and will be introduced as they are implemented, tested, and ready for release.

### Platform dashboard

A central control panel for the TJ Studios ecosystem.

- Manage projects, applications, and workspaces from one interface.
- View service health, deployment state, and resource usage.
- Configure platform services without constantly switching between tools.
- Manage account settings, access, and connected resources.

### Website and application hosting

A unified workflow for deploying and operating web projects.

- Create and configure website and application projects.
- Deploy projects and manage their runtime configuration.
- Connect domains and configure routing.
- View deployment status, logs, and service health.

### Container and server management

Tools for operating Docker-based workloads and the infrastructure that runs them.

- Create, start, stop, restart, and inspect containers.
- Organize services and deployments.
- Monitor connected hosts and system resources.
- Manage application environment configuration and operational settings.

### Database management

A simpler way to provision and manage application data services.

- Create and manage PostgreSQL databases.
- Organize database resources by project or workspace.
- Manage connection information and access permissions.
- Monitor database service availability.

### File and object storage

Centralized storage capabilities for projects and applications.

- Upload, organize, and manage files.
- Store application assets and project resources.
- Configure storage access and permissions.
- Connect storage resources to hosted applications.

### Developer tools and CLI

A developer-focused toolkit that connects local workflows to the TJ Studios platform.

- Use the planned TJ Studios CLI to interact with platform resources.
- Manage projects and deployments from the terminal.
- Connect development workflows to platform APIs.
- Use integrations to reduce repetitive administration.

### APIs and integrations

A shared API foundation for the dashboard, CLI, and external tools.

- Authenticated access to platform resources.
- API keys and permission-aware operations.
- Integration points for supported external services.
- Consistent APIs across platform capabilities.

### Business email

Managed email capabilities integrated into the broader TJ Studios experience.

- Connect supported email providers.
- Manage domains and mailbox provisioning.
- Organize email services alongside other project resources.
- View service configuration and account-level details.

### AI-assisted development

An area of planned exploration for improving developer workflows.

- Assistance with common development tasks.
- Tools for understanding and working with projects.
- Potential integrations with local and hosted development models.

*These features are planned capabilities, not a representation that they are currently available. Availability and scope may change as development progresses.*

## Platform principles

- **Self-hosted first** — keep infrastructure and deployment under the operator's control.
- **One connected experience** — bring projects and services together through a central dashboard.
- **Real infrastructure, real data** — status and resource information should come from actual services, not placeholder or browser-only state.
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

TJ Studios is being built incrementally. Current priorities include:

- [ ] Complete and harden the central authentication and session system.
- [ ] Establish the shared platform API and authorization model.
- [ ] Connect the dashboard to real backend services.
- [ ] Establish reliable PostgreSQL and Redis operations.
- [ ] Implement project, application, and container management.
- [ ] Add storage and deployment workflows.
- [ ] Improve infrastructure monitoring and operational visibility.
- [ ] Expand integrations, documentation, and developer tooling.
- [ ] Prepare the public website and platform launch.

The roadmap may change as features are tested against the needs of a real self-hosted environment.

## Who is TJ Studios for?

TJ Studios is being designed for:

- Independent developers managing their own infrastructure.
- Creators and small teams running websites and applications.
- Developers who want a unified place to manage projects and services.
- Operators who prefer self-hosted tools and direct control over their deployments.

## Website and platform availability

<badge color="discovery">Coming soon</badge>

The public TJ Studios website, central dashboard, and full platform experience are not yet launched. They are being developed alongside the underlying services.

Until launch, follow the individual projects and development activity through the [TJ Studios GitHub organization](https://github.com/tjstudios-llc).

For questions or project support, contact [support@tjstudios.xyz](mailto:support@tjstudios.xyz).

## Project status

TJ Studios is actively being developed. Features, interfaces, APIs, and deployment workflows may change while the platform is being built. Planned capabilities will be announced as they become ready, and each component should be evaluated using its own repository documentation before production use.

---

<p align="center">
  <strong>TJ Studios</strong>
  <br />
  Build with control. Operate with confidence.
  <br /><br />
  <strong>Website and platform — Coming Soon</strong>
  <br />
  <a href="https://github.com/tjstudios-llc">GitHub Organization</a>
</p>
