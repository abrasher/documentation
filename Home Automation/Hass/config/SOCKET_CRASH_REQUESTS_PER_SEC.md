> SOCKET_CRASH_REQUESTS_PER_SEC

## 📜 Description

Socket service will commit sudoku if more than this many outgoing messages are sent to Home Assistant in a second. Usually indicates runaway code.

- **type**: `number`
- required: `false`
- default: `500`
- project: [[Hass Overview]]

### 💡 Example Usage

### 🌍 Environment

> [!summary] Set up as an environment variable for your shell, then run the script
```bash
export SOCKET_CRASH_REQUESTS_PER_SEC=500
tsx src/main.ts
```
> [!summary] Set up as an environment variable for just the single run

```bash
SOCKET_CRASH_REQUESTS_PER_SEC=500 tsx src/main.ts
```
### 🎛️ CLI Switch

> [!summary] Provide your config as a switch
```bash
tsx src/main.ts --socket_crash_requests_per_sec=500
# or
tsx src/main.ts --socket_crash_requests_per_sec 500
```
### 📁 File
> [!tip] If your file does not have an extension, [[Configuration]] will do auto
#### 📘 ini

> [!example] 
> `.my_app_name`, `~/.config/my_app_name`

```ini
[hass]
  SOCKET_CRASH_REQUESTS_PER_SEC=500
```
#### 📄 yaml

> [!example]
> `.my_app_name.yaml`

```yaml
hass:
  SOCKET_CRASH_REQUESTS_PER_SEC: 500
```
### 🗃️ json

> [!example]
> `.my_app_name.json`

```json
{
  "hass": {
    "SOCKET_CRASH_REQUESTS_PER_SEC": 500
  }
}
```