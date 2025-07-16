Tips and guidelines for using Jupyter notebooks.

# Best practices
- Whenever possible, refactor repetitive code into separate .py #python scripts. 
	**DRY**: **D**on't **R**epeat **Y**ourself. 

# Uses
- It's fun to do [[statistics]] in Jupyter notebooks!

# Kernels
- One annoying bit with Jupyter notebooks is updating a source script does not immediately change the version of the script the notebook kernel has imported. This is because on initial import, the kernel is cached into memory, but does not dynamically update even if the source changes. To circumvent this, do
```
	import imp 
	imp.reload(YOUR_PACKAGE_HERE)
```