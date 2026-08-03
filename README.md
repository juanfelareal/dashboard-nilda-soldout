# Dashboard Sold Out - Nilda Chiaraviglio

Dashboard para trackear el progreso de venta de boletas para los eventos de Nilda en Bogotá y Medellín.

**URL del Dashboard:** https://juanfelareal.github.io/dashboard-nilda-soldout/

---

## Configuración del Google Sheet

### 1. Crear el Google Sheet

Crea un nuevo Google Sheet con **dos hojas** (tabs):
- `Medellin` (sin tilde)
- `Bogota` (sin tilde)

### 2. Estructura de cada hoja

Cada hoja debe tener 3 columnas:

| Fecha | Boletas | Inversion |
|-------|---------|-----------|
| 2025-07-31 | 293 | 0 |
| 2025-08-01 | 310 | 150000 |
| 2025-08-02 | 325 | 300000 |

**Importante:**
- `Fecha`: Formato YYYY-MM-DD (ej: 2025-08-01)
- `Boletas`: Número **acumulado** total de boletas vendidas
- `Inversion`: Número **acumulado** total invertido en pauta (sin símbolos, solo el número)

### 3. Datos iniciales

**Medellín (al 31 de julio):**
| Fecha | Boletas | Inversion |
|-------|---------|-----------|
| 2025-07-31 | 293 | 0 |

**Bogotá (al 31 de julio):**
| Fecha | Boletas | Inversion |
|-------|---------|-----------|
| 2025-07-31 | 296 | 0 |

### 4. Publicar el Google Sheet

1. Ve a **Archivo → Compartir → Publicar en la web**
2. Selecciona **"Todo el documento"**
3. Formato: **CSV**
4. Clic en **Publicar**
5. Copia el **ID del sheet** de la URL

El ID es la parte larga en la URL:
```
https://docs.google.com/spreadsheets/d/[ESTE-ES-EL-ID]/edit
```

### 5. Conectar al Dashboard

1. Ve al dashboard: https://juanfelareal.github.io/dashboard-nilda-soldout/
2. Pega el ID del Google Sheet en el campo
3. Clic en **Conectar**

---

## Cómo actualizar los datos

### Sandra (Boletas vendidas):
1. Cada día, agrega una nueva fila con la fecha
2. Pon el número **total acumulado** de boletas vendidas hasta ese día
3. Deja la columna Inversion igual al día anterior (o vacía)

### Juan (Inversión en pauta):
1. Cada día, actualiza la columna `Inversion` con el total acumulado invertido
2. O agrega una nueva fila si Sandra no lo ha hecho

---

## Métricas del Dashboard

- **Boletas vendidas:** Progreso vs meta (1,000 por evento)
- **Inversión en pauta:** Gasto vs presupuesto ($3M por evento)
- **CPA:** Costo por boleta vendida
- **Velocidad:** Boletas por día (últimos 7 días)
- **Proyección:** Estimación de boletas al día del evento

---

## Eventos

| Ciudad | Fecha | Meta | Presupuesto Pauta |
|--------|-------|------|-------------------|
| Bogotá | 19 de agosto 2026 | 1,000 | $3,000,000 |
| Medellín | 22 de agosto 2026 | 1,000 | $3,000,000 |

---

*Dashboard creado por LA REAL*
