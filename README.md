# 🚀 Astro Project - Página Dinámica con Markdown  

Este proyecto usa **Astro** para construir una página web dinámica que carga publicaciones desde archivos **Markdown**. Se organiza con **componentes reutilizables** y una plantilla base.  

---

## 📌 Tecnologías Utilizadas  
- **[Astro](https://astro.build/)** - Framework para sitios estáticos  
- **TypeScript** - Tipado seguro  
- **Markdown** - Contenido del blog  
- **Gulp** (opcional) - Automatización de tareas  

---

## 📜 Código Explicado  

### 📥 **Importaciones**  
```ts
import type { IFrontmatter } from 'astro-boilerplate-components';

import { CTA } from '@/partials/CTA';
import { Hero } from '@/partials/Hero';
import { ProjectList } from '@/partials/ProjectList';
import { RecentPosts } from '@/partials/RecentPosts';
import Base from '@/templates/Base.astro';
import { AppConfig } from '@/utils/AppConfig';
import { sortByDate } from '@/utils/Posts';