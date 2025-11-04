# Roadmap Git Senior 2025-2026
---

## Unidad 1 — Fundamentos y arquitectura de Git

### Capítulo 1.1 — Introducción conceptual a Git

* - [ ] ¿Qué es Git y por qué usarlo? Ventajas competitivas
* - [ ] Sistemas de control de versiones: centralizados vs distribuidos
* - [ ] Arquitectura interna: objetos (blobs, trees, commits, tags)
* - [ ] El DAG (Directed Acyclic Graph) y cómo Git modela el historial
* - [ ] Working tree, staging area (index) y HEAD: roles y flujo
* - [ ] Protocolos de transporte: file, ssh, http/https, git
* - [ ] Ejercicios
* - [ ] Respuestas (paso a paso)

### Capítulo 1.2 — Instalación, configuración y entorno

* - [ ] Instalación multiplataforma y verificación
* - [ ] Configuración esencial: `user.name`, `user.email`, `core.editor`
* - [ ] Configuración avanzada: `includeIf`, aliases, templates
* - [ ] Jerarquía de configuración: system, global, local, worktree
* - [ ] Gestión de credenciales: credential helpers, SSH keys, tokens
* - [ ] Normalización de líneas: `core.autocrlf`, `core.eol`, `.gitattributes`
* - [ ] Herramientas recomendadas: GUI clients, diff/merge tools
* - [ ] Ejercicios
* - [ ] Respuestas (paso a paso)

---

## Unidad 2 — Flujo de trabajo local básico

### Capítulo 2.1 — Inicialización y ciclo fundamental

* - [ ] `git init` y `git clone`: opciones y casos de uso
* - [ ] Ciclo básico: modificar → `add` → `commit` → `status` → `log`
* - [ ] `git add -p` (patch mode) para commits atómicos
* - [ ] `git restore` y `git switch`: alternativas modernas a `checkout`
* - [ ] Mensajes de commit: convenciones y Conventional Commits
* - [ ] `.gitignore` y `.gitattributes`: patrones y casos especiales
* - [ ] `git check-ignore` para debugging de .gitignore
* - [ ] Ejercicios
* - [ ] Respuestas (paso a paso)

### Capítulo 2.2 — Exploración e inspección del historial

* - [ ] `git log` avanzado: formatos, `--graph`, `--grep`, `-S`, `-L`
* - [ ] `git show` y `git diff` en profundidad
* - [ ] `git diff --color-moved` para visualizar refactors
* - [ ] `git blame` y `git blame -C -C` para rastrear cambios
* - [ ] `git shortlog` para resúmenes por autor
* - [ ] `git restore --source=<commit>` para comparaciones
* - [ ] Herramientas visuales: `gitk`, `git gui`, integraciones IDE
* - [ ] Ejercicios
* - [ ] Respuestas (paso a paso)

---

## Unidad 3 — Branching y merging

### Capítulo 3.1 — Gestión de ramas

* - [ ] Concepto de rama y estrategias de nombrado
* - [ ] `git branch`: crear, listar, borrar, renombrar
* - [ ] `git switch` y `git switch -c`: navegación moderna
* - [ ] Ramas remotas vs locales y tracking (`-u`, `--set-upstream-to`)
* - [ ] `git branch --merged` y `--no-merged` para limpieza
* - [ ] Ejercicios
* - [ ] Respuestas (paso a paso)

### Capítulo 3.2 — Merge: estrategias y resolución de conflictos

* - [ ] `git merge`: fast-forward vs merge commit
* - [ ] Estrategias de merge: recursive, ours, theirs, octopus
* - [ ] `git merge --squash` para integración limpia
* - [ ] Resolución de conflictos: manual y con `mergetool`
* - [ ] `git rerere` para reutilizar resoluciones
* - [ ] Abortar y reintentar merges
* - [ ] Ejercicios
* - [ ] Respuestas (paso a paso)

### Capítulo 3.3 — Rebase: reescritura y linearización

* - [ ] `git rebase` básico e interactivo (`-i`)
* - [ ] Comandos interactivos: `pick`, `reword`, `edit`, `squash`, `fixup`, `drop`
* - [ ] `git rebase --onto` para mover ramas
* - [ ] Rebase vs merge: cuándo usar cada uno
* - [ ] Regla de oro: nunca rebase ramas públicas
* - [ ] Conflictos durante rebase: resolución y continuación
* - [ ] `git rebase --abort` y `git rebase --skip`
* - [ ] Ejercicios
* - [ ] Respuestas (paso a paso)

### Capítulo 3.4 — Cherry-pick, revert y reset

* - [ ] `git cherry-pick` y trazabilidad con `-x`
* - [ ] `git revert` para deshacer cambios públicos
* - [ ] `git revert` de merge commits
* - [ ] `git reset`: `--soft`, `--mixed`, `--hard`
* - [ ] Diferencia entre `reset`, `restore` y `revert`
* - [ ] Uso responsable de comandos destructivos
* - [ ] Ejercicios
* - [ ] Respuestas (paso a paso)

---

## Unidad 4 — Trabajo colaborativo con remotos

### Capítulo 4.1 — Gestión de remotos

* - [ ] `git remote add/remove/rename` y gestión de múltiples remotos
* - [ ] `git fetch` y `git fetch --prune`
* - [ ] `git pull` vs `git pull --rebase`
* - [ ] `git push` y refspecs personalizados
* - [ ] Push forzado seguro: `--force-with-lease` vs `--force`
* - [ ] Ramas de tracking y sincronización
* - [ ] Ejercicios
* - [ ] Respuestas (paso a paso)

### Capítulo 4.2 — Workflows colaborativos

* - [ ] Git Flow: estructura y casos de uso
* - [ ] GitHub Flow: simplicidad y continuous delivery
* - [ ] Trunk-Based Development: tendencia 2025-2026
* - [ ] Comparativa de workflows y cuándo aplicar cada uno
* - [ ] Branching policies y estrategias de integración
* - [ ] Ramas de release, hotfix y mantenimiento
* - [ ] Ejercicios
* - [ ] Respuestas (paso a paso)

### Capítulo 4.3 — Pull Requests y Code Review

* - [ ] Anatomía de un PR/MR: estructura y ciclo de vida
* - [ ] Draft PRs y work in progress
* - [ ] Code review efectivo: comentarios, sugerencias, aprobaciones
* - [ ] `CODEOWNERS` y asignación automática de revisores
* - [ ] Templates de PR y convenciones de descripción
* - [ ] Estrategias de merge: squash, rebase-merge, merge commit
* - [ ] CI checks y required status checks
* - [ ] Ejercicios
* - [ ] Respuestas (paso a paso)

---

## Unidad 5 — Recuperación y disaster recovery

### Capítulo 5.1 — Reflog y recuperación de commits

* - [ ] `git reflog`: el "salvavidas" de Git
* - [ ] Recuperar commits perdidos y ramas borradas
* - [ ] Recuperar archivos eliminados de commits antiguos
* - [ ] `git fsck` para encontrar objetos huérfanos
* - [ ] `git cat-file` para inspeccionar objetos
* - [ ] Ejercicios
* - [ ] Respuestas (paso a paso)

### Capítulo 5.2 — Depuración con bisect

* - [ ] `git bisect`: búsqueda binaria de regresiones
* - [ ] `git bisect start`, `good`, `bad`, `reset`
* - [ ] `git bisect run` para automatización
* - [ ] Casos de uso prácticos y limitaciones
* - [ ] Ejercicios
* - [ ] Respuestas (paso a paso)

### Capítulo 5.3 — Limpieza y reescritura de historial

* - [ ] `git filter-repo` como herramienta moderna (reemplazo de filter-branch)
* - [ ] Eliminar archivos grandes del historial
* - [ ] Remover secretos y datos sensibles
* - [ ] BFG Repo-Cleaner: mención histórica
* - [ ] Consideraciones al reescribir historial público
* - [ ] Coordinación de equipo tras reescritura
* - [ ] Ejercicios
* - [ ] Respuestas (paso a paso)

### Capítulo 5.4 — Mantenimiento del repositorio

* - [ ] `git gc`: garbage collection y optimización
* - [ ] `git prune` y limpieza de objetos
* - [ ] `git repack` para compresión
* - [ ] Verificación de integridad con `git fsck --full`
* - [ ] Ejercicios
* - [ ] Respuestas (paso a paso)

---

## Unidad 6 — Arquitectura de repositorios

### Capítulo 6.1 — Repositorios grandes y optimización

* - [ ] Shallow clone y partial clone
* - [ ] `git sparse-checkout` y cone mode
* - [ ] Filtrado de directorios y optimización de clones
* - [ ] Técnicas de rendimiento para monorepos
* - [ ] Ejercicios
* - [ ] Respuestas (paso a paso)

### Capítulo 6.2 — Git LFS para archivos binarios

* - [ ] Cuándo usar Git LFS
* - [ ] Instalación y configuración: `git lfs install`, `track`
* - [ ] Migración de archivos existentes a LFS
* - [ ] Limitaciones y consideraciones de costo
* - [ ] Alternativas: DVC, artifact repositories
* - [ ] Ejercicios
* - [ ] Respuestas (paso a paso)

### Capítulo 6.3 — Submodules

* - [ ] `git submodule add`, `init`, `update`, `sync`
* - [ ] Flujo de trabajo con submodules
* - [ ] Actualización de submodules y versionado
* - [ ] Problemas comunes y soluciones
* - [ ] Submodules en CI/CD
* - [ ] Ejercicios
* - [ ] Respuestas (paso a paso)

### Capítulo 6.4 — Subtree y alternativas

* - [ ] `git subtree`: add, merge, split, pull
* - [ ] Ventajas de subtree vs submodule
* - [ ] Casos de uso: librerías compartidas, vendor directories
* - [ ] Monorepo vs multi-repo: análisis estratégico
* - [ ] Ejercicios
* - [ ] Respuestas (paso a paso)

---

## Unidad 7 — Seguridad y compliance

### Capítulo 7.1 — Firmas de commits y tags

* - [ ] Firmas GPG: configuración y uso
* - [ ] Firmas SSH: alternativa moderna y más simple
* - [ ] Verificación de firmas: `git verify-commit`, `git verify-tag`
* - [ ] Políticas de firma obligatoria
* - [ ] "Vigilant Mode" en GitHub
* - [ ] Ejercicios
* - [ ] Respuestas (paso a paso)

### Capítulo 7.2 — Prevención de secretos

* - [ ] Evitar commits de secretos: mejores prácticas
* - [ ] Herramientas de escaneo: `git-secrets`, `detect-secrets`, `trufflehog`
* - [ ] Pre-commit hooks para prevención
* - [ ] Secret scanning nativo en GitHub/GitLab
* - [ ] Mitigación tras exposición accidental
* - [ ] Ejercicios
* - [ ] Respuestas (paso a paso)

### Capítulo 7.3 — Dependabot y gestión de dependencias

* - [ ] Dependabot: configuración y alertas
* - [ ] Security advisories y parches automáticos
* - [ ] Code scanning y análisis estático
* - [ ] GitHub Advanced Security: conceptos
* - [ ] Ejercicios
* - [ ] Respuestas (paso a paso)

---

## Unidad 8 — Automatización con hooks

### Capítulo 8.1 — Git hooks locales

* - [ ] Hooks del lado del cliente: `pre-commit`, `pre-push`, `commit-msg`, `post-checkout`
* - [ ] Ejemplos prácticos: linting, testing, formateo
* - [ ] Distribución de hooks en el equipo
* - [ ] Ejercicios
* - [ ] Respuestas (paso a paso)

### Capítulo 8.2 — Frameworks de gestión de hooks

* - [ ] `husky` (JavaScript/Node.js)
* - [ ] `pre-commit` (Python)
* - [ ] `lefthook` (Go, multiplataforma)
* - [ ] Comparativa y casos de uso
* - [ ] Ejercicios
* - [ ] Respuestas (paso a paso)

### Capítulo 8.3 — Hooks del lado del servidor

* - [ ] `pre-receive`, `update`, `post-receive`
* - [ ] Aplicación de políticas en el servidor
* - [ ] Integración con sistemas de notificación
* - [ ] Ejercicios
* - [ ] Respuestas (paso a paso)

---

## Unidad 9 — CI/CD con GitHub Actions

### Capítulo 9.1 — Fundamentos de GitHub Actions

* - [ ] Anatomía de un workflow: triggers, jobs, steps
* - [ ] Eventos: push, pull_request, schedule, workflow_dispatch
* - [ ] Runners: GitHub-hosted vs self-hosted
* - [ ] Contexts y expresiones
* - [ ] Ejercicios
* - [ ] Respuestas (paso a paso)

### Capítulo 9.2 — Workflows avanzados

* - [ ] Matrix builds para testing multiplataforma
* - [ ] Secrets y variables de entorno
* - [ ] Artifacts y caching para optimización
* - [ ] Conditional execution y estrategias
* - [ ] Reusable workflows
* - [ ] Ejercicios
* - [ ] Respuestas (paso a paso)

### Capítulo 9.3 — GitHub Marketplace y Actions personalizadas

* - [ ] Uso de actions del marketplace
* - [ ] Creación de custom actions: JavaScript, Docker, Composite
* - [ ] Publicación y versionado de actions
* - [ ] Ejercicios
* - [ ] Respuestas (paso a paso)

### Capítulo 9.4 — GitLab CI/CD (comparativa)

* - [ ] Conceptos básicos de `.gitlab-ci.yml`
* - [ ] Pipelines, stages y jobs
* - [ ] Comparación con GitHub Actions
* - [ ] Ejercicios
* - [ ] Respuestas (paso a paso)

---

## Unidad 10 — Gobernanza y políticas organizacionales

### Capítulo 10.1 — Protección de ramas

* - [ ] Branch protection rules en GitHub/GitLab
* - [ ] Required reviews y approvals
* - [ ] Required status checks
* - [ ] Restricciones de push y force-push
* - [ ] Dismiss stale reviews y code owners review
* - [ ] Ejercicios
* - [ ] Respuestas (paso a paso)

### Capítulo 10.2 — CODEOWNERS y equipos

* - [ ] Archivo `CODEOWNERS`: sintaxis y patrones
* - [ ] Equipos y asignación automática
* - [ ] Estrategias para repos grandes
* - [ ] Ejercicios
* - [ ] Respuestas (paso a paso)

### Capítulo 10.3 — Permisos y roles

* - [ ] Roles en GitHub: Read, Triage, Write, Maintain, Admin
* - [ ] Organizations y Teams
* - [ ] SAML SSO y SCIM provisioning
* - [ ] Audit logs y rastreabilidad
* - [ ] Ejercicios
* - [ ] Respuestas (paso a paso)

### Capítulo 10.4 — Políticas de merge y estrategias

* - [ ] Require linear history
* - [ ] Squash merging vs rebase merging vs merge commits
* - [ ] Auto-merge y merge queue
* - [ ] Branch deletion automática
* - [ ] Ejercicios
* - [ ] Respuestas (paso a paso)

---

## Unidad 11 — Releases y distribución

### Capítulo 11.1 — GitHub Releases

* - [ ] Creación de releases y tags
* - [ ] Release assets y binarios
* - [ ] Changelogs automáticos y release notes
* - [ ] Versionado semántico y estrategias
* - [ ] Ejercicios
* - [ ] Respuestas (paso a paso)

### Capítulo 11.2 — GitHub Packages

* - [ ] GitHub Package Registry: npm, Maven, Docker, NuGet
* - [ ] Publicación automática desde CI
* - [ ] Autenticación y permisos
* - [ ] Integración con dependencias privadas
* - [ ] Ejercicios
* - [ ] Respuestas (paso a paso)

### Capítulo 11.3 — Versionado y changelog

* - [ ] Conventional Commits y semantic versioning
* - [ ] Generación automática de changelogs
* - [ ] Herramientas: `semantic-release`, `standard-version`, `release-please`
* - [ ] Vinculación con issues y PRs
* - [ ] Ejercicios
* - [ ] Respuestas (paso a paso)

---

## Unidad 12 — Gestión de proyectos y trazabilidad

### Capítulo 12.1 — GitHub Projects (v2)

* - [ ] Tableros y vistas: table, board, roadmap
* - [ ] Campos personalizados e iteraciones
* - [ ] Automatización de proyectos
* - [ ] Integración con issues y PRs
* - [ ] Ejercicios
* - [ ] Respuestas (paso a paso)

### Capítulo 12.2 — Issues y milestones

* - [ ] Templates de issues
* - [ ] Labels y asignación
* - [ ] Milestones para planificación
* - [ ] Linking entre issues, PRs y commits
* - [ ] Ejercicios
* - [ ] Respuestas (paso a paso)

### Capítulo 12.3 — Integración con Jira y otras herramientas

* - [ ] Vinculación de commits con tickets externos
* - [ ] Smart commits y automatización
* - [ ] Webhooks para sincronización
* - [ ] Ejercicios
* - [ ] Respuestas (paso a paso)

---

## Unidad 13 — Herramientas del ecosistema

### Capítulo 13.1 — GitHub CLI

* - [ ] Instalación y autenticación de `gh`
* - [ ] Gestión de PRs, issues y releases desde terminal
* - [ ] Automatización con scripts
* - [ ] Ejercicios
* - [ ] Respuestas (paso a paso)

### Capítulo 13.2 — Integraciones IDE

* - [ ] GitLens para VS Code
* - [ ] Git en JetBrains IDEs
* - [ ] GitHub Copilot en el flujo de desarrollo
* - [ ] Ejercicios
* - [ ] Respuestas (paso a paso)

### Capítulo 13.3 — Herramientas de terminal

* - [ ] `lazygit` para flujo interactivo
* - [ ] `tig` como navegador de historial
* - [ ] `fzf` para búsquedas rápidas
* - [ ] `delta` para diffs mejorados
* - [ ] Ejercicios
* - [ ] Respuestas (paso a paso)

---

## Unidad 14 — Migraciones y consolidaciones

### Capítulo 14.1 — Migración entre plataformas

* - [ ] GitHub ↔ GitLab ↔ Bitbucket: estrategias
* - [ ] Preservación de issues, PRs y metadata
* - [ ] GitHub Enterprise Importer (`gh gei`)
* - [ ] Validación post-migración
* - [ ] Ejercicios
* - [ ] Respuestas (paso a paso)

### Capítulo 14.2 — Fusión de repositorios (multi-repo → monorepo)

* - [ ] Técnicas sin perder historial: `filter-repo`, `subtree`
* - [ ] Reorganización de estructura de directorios
* - [ ] Actualización de CI/CD y configuraciones
* - [ ] Consideraciones de permisos y acceso
* - [ ] Ejercicios
* - [ ] Respuestas (paso a paso)

### Capítulo 14.3 — División de repositorios (monorepo → multi-repo)

* - [ ] Extracción de subdirectorios con historial
* - [ ] Uso de `git filter-repo` para split
* - [ ] Mantenimiento de dependencias entre repos
* - [ ] Ejercicios
* - [ ] Respuestas (paso a paso)

---

## Unidad 15 — Internals: bajo el capó de Git

### Capítulo 15.1 — Estructura del directorio .git

* - [ ] Anatomía de `.git`: `HEAD`, `config`, `refs`, `objects`, `index`
* - [ ] Cómo Git almacena objetos
* - [ ] Pack files y optimización de almacenamiento
* - [ ] Ejercicios
* - [ ] Respuestas (paso a paso)

### Capítulo 15.2 — Comandos plumbing

* - [ ] `git hash-object`, `git cat-file`
* - [ ] `git update-index`, `git write-tree`, `git commit-tree`
* - [ ] Construcción manual de commits
* - [ ] Automatización con plumbing commands
* - [ ] Ejercicios
* - [ ] Respuestas (paso a paso)

---

## Unidad 16 — Buenas prácticas y convenciones

### Capítulo 16.1 — Convenciones de código y commits

* - [ ] Conventional Commits en profundidad
* - [ ] Templates de commit messages
* - [ ] Estrategias de nombrado de ramas
* - [ ] Tamaño y atomicidad de commits
* - [ ] Ejercicios
* - [ ] Respuestas (paso a paso)

### Capítulo 16.2 — Documentación del repositorio

* - [ ] README.md efectivo
* - [ ] CONTRIBUTING.md y guías de contribución
* - [ ] CODE_OF_CONDUCT.md
* - [ ] SECURITY.md y políticas de vulnerabilidades
* - [ ] Templates de issues y PRs
* - [ ] Ejercicios
* - [ ] Respuestas (paso a paso)

### Capítulo 16.3 — Onboarding de desarrolladores

* - [ ] Checklists de incorporación
* - [ ] Documentación de flujos y procesos
* - [ ] Setup automático y scripts de inicialización
* - [ ] Ejercicios
* - [ ] Respuestas (paso a paso)

---

## Unidad 17 — Escenarios avanzados y resolución de problemas

### Capítulo 17.1 — Conflictos complejos y divergencias

* - [ ] Resolución de conflictos en rebases de larga duración
* - [ ] Divergencias entre ramas remotas y locales
* - [ ] Estrategias para branches "zombie" y PRs abandonados
* - [ ] Uso avanzado de `git rerere`
* - [ ] Ejercicios
* - [ ] Respuestas (paso a paso)

### Capítulo 17.2 — Recuperación tras incidentes

* - [ ] Push accidental de secretos: remediación completa
* - [ ] Force push a rama protegida: recuperación
* - [ ] Merge incorrecto en producción
* - [ ] Auditoría forense con logs y reflog
* - [ ] Ejercicios
* - [ ] Respuestas (paso a paso)

### Capítulo 17.3 — Debugging avanzado

* - [ ] Combinación de `bisect`, `blame` y `log` para investigación
* - [ ] Rastreo de cambios a través de refactors
* - [ ] Identificación de regresiones de rendimiento
* - [ ] Ejercicios
* - [ ] Respuestas (paso a paso)

---

## Unidad 18 — Certificación y evaluación senior

### Capítulo 18.1 — Competencias técnicas senior

* - [ ] Dominio de branching, merging y rebase
* - [ ] Recuperación y disaster recovery
* - [ ] CI/CD y automatización
* - [ ] Seguridad y compliance
* - [ ] Liderazgo técnico y mentoría
* - [ ] Ejercicios
* - [ ] Respuestas (paso a paso)

### Capítulo 18.2 — Simulacros de entrevista

* - [ ] Preguntas técnicas frecuentes
* - [ ] Ejercicios prácticos tipo whiteboard
* - [ ] Escenarios de crisis y resolución
* - [ ] Ejemplos: "Un junior hizo force push a main, ¿qué haces?"
* - [ ] Ejercicios
* - [ ] Respuestas (paso a paso)

### Capítulo 18.3 — Proyectos finales

* - [ ] Migración de repositorio completo
* - [ ] Implementación de CI/CD desde cero
* - [ ] Setup de gobernanza organizacional
* - [ ] Limpieza y optimización de monorepo
* - [ ] Ejercicios
* - [ ] Respuestas (paso a paso)

---

## Unidad 19 — Tendencias y futuro

### Capítulo 19.1 — IA en desarrollo de software

* - [ ] GitHub Copilot en PRs y code review
* - [ ] Generación automática de tests y documentación
* - [ ] IA en detección de bugs y vulnerabilidades
* - [ ] Consideraciones de verificación humana
* - [ ] Ejercicios
* - [ ] Respuestas (paso a paso)

### Capítulo 19.2 — Evolución de workflows

* - [ ] Trunk-Based Development como estándar
* - [ ] Ship/Show/Ask y otras metodologías emergentes
* - [ ] GitOps y infraestructura como código
* - [ ] Ejercicios
* - [ ] Respuestas (paso a paso)

### Capítulo 19.3 — Actualización continua

* - [ ] Recursos de aprendizaje: blogs, conferencias, comunidades
* - [ ] Certificaciones y credenciales
* - [ ] Plan personal de desarrollo profesional
* - [ ] Ejercicios
* - [ ] Respuestas (paso a paso)

---

## Apéndices

### Apéndice A — Glosario técnico
* - [ ] Términos y definiciones completas

### Apéndice B — Cheatsheet de comandos
* - [ ] Comandos esenciales y avanzados con ejemplos

### Apéndice C — Templates y configuraciones
* - [ ] `.gitconfig` ejemplo
* - [ ] Hooks de ejemplo
* - [ ] Templates de PR/issue
* - [ ] Workflows de GitHub Actions

### Apéndice D — Recursos de práctica
* - [ ] Repositorios de ejemplo por nivel
* - [ ] Ejercicios graduados por dificultad
* - [ ] Proyectos de código abierto para contribuir

### Apéndice E — Guía de entrevistas
* - [ ] Checklist de preparación para roles senior
* - [ ] Preguntas frecuentes y respuestas modelo
* - [ ] Construcción de portafolio técnico