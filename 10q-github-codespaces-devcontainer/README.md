## Dev Containers Setup

1. **Create a new repository** on [GitHub](https://github.com).  

2. **Create a folder manually** in your repository: `./devcontainer` 

3. **Add the devcontainer configuration file**:  
- Copy the provided `devcontainer.json` file into the `./devcontainer` folder.  
- Update the `"name"` field in the JSON to match your assignment question.  
- Commit and push the changes to your repository.

4. **Open a Codespace**:  
- Go to the **Code** tab in your repository.  
- Click **Codespaces** → **New codespace**.  

5. **Verify environment variables** in the Codespace terminal:  

```bash

echo $GITHUB_REPOSITORY $GITHUB_TOKEN
```

