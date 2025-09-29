## Docker Hub Image Deployment

This guide explains how to create a Docker image, tag it as `23f1001691`, and push it to Docker Hub.

---

1. Prerequisites

- Docker installed on your machine: [Docker Desktop](https://www.docker.com/products/docker-desktop)
- A Docker Hub account: [https://hub.docker.com/](https://hub.docker.com/)
- Dockerfile present in your project root directory

---

2. Create a Personal Access Token (PFA) on Docker Hub

-  Go to [Docker App > Account Settings > Personal Access Tokens](https://app.docker.com/accounts/<username>/settings/personal-access-tokens)
- Click **Generate New Token**
- Give it a name and copy the token
- **You will use this token instead of your Docker Hub password**

---

3. Log in to Docker Hub

Open your root folder and go to terminal and run:

```bash

docker login
```

---

4. Build the Image

```bash

docker build -t <your-username>/<repository-name>:23f1001691 .
```

---

5. Verify the Image

```bash

docker images
```

---

6. Push the Image to Docker Hub

```bash

docker push <your-username>/<repository-name>:23f1001691
```

---

7. Verify on Docker Hub

```bash

Go to: `https://hub.docker.com/repository/docker/<your-username>/<repository-name>/general`
```

---
