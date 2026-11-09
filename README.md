# 🤗 HugzUp

**Conectando gente a través de abrazos**

Una plataforma para encontrar y conectar con personas que buscan compartir momentos significativos mediante abrazos en tu comunidad.

---

## 📋 Tabla de Contenidos

- [Descripción del Proyecto](#descripción-del-proyecto)
- [Tecnología](#tecnología)
- [Estructura del Proyecto](#estructura-del-proyecto)
- [Requisitos Previos](#requisitos-previos)
- [Instalación](#instalación)
- [Desarrollo](#desarrollo)
- [Contribuciones](#contribuciones)
- [Contacto](#contacto)

---

## 🎯 Descripción del Proyecto

HugzUp es una app social que conecta personas en tu zona que desean compartir abrazos y crear conexiones humanas significativas. 

### Características Principales
- [ ] Localización geográfica de usuarios cercanos
- [ ] Perfiles de usuario personalizables
- [ ] Sistema de matching/conexiones
- [ ] Chat para coordinación
- [ ] Sistema de confianza/reputación

---

## 🛠 Tecnología

**Frontend:** (Por definir - React/Vue/Flutter)  
**Backend:** (Por definir - Node.js/Python/Go)  
**Base de Datos:** (Por definir - PostgreSQL/MongoDB)  
**Hosting:** (Por definir)  

---

## 📁 Estructura del Proyecto

```
HugzUp/
├── frontend/              # Aplicación cliente (web/mobile)
│   ├── src/
│   ├── public/
│   └── package.json
├── backend/               # Servidor API
│   ├── src/
│   ├── config/
│   └── requirements.txt
├── docs/                  # Documentación
│   ├── SETUP.md          # Guía de configuración inicial
│   ├── WORKFLOW.md       # Flujo de trabajo colaborativo
│   ├── API.md            # Documentación de API
│   └── DECISIONS.md      # Decisiones técnicas
├── .github/
│   └── workflows/         # CI/CD (GitHub Actions)
├── .gitignore
└── README.md
```

---

## 📦 Requisitos Previos

- Git configurado
- Node.js v18+ (si usamos Node para backend)
- Python 3.9+ (si usamos Python para backend)
- Cuenta en GitHub

---

## 🚀 Instalación

### Clonar el repositorio
```bash
git clone https://github.com/avocadohel/HugzUp.git
cd HugzUp
```

### Configurar frontend
```bash
cd frontend
npm install
# npm start
```

### Configurar backend
```bash
cd ../backend
# python -m venv venv
# source venv/bin/activate
# pip install -r requirements.txt
```

---

## 👨‍💻 Desarrollo

### Flujo de trabajo colaborativo
1. **Crear rama**: `git checkout -b feature/descripcion-corta`
2. **Hacer cambios**: Commitea regularmente con mensajes claros
3. **Push**: `git push origin feature/descripcion-corta`
4. **Pull Request**: Abre PR en GitHub con descripción
5. **Review**: El otro colaborador revisa y aprueba
6. **Merge**: Se integra a `main`

### Convenciones de commits
```
feat: nueva funcionalidad
fix: corrección de bug
docs: cambios en documentación
style: cambios de formato/estilo
refactor: reorganización de código
test: cambios en tests
chore: cambios en build/config
```

Ejemplo: `git commit -m "feat: agregar autenticación con Google"`

### Ramas principales
- **main**: Versión estable, lista para producción
- **develop**: Rama de desarrollo (opcional)
- **feature/***: Nuevas funcionalidades
- **bugfix/***: Correcciones de errores

---

## 🤝 Contribuciones

### Para colaboradores (tú y avocadohel)
1. Revisa los [issues abiertos](https://github.com/avocadohel/HugzUp/issues)
2. Discutan en issues o pull requests antes de cambios importantes
3. Actualiza la documentación si cambias comportamiento
4. Escribe tests para nuevas funcionalidades

### Código limpio
- Comenta el código complejo
- Sigue el estilo del proyecto
- Prueba localmente antes de push

---

## 📞 Contacto

- **avocadohel**: [GitHub Profile](https://github.com/avocadohel)
- **Guillem Pons Barcons**: [GitHub Profile](https://github.com/avocadohel) (temporalmente compartido)

---

## 📝 Próximos Pasos

- [ ] Definir stack tecnológico
- [ ] Crear documento de arquitectura inicial
- [ ] Configurar proyecto frontend
- [ ] Configurar proyecto backend
- [ ] Agregar CI/CD pipeline
- [ ] Definir modelo de base de datos
- [ ] Configurar autenticación

---

**Última actualización:** 9 de noviembre de 2026
