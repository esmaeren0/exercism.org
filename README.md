# exercism.org
This repository contains bash practices from exercisim.org

## PARAMETER EXPANSION

this structure using for define a default value when parameter is empty or not defined.
 * basic structure
 ```bash
# if $1 empty , using "you" 
name=${1:-you}
echo "Hello, $name!"
```
#  Use Cases

| Area | Description |
|------|------------|
| Default value assignment | Provide a safe value when a script receives optional arguments |
| Empty or undefined variable check | Use a default value if an environment variable is missing |
| CLI tools | Handle optional parameters in command-line scripts |
| System administration / DevOps | Run scripts with default values if config is missing |
| Data pipelines / ETL | Use default paths or parameters when none are provided |

---

# Similar Constructs

| Construct | Meaning |
|-----------|--------|
| `${parameter:-default}` | Use default if the variable is empty or undefined; otherwise use the variable |
| `${parameter:=default}` | If the variable is empty or undefined, assign it the default value |
| `${parameter:+alt}` | If the variable is set, use `alt`; otherwise use nothing |
| `${parameter:?error}` | If the variable is empty or undefined, display an error message |
