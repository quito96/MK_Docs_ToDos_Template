# Easy way to get documentation for Python projects

---

1. Install MkDocs and mkdocstrings into your Project: If not done yet, install MkDocs and the mkdocstrings plugin using pip:
```bash
pip install mkdocs
pip install mkdocstrings
```
## Commands

* `mkdocs new [dir-name]` - Create a new project.
* `mkdocs serve` - Start the live-reloading docs server.
* `mkdocs build` - Build the documentation site.
* `mkdocs -h` - Print help message and exit.
2. Create a new MkDocs project: Make a new directory for [your project]() and initialize it with MkDocs in Projekt root:
```bash
mkdir my_project
cd my_project
```
The . behind new is for the root Project Directory.
```bash
mkdocs new .
```
3. Configure the mkdocstrings plugin: 
Edit the [mkdocs.yml]() file in your project directory to include the mkdocstrings plugin:
```yaml
plugins:
  - search
  - mkdocstrings
```
4. Add code documentation: In your Markdown files, you can use the ::: identifier syntax to automatically generate documentation for specific code objects. For example, if you have a class MyClass in a module mymodule, you could write the following in your Markdown file:
```markdown
::: mymodule.MyClass
```

5. Start the server: Start MkDocs' local development server to view your documentation:
```bash
mkdocs serve 
```
6. Open in browser: Open http://localhost:8000 in your web browser to see the generated documentation. 


7. Optionally, make customizations: You can customize the appearance and behavior of mkdocstrings by setting various options in the mkdocs.yml file. Complete documentation can be found in the official mkdocstrings documentation.

Remember, mkdocstrings utilizes the docstrings from your Python code, so ensure they are well-written and informative. This aligns well with your desire for clear and understandable code documentation.