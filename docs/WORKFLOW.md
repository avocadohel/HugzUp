# 🔄 Flujo de Trabajo Colaborativo

Guía para trabajar juntas en HugzUp de forma organizada.

## Comunicación

- **Issues**: Para tareas, bugs y decisiones importantes
- **Pull Requests**: Para revisar código antes de mergear
- **Discussiones** (opcional): Para ideas y preguntas

## Proceso de desarrollo

### 1️⃣ Crear una rama

Antes de empezar cualquier trabajo, crea una rama desde `main`:

```bash
git checkout main
git pull origin main
git checkout -b feature/nombre-descriptivo
```

**Formato de ramas:**
- `feature/login-google` - Nueva funcionalidad
- `bugfix/error-notificaciones` - Corrección de bug
- `docs/actualizar-api` - Documentación

### 2️⃣ Hacer cambios

Trabaja en tu rama normalmente:

```bash
git add .
git commit -m "feat: descripción clara del cambio"
git push origin feature/nombre-descriptivo
```

### 3️⃣ Crear Pull Request

En GitHub:
1. Abre un **New Pull Request**
2. Compara tu rama con `main`
3. Escribe descripción clara (qué hace, por qué, cómo probar)
4. Asigna a tu colaboradora para review

Plantilla de PR:
```markdown
## Descripción
Qué hace este PR

## Por qué
Por qué es necesario este cambio

## Cómo probar
Pasos para verificar que funciona

## Checklist
- [ ] Código probado localmente
- [ ] Documentación actualizada (si aplica)
- [ ] Sin conflictos con main
```

### 4️⃣ Review y aprobación

- La otra colaboradora revisa el código
- Puede pedir cambios con comentarios
- Si todo está bien, aprueba el PR

### 5️⃣ Mergear a main

Una vez aprobado:
```bash
# En GitHub, usa "Squash and merge" para mantener historial limpio
# O localmente:
git checkout main
git pull origin main
git merge feature/nombre-descriptivo
git push origin main
```

## Resolver conflictos

Si hay conflictos al mergear:

```bash
# Actualiza tu rama con main
git fetch origin
git merge origin/main

# Resuelve conflictos manualmente en tu editor
# Después:
git add .
git commit -m "fix: resolver conflictos con main"
git push origin feature/nombre-descriptivo
```

## Sincronizar localmente

Antes de empezar trabajo nuevo:

```bash
git checkout main
git fetch origin
git pull origin main
```

## Recomendaciones

✅ **Haz**
- Commits frecuentes con mensajes claros
- PRs pequeños y enfocados (más fáciles de revisar)
- Usa Draft PR si el trabajo está en progreso
- Comunica cambios importantes antes de implementar

❌ **Evita**
- Mergear cambios sin review
- Commits muy grandes con muchos cambios
- Push directo a main
- Mensajes de commit vagos ("arreglé cosas")

## Tareas frecuentes

### Descartar cambios locales
```bash
git checkout -- archivo.txt
# O todos:
git reset --hard origin/main
```

### Ver commits de una rama
```bash
git log main..feature/mi-rama
```

### Cambiar de rama sin commitear
```bash
git stash
git checkout otra-rama
# Después vuelves:
git checkout feature/mi-rama
git stash pop
```
