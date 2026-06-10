# affiliate-campaigns

Monorepo de landing pages para campañas de afiliados.  
Desplegado en Vercel con CI/CD automático desde GitHub.

## Estructura

```
affiliate-campaigns/
├── noocube/              ← Campaña: NooCube Brain Productivity v3.0
│   ├── index.html        → /noocube
│   ├── optin.html        → /noocube/optin
│   └── webinar.html      → /noocube/webinar
└── vercel.json
```

## Agregar nueva campaña

```bash
mkdir [nombre-producto]
# crear index.html, optin.html, etc.
# agregar rutas en vercel.json
git add . && git commit -m "feat: campaña [nombre-producto]" && git push
```
Vercel despliega automáticamente en ~30 segundos.

## Variables a reemplazar en cada campaña

- `YOUR_AFFILIATE_LINK` → link real del programa afiliado
- `contacto@biohackingejectivo.com` → tu email
