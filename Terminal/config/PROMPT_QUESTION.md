## 📜 Description

Text to add in front of prompt messages.

- **type**: `string`
- required: `false`
- default: `{blue ?}`
- project: [[Terminal Overview]]

### 💡 Example Usage

### 🌍 Environment

> [!summary] Set up as an environment variable for your shell, then run script
```bash
export PROMPT_QUESTION="{blue ?}"
tsx src/main.ts
```
> [!summary] Set up as environment variable for just the single run

```bash
PROMPT_QUESTION="{blue ?}" tsx src/main.ts
```
### 🎛️ CLI Switch

> [!summary] Provide your config as a switch
```bash
tsx src/main.ts --prompt_question="{blue ?}"
# or
tsx src/main.ts --prompt_question {blue ?}
```
### 📁 File
> [!tip] If your file does not have an extension, [[Configuration]] will do auto
#### 📘 ini

> [!example] 
> `.my_app_name`, `~/.config/my_app_name`

```ini
[terminal]
  PROMPT_QUESTION={blue ?}
```
#### 📄 yaml

> [!example]
> `.my_app_name.yaml`

```yaml
terminal:
  PROMPT_QUESTION: "{blue ?}"
```
### 🗃️ json

> [!example]
> `.my_app_name.json`

```json
{
  "terminal": {
    "PROMPT_QUESTION": "{blue ?}"
  }
}
```