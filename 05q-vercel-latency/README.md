## Vercel Deployment

1. Go to **[vercel.com](https://vercel.com/)** and create a **free account**.

2. **Download the JSON file** given in the question and **replace `q-vercel-latency.json`** in the folder.

3. On your local machine, open a terminal (Ubuntu/WSL).

   - Navigate to your **project’s root folder**.

4. Install **Node.js** (if not already installed):

   ```bash

   sudo apt update
   sudo apt install -y nodejs npm
   ```

5. Install the **Vercel CLI** globally:

   ```bash

   npm install -g vercel
   ```

6. Verify installation:

   ```bash

   vercel --version
   ```

7. Log in to Vercel:

   ```bash

   vercel login
   ```

8. Deploy your project:

   ```bash

   vercel
   ```
