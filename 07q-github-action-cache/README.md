## GitHub Cache Workflow Submission

1. **Create a new repository** on [GitHub](https://github.com).  

2. Initialise `README.md` file and make it public.

3. **Create a folder manually** in your repo:  `./github/workflows`

4. **Upload your YAML file** (workflow file) into the `workflows` folder.

5. Customize the workflow as per instructions given in your question.

- Change your cache keys in 2 places. 

    ```

    with:
       path: ~/.uv
       key: cache-7845754 

   - name: prime-cache-7845754
   ```

6. Go to the **Actions** tab in your repository.

7. Select **My Workflow** from the list.

8. Use the **manual trigger** button to run the workflow.

9. Once the workflow runs successfully, you will see a **green tick** indicating success.

10. **Submit the repository link** 
