# 🫒 Abuela Matilde — AOVE Bio Premium

> *Cuatro generaciones de saber, un olivar excepcional y la honestidad como filosofía de empresa.*

Repositorio del sitio de presentación de **Abuela Matilde AOVE Bio Premium**, desplegado como sitio estático en [Vercel](https://vercel.com).

---

## 📄 Documentos

| Archivo | Descripción | Idioma |
|---|---|---|
| `index.html` | Página de bienvenida con acceso a los tres documentos | ES |
| `dosier_abuela_matilde_v3.html` | Dossier completo de presentación del proyecto | ES |
| `dosier_abuela_matilde_v3_EN.html` | Full presentation dossier for international contacts | EN |
| `mercado_competencia_aove_2026.html` | Análisis de mercado y competencia AOVE Premium 2026 | ES |

---

## 🌿 El Proyecto

**Abuela Matilde AOVE Bio Premium** es un aceite de oliva virgen extra ecológico artesanal producido en Torredonjimeno, Jaén, en el corazón de la campiña jiennense — una zona señalada en mapas del Vaticano como zona privilegiada para el olivar ya desde el Imperio Romano.

### Lo que nos hace diferentes

- **Olivar tradicional de secano** en marco 12×12 metros, con grandes olivos de dos y tres patas
- **Variedad Picual** en su máxima expresión: frutado verde intenso, notas a tomatera, hierba recién cortada y un amargor y picor que son señal de salud
- **Cosecha temprana** entre finales de octubre y principios de noviembre, en el punto óptimo de maduración
- **100% del árbol**, recolectada por personas con el método tradicional de fardos (manteos) y varas
- **Sin riego artificial** — solo agua de lluvia
- **Del campo a la botella en el mismo día**, mediante procesos mecánicos en frío por maestros de almazara
- **Solo productos orgánicos** de Gesmontes (Córdoba), empresa especializada en gestión del olivar ecológico
- **Certificación ecológica** y marca registrada ante la OEPM (expediente M4347748)

### Las personas detrás del proyecto

- **Matilde Cañada Gutiérrez** — La abuela. Alma y nombre del proyecto. Su generosidad hizo posible el cambio.
- **Fernando Cañada** (abuelo) — Patriarca. Visionario. Construyó el patrimonio que hoy sostiene el proyecto.
- **Fernando Carpio Cañada** — Cofundador. Hijo de Matilde.
- **José Carpio Cañada** — Cofundador. Hijo de Matilde.
- **Familia Quesada** (José, Paco, Antonio y Luis) — Los encargados del campo. Pilar fundamental del proyecto.
- **Juan Casado · Gesmontes** — Ingeniero agrónomo. Gestión ecológica del olivar.

---

## 🚀 Despliegue

El sitio es **100% estático** — sin framework, sin build step, sin dependencias. Vercel lo despliega directamente desde el repositorio.

### Requisitos

- Cuenta en [Vercel](https://vercel.com)
- Cuenta en [GitHub](https://github.com)
- Git instalado en local

### Pasos

```bash
# 1. Clona o inicializa el repositorio
git clone https://github.com/tu-usuario/abuela-matilde.git
cd abuela-matilde

# 2. (Opcional) Crea el archivo vercel.json para headers de seguridad
cat > vercel.json << 'EOF'
{
  "cleanUrls": true,
  "headers": [
    {
      "source": "/(.*)",
      "headers": [
        { "key": "X-Frame-Options", "value": "DENY" },
        { "key": "X-Content-Type-Options", "value": "nosniff" }
      ]
    }
  ]
}
EOF

# 3. Commit y push
git add .
git commit -m "Initial deploy"
git push origin main
```

### En Vercel

1. Ve a [vercel.com/new](https://vercel.com/new)
2. Importa el repositorio de GitHub
3. Framework Preset: **Other** (static)
4. Haz clic en **Deploy**

✅ En menos de 2 minutos el sitio estará disponible en `abuela-matilde.vercel.app`

### Dominio personalizado (opcional)

Desde el panel de Vercel → Settings → Domains, puedes añadir un dominio propio como `dossier.abuelamatilde.com`.

---

## 🗂 Estructura

```
abuela-matilde/
├── index.html                          # Página de bienvenida
├── dosier_abuela_matilde_v3.html       # Dossier ES
├── dosier_abuela_matilde_v3_EN.html    # Dossier EN
├── mercado_competencia_aove_2026.html  # Análisis de mercado
├── vercel.json                         # Configuración Vercel (opcional)
└── README.md                           # Este archivo
```

---

## 🎨 Stack técnico

- **HTML5 + CSS3 + Vanilla JS** — sin dependencias, sin framework
- **Google Fonts** — Cormorant Garamond, Cinzel, EB Garamond
- **IntersectionObserver API** — animaciones de entrada al hacer scroll
- **Vercel** — hosting estático con CDN global

---

## 📍 Origen

**Torredonjimeno · Jaén · España**

A pocos kilómetros de Córdoba, en el centro de la campiña jiennense, donde a kilómetros a la redonda no hay ninguna empresa contaminante — solo un inmenso mar de olivos.

---

## ©️ Propiedad

© 2026 José Carpio Cañada · Fernando Carpio Cañada  
Marca registrada OEPM — Expediente M4347748  
Todos los derechos reservados. Documento confidencial.

---

*"Ser buena persona a la larga es un negocio."*  
— Manuel José Carpio Bueno, carpintero y agricultor
