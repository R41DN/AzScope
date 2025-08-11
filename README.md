# AzScope

AzScope es una herramienta de **enumeración y detección de subdominios** con un enfoque especial en identificar activos alojados en **Microsoft Azure**.

Diseñada para **pentesters**, **bug bounty hunters** y analistas de seguridad, permite descubrir subdominios válidos, resolver sus IPs y verificar si están dentro de los rangos IPv4 públicos de Azure.  
Su interfaz en terminal es **colorida, moderna y fácil de leer**, pensada para hacer más agradable y clara la revisión de resultados.

---

## 🚀 Características

- Enumeración de subdominios usando listas personalizadas.
- Resolución y filtrado de IPs contra prefijos IPv4 oficiales de Azure.
- Exportación opcional de resultados a formato `.tsv` para análisis posterior.
- Compatible con entornos Linux.

---

## 📦 Requisitos

Antes de ejecutar AzScope, asegúrate de tener instaladas las siguientes herramientas y librerías:

```bash
sudo apt install grepcidr && go install github.com/projectdiscovery/dnsx/cmd/dnsx@latest && pip install rich
```

**Notas:**
- `dnsx` se instala con `go install` (requiere tener Go instalado).
- Si no tienes Go, instálalo siguiendo la [documentación oficial](https://go.dev/doc/install).

---

## 🔧 Instalación

Clona el repositorio y da permisos de ejecución al script:

```bash
git clone https://https://github.com/R41DN/AzScope.git
cd AzScope
chmod +x AzScopee.py
```

---

## 📌 Uso

Ejecución básica:

```bash
./AzScope.py <dominio> <wordlist> [output.tsv]
```

- `<dominio>` → Dominio objetivo (ej: `example.com`)
- `<wordlist>` → Lista de subdominios (ej: `/usr/share/seclists/Discovery/DNS/subdomains-top1million-5000.txt`)
- `[output.tsv]` → (Opcional) Archivo donde se guardarán los resultados filtrados.

Ejemplo:

```bash
./AzScope.py microsoft.com /usr/share/seclists/Discovery/DNS/subdomains-top1million-5000.txt resultados.tsv
```

---

