## Local Ollama Endpoint

1. Open WSL/Ubuntu

2. Install Ollama

```bash

curl -fsSL https://ollama.com/install.sh | sh
```

3. Run Ollama server with CORS enabled

```bash

export OLLAMA_ORIGINS="*"
ollama serve
```

4. Install Ngrok

```bash

curl -sSL https://ngrok-agent.s3.amazonaws.com/ngrok.asc \
  | sudo tee /etc/apt/trusted.gpg.d/ngrok.asc >/dev/null \
  && echo "deb https://ngrok-agent.s3.amazonaws.com bookworm main" \
  | sudo tee /etc/apt/sources.list.d/ngrok.list \
  && sudo apt update \
  && sudo apt install ngrok
```

5. Run ngrok with custom headers for CORS and bypassing browser warning

```bash

ngrok http 11434 \
  --response-header-add "X-Email: 23f1001691@ds.study.iitm.ac.in" \
  --response-header-add "Access-Control-Expose-Headers: *" \
  --response-header-add "Access-Control-Allow-Headers: Ngrok-skip-browser-warning" \
  --host-header=localhost
```

6. In the above ngrok run command, make sure you add your smail instead mine. 

---

**Notes**

* If Ollama is already running on `11434`, stop it first:

```bash

pkill -f ollama
```

* Test CORS locally before ngrok:

```bash

curl -i -H "Origin: http://example.com" http://localhost:11434
```

* For ngrok, you can test:

```bash

curl -i -H "Origin: https://<your-ngrok-id>.ngrok-free.app" https://<your-ngrok-id>.ngrok-free.app
```

---


