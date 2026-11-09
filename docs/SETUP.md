# 🚀 Guía de Instalación y Configuración

Pasos para configurar el proyecto HugzUp en tu máquina.

## Requisitos del Sistema

- **Git**: [Descargar](https://git-scm.com/)
- **Node.js**: v18+ (si usamos JS/React)
- **Python**: 3.9+ (si usamos Python/Django/FastAPI)
- **Editor**: VS Code recomendado

## Primer Setup (Solo la primera vez)

### 1. Clonar el repositorio

```bash
cd ~/Desktop  # o donde quieras el proyecto
git clone https://github.com/avocadohel/HugzUp.git
cd HugzUp
```

### 2. Verificar acceso

```bash
git remote -v
# Debería mostrar:
# origin  https://github.com/avocadohel/HugzUp.git (fetch)
# origin  https://github.com/avocadohel/HugzUp.git (push)
```

### 3. Configurar Git localmente (si es primera vez)

```bash
git config user.name "Tu Nombre"
git config user.email "tu.email@ejemplo.com"

# O globalmente en tu sistema:
git config --global user.name "Tu Nombre"
git config --global user.email "tu.email@ejemplo.com"
```

## Desarrollo Frontend (JavaScript/React)

### Configuración inicial

```bash
cd frontend
npm install
```

### Desarrollo local

```bash
npm start
# Abre http://localhost:3000
```

### Build para producción

```bash
npm run build
```

## Desarrollo Backend (Python/Node.js)

### Si es Node.js

```bash
cd backend
npm install
npm start
```

### Si es Python

```bash
cd backend

# Windows
python -m venv venv
venv\Scripts\activate

# macOS/Linux
python3 -m venv venv
source venv/bin/activate

# Instalar dependencias
pip install -r requirements.txt

# Ejecutar servidor
python app.py  # o similar
```

## Verificar que todo funciona

```bash
# 1. Desde la raíz del proyecto
git status
# Debería mostrar branch actual (main o develop)

# 2. Verifica que las carpetas existan
ls frontend backend docs
```

## Crear tu primera rama

```bash
git checkout -b feature/mi-primera-rama
git push origin feature/mi-primera-rama
```

Ahora puedes abrir un PR en GitHub.

## Solucionar problemas

### "Permission denied (publickey)"
```bash
# Configura SSH con GitHub
# En GitHub: Settings → SSH and GPG keys → Add new SSH key
ssh -T git@github.com
```

### "Your branch is behind 'origin/main'"
```bash
git pull origin main
```

### "Conflictos al mergear"
Ver la sección de "Resolver conflictos" en WORKFLOW.md

## Variables de entorno

Crea un archivo `.env` en cada carpeta (frontend/backend) con:

```bash
# Ejemplo .env
REACT_APP_API_URL=http://localhost:5000
NODE_ENV=development
```

⚠️ **Nunca commits .env con secretos reales** - usa `.env.example` en Git.

## Siguientes pasos

- [ ] Instala las dependencias
- [ ] Prueba que el proyecto inicia sin errores
- [ ] Lee WORKFLOW.md
- [ ] Crea una rama y haz tu primer commit
