
# Alexandria Archives

---

## Welcome to Alexandria Archives
This is a consolidated guide for various technical setups mostly for me, to make sure it's stored somewher, as technical work like this is not always intuitive and sometimes you will face an issue which is not easily solved. These are currently including:

- Setting up markdown projects like this one
- Setting up Switch emulation using Yuzu, including:
    - Setting up Zelda: Tears of the Kingdom (TotK) and Breath of the Wild (BotW)
    - Optimizing both TotK and BotW with settings or tools
    - Installing and configuring mods

___

## Setting Up MkDocs with Material

This section will guide you through setting up MkDocs with the Material theme. MkDocs is a static site generator that's geared towards project documentation.

### Prerequisites

Make sure you have Python installed. You can download it from the [official Python website](https://www.python.org/).

### Step-by-Step Setup

1. **Create a Virtual Environment**

   It's a good practice to use a virtual environment to manage your project's dependencies. Here are the commands to create and activate a virtual environment:

   ```sh
   python -m venv venv
   ```

2. **Activate the Virtual Environment**

   - On Windows:

     ```sh
     .\venv\Scripts\activate
     ```

   - On macOS and Linux:

     ```sh
     source venv/bin/activate
     ```

3. **Install MkDocs and MkDocs-Material**

   With your virtual environment activated, install MkDocs and the Material theme:

   ```sh
   pip install mkdocs mkdocs-material
   ```

4. **Create a New MkDocs Project**

   Initialize a new MkDocs project using the following command:

   ```sh
   mkdocs new my-project
   cd my-project
   ```

5. **Edit `mkdocs.yml` to Use the Material Theme**

   Open the `mkdocs.yml` file in your project directory and modify it to use the Material theme:

   ```yaml
   site_name: My Project
   theme:
     name: material
   ```

6. **Serve the Documentation Locally**

   To preview your documentation locally, use the `serve` command:

   ```sh
   mkdocs serve
   ```

   Open your browser and navigate to `http://127.0.0.1:8000/` to see your MkDocs site in action.

***

## Conclusion

With these steps, you have successfully set up MkDocs with the Material theme. You can now start writing your project documentation and use the MkDocs server to preview your changes in real-time.