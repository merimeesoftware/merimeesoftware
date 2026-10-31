<!--
  Personal GitHub user profile README (not an organization).
  For user accounts, the special repo must be named <username>/<username>
  and this file must live at the repository ROOT as README.md.

  Do NOT use .github/profile/README.md or profile/README.md —
  those paths are for organization profile READMEs only.

  Voice, sources, and edit rules: see .profile/ (not rendered on the profile).
-->

### Michael Merimee
**I build AI that does real work.**

My story starts at a publisher, where I wore every hat. Then I took the leap into engineering. Today I do platform engineering at Westfield Insurance, and I engineer the harness: the agents, skills, tools, and controls that let AI do real work on systems people depend on.

**Currently:** moving my workstation to Arch Linux to run Hermes Agent plus local and cloud agents, with tight control over cost and token use.

---

### Scepter: many hats
At Scepter Publishers I was Technology and Marketing Manager. The job crossed marketing, operations, and IT. I picked and ran the company's selling technology: website, store integrations, ERP and CRM, email automation, analytics. I set a measure for each tool and reported the results in business terms.

### The leap
Then I took the risk and moved into tech, through Tech Elevator and into platform engineering. I believed I could be a great engineer, because the powers that make one were ones I already used every day: thinking logically, learning a system fast, and making a hard idea simple enough that whoever is listening can use it.

---

### Westfield: platform ownership
The bet turned into ownership of shared infrastructure that other teams depend on.

**Three core apps, off TFVC, in about six months.**
Billing, Policy, and AgencyPlus had 120 developers on TFVC. Two engineers moved all of it to Git in about six months. Agents carried the volume under human approval: they read 200 pipeline definitions, wrote most of the pull requests, and checked 405,198 files against production. Along the way, 200 classic definitions became 9 YAML pipelines on 2 shared templates. In the first month, 54 developers shipped 404 pull requests.

**SonarQube, owned end to end.**
I own SonarQube and led its implementation. I brought scanning to Java, Python, and COBOL codebases, and I run the platform in production. In June 2026 I upgraded SonarQube Enterprise to 2026.3.1.

**Shared templates and the Azure underneath.**
When a shared pipeline template breaks, every team on it feels it. I own and manage a number of those templates. Breaks, changes, and updates for the teams that depend on them come to me, and I recently stepped up to take on more. Underneath, I do the Azure work: permissions and access, and the private build pools I built in Terraform. 418 pipelines from 39 projects moved onto them.

---

### Today: agent harness engineering
A model on its own does not do real work. The harness does: the loop, the tools, the memory, the gates, and the person who signs off.

I have been building toward it since the start of my AI work. From the beginning I built self-learning agent frameworks, more than one, and experimented with the engineering patterns the industry now calls "the harness."

I work in OpenCode, Codex, Claude Code, and Cursor. I try everything, use all of it, and have torn down and rebuilt my setup more than once. The tools change. The engineering holds.

- **Agent systems.** I engineer agents that work together toward one goal, each with its own job, handing work to the next.
- **Skills.** I build Claude skills that package know-how, so an agent does a job the same way every time. At work that includes skills that fix pipelines.
- **Controls.** Identity, gates, audit, blast radius. The same controls I already run on pipelines. A person is accountable for every change.
- **Cost.** Local and cloud models side by side, so I decide where every token goes.

---

### Private work (links coming)
- **The agent fleet.** A multi-agent organization I designed and run: a manager agent that coordinates, project agents for each venture, and reviewer agents that gate purpose, design, architecture, security, and release. Decision gates with a logged trail, a shared skill library across agents, scheduled routines, and a human accountable for every change.
- **Book typesetting studio.** An engine that typesets manuscripts to print quality, tuned by an agent loop that scores the pages.
- **Trinitas.** A trading-card scanner MVP.
- **Client sites run by agents.** The Merimee Ventures client model: each client gets a site plus a dedicated agent that makes changes under review.
- **platform-lab** (planned). The True Rankings job on Kubernetes with k3d and Argo CD, Terraform for AWS EKS, and a one-day EKS demo.

---

### Public proof

**[sleeper-mcp](https://github.com/merimeesoftware/sleeper-mcp)** — remote MCP server on Cloudflare Workers  
One URL for Grok, Cursor, Claude, or any MCP client. Read-only tools, encrypted secrets, KV cache.

**[True Rankings](https://github.com/merimeesoftware/cfb-ranking-algorithm)** — college football rankings  
A list that was not an argument. Weekly drop on a Cloudflare Worker.

**[Senior Schools Network](https://seniorschoolnetwork.com/)** — live site  
Schools in the John Senior and Alan Hicks line. [Repo](https://github.com/merimeesoftware/Senior-Schools-Network).

**[Merimee Solutions](https://github.com/merimeesoftware/merimee-solutions)** — client sites, native rebuild  
Page builders when that was what the owner could run. Native now, same rule.

---

### Client delivery
- [Saint Joseph the Worker Academy](https://www.saintjosephtheworkeracademy.org/) — designed and built from the ground up
- [Holy Rollers](https://www.holyrollers.us/) — website design, messaging
- [Parker Eidle](https://www.parkereidle.com/) — website design

---

### How I work
Evidence over assertion. Live systems outrank documentation. A tool is good when it serves the person using it.

Hand me the part of the job I haven't done yet. Learning it fast is the thing I have proven most.

---

### Stack
OpenCode · Codex · Claude Code · Cursor · Hermes Agent · MCP · Cloudflare Workers · Azure · Azure DevOps · Terraform · SonarQube · Arch Linux

---

### Contact
LinkedIn: [michael-merimee](https://www.linkedin.com/in/michael-merimee/)
