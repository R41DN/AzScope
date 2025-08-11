# AzScope

AzScope es una herramienta de **enumeración y detección de subdominios** con un enfoque especial en identificar activos alojados en **Microsoft Azure**.

Diseñada para **pentesters**, **bug bounty hunters** y analistas de seguridad, permite descubrir subdominios válidos, resolver sus IPs y verificar si están dentro de los rangos IPv4 públicos de Azure.  
Su interfaz en terminal es **colorida, moderna y fácil de leer**, pensada para hacer más agradable y clara la revisión de resultados.

---

## 🚀 Características

- Enumeración de subdominios usando listas personalizadas.
- Resolución y filtrado de IPs contra prefijos IPv4 oficiales de Azure.
- Interfaz visual llamativa y organizada con colores brillantes.
- Exportación opcional de resultados a formato `.tsv` para análisis posterior.
- Compatible con entornos Linux.

## Requisitos
<pre> ```bash sudo apt install grepcidr && go install github.com/projectdiscovery/dnsx/cmd/dnsx@latest && pip install rich ``` </pre>

