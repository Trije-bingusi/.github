# RSO project — UL FRI

Organization for a course project in **Cloud Services (RSO)** at the University of Ljubljana, Faculty of Computer and Information Science (UL FRI).  
We are **three students** (Janez Tomšič, Matija Bažec, Matic Zadobovšek) building a microservices-based platform for easier studying, one repo per service.

> Currently available: **svc-courses** — minimal Courses service (Node/Express + PostgreSQL) with Docker/Kubernetes manifests, Azure ACR/AKS scripts, Prisma migrations, and some tests. See that repo’s README for setup & deployment.

## Platform vision
- **Subjects & lectures:** each subject page aggregates its lectures.
- **Lecture view:** a dedicated page per lecture with the video centered and a right-hand sidebar offering:
  - **Chat:** persistent history with **timestamps** for each message.
  - **Speech-to-Text:** live/archived transcript of the lecture.
  - **Personal notes:** take and save notes per lecture; notes are also accessible from the subject’s main page for study.
- **Smart search:** search across transcripts and jump directly to the **lecture + timestamp** where the topic appears.
- **Forum:** a subject-level forum on each subject subpage for Q&A among students.
- **Administration:** professors/admins can **upload and remove** lecture videos and manage metadata.

## Contributing
This is a **course project**. We do **not** accept external contributions; PRs from non-members will be closed.

---
© UL FRI — RSO course project
