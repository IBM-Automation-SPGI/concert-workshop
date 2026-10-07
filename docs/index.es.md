# IBM Concert Workshop

<div style="background: linear-gradient(135deg, #0043ce 0%, #001141 60%, #0f62fe 100%); border-radius: 12px; padding: 3rem 2.5rem; margin: 1.5rem 0 2.5rem 0; text-align: center; box-shadow: 0 8px 32px rgba(0,67,206,0.35);">
  <div style="font-size: 0.85rem; font-weight: 600; letter-spacing: 0.18em; color: #78a9ff; text-transform: uppercase; margin-bottom: 0.6rem;">IBM Client Engineering</div>
  <div style="font-size: 2.4rem; font-weight: 700; color: #ffffff; letter-spacing: -0.01em; line-height: 1.15; margin-bottom: 0.5rem;">IBM Concert Workshop</div>
  <div style="font-size: 1.1rem; color: #a8c8ff; font-weight: 300; margin-bottom: 1.4rem;">Agentic ITOps · Observabilidad · Resiliencia · Optimización</div>
  <div style="display: inline-flex; gap: 0.75rem; flex-wrap: wrap; justify-content: center;">
    <span style="background: rgba(255,255,255,0.12); border: 1px solid rgba(255,255,255,0.25); border-radius: 20px; padding: 0.3rem 1rem; color: #ffffff; font-size: 0.8rem; font-weight: 500;">🛡️ Concert Protect</span>
    <span style="background: rgba(255,255,255,0.12); border: 1px solid rgba(255,255,255,0.25); border-radius: 20px; padding: 0.3rem 1rem; color: #ffffff; font-size: 0.8rem; font-weight: 500;">🔭 Concert Observe</span>
    <span style="background: rgba(255,255,255,0.12); border: 1px solid rgba(255,255,255,0.25); border-radius: 20px; padding: 0.3rem 1rem; color: #ffffff; font-size: 0.8rem; font-weight: 500;">⚡ Concert Resilience</span>
    <span style="background: rgba(255,255,255,0.12); border: 1px solid rgba(255,255,255,0.25); border-radius: 20px; padding: 0.3rem 1rem; color: #ffffff; font-size: 0.8rem; font-weight: 500;">📊 Concert Optimize</span>
    <span style="background: rgba(255,255,255,0.12); border: 1px solid rgba(255,255,255,0.25); border-radius: 20px; padding: 0.3rem 1rem; color: #ffffff; font-size: 0.8rem; font-weight: 500;">🔄 Concert Workflows</span>
  </div>
</div>

!!! info "Bienvenido/a al Workshop de IBM Concert"
    Este workshop práctico te guiará por las principales funcionalidades de **IBM Concert**, la plataforma agentic de ITOps que unifica observabilidad, protección, operaciones y optimización en un único sistema inteligente.

    **URL de la plataforma**: `https://concert.tec.spgi.ibm.com:12443`  
    **Usuario**: `ibmconcert`  
    **Duración estimada**: 4–5 horas

---

## ¿Qué es IBM Concert?

IBM Concert es una plataforma agentic de ITOps que crea una capa operacional unificada y adaptable en todo tu entorno. Conecta señales, genera contexto compartido y coordina acciones entre equipos y herramientas para que todo el sistema funcione como uno.

```mermaid
graph LR
    subgraph CONCERT["🎵 IBM CONCERT - Plataforma Agentic ITOps"]
        direction TB
        OBS["🔭 Concert Observe<br/>Observabilidad Full-Stack"]
        PRO["🛡️ Concert Protect<br/>Vulnerabilidades & Riesgo"]
        OPE["⚙️ Concert Resilience<br/>Respuesta a Incidentes"]
        OPT["📊 Concert Optimize<br/>Recursos & Costes"]
        WFL["🔄 Concert Workflows<br/>Automatización Low-Code"]
        RES["🔁 Concert Resilience<br/>Recuperación & Fiabilidad"]
    end

    APP["Aplicaciones"] --> CONCERT
    INFRA["Infraestructura"] --> CONCERT
    NET["Red"] --> CONCERT
    CONCERT --> ACTION["✅ Insight → Acción"]

    style CONCERT fill:#e8f0fe,stroke:#0043ce,stroke-width:2px
    style OBS fill:#e0f7fa,stroke:#009d9a
    style PRO fill:#fde8e8,stroke:#da1e28
    style OPE fill:#e3f2fd,stroke:#0f62fe
    style OPT fill:#e8f5e9,stroke:#198038
    style WFL fill:#f3e5f5,stroke:#8a3ffc
    style RES fill:#fff3e0,stroke:#ff832b
```

---

## Módulos del Workshop

| Lab | Módulo | Descripción | Duración |
|-----|--------|-------------|----------|
| 🚀 **Lab 0** | Prerequisitos | Verificación de entorno y acceso a Concert | 10 min |
| 🏠 **Lab 1** | Introducción | Navegación y dashboard principal de Concert | 15 min |
| 🛡️ **Lab 2** | Concert Protect | Gestión de vulnerabilidades CVE y SBOM | 25 min |
| 🔭 **Lab 3** | Concert Observe | Observabilidad full-stack con IBM Instana | 20 min |
| ⚙️ **Lab 4** | Concert Resilience | Gestión de incidentes y respuesta | 20 min |
| 📊 **Lab 5** | Concert Optimize | Optimización de recursos con IBM Turbonomic | 15 min |
| 🔄 **Lab 6** | Concert Workflows | Automatización de flujos de trabajo | 15 min |

---

## Arquitectura del Entorno

```mermaid
graph TB
    subgraph CLIENTE["Tu Entorno"]
        BROWSER["🌐 Navegador Web<br/>(Chrome/Firefox)"]
    end

    subgraph CONCERT_ENV["Entorno IBM Concert (Demostración)"]
        direction TB
        CONCERT_UI["Concert UI<br/>:12443/platform"]
        API["Concert API"]
        DB["Base de Datos<br/>de Configuración"]
        AI["Motor IA<br/>Agente IBM"]
        
        subgraph MONITORED["Aplicaciones Monitorizadas"]
            APP1["App: RobotShop"]
            APP2["App: BookInfo"]
            APP3["App: Sock Shop"]
        end
    end

    BROWSER -->|HTTPS| CONCERT_UI
    CONCERT_UI --> API
    API --> DB
    API --> AI
    API --> MONITORED

    style CONCERT_ENV fill:#e8f0fe,stroke:#0043ce,stroke-width:2px
    style MONITORED fill:#f4f4f4,stroke:#525252
```

---

## Prerequisitos

!!! warning "Antes de comenzar"
    Asegúrate de tener lo siguiente disponible:

- [x] Acceso a un navegador moderno (Chrome 90+ o Firefox 88+)
- [x] Acceso a la URL del entorno Concert
- [x] Credenciales facilitadas por el instructor
- [x] Conexión a la red del laboratorio

---

## Política de seguridad del workshop

!!! danger "Aviso de seguridad"
    Las credenciales proporcionadas son **exclusivamente para uso en este workshop**. No compartir fuera del entorno de laboratorio. El entorno se reseteará al finalizar la sesión.

---

## Soporte durante el workshop

Si encuentras algún problema durante los laboratorios:

1. Consulta la sección **"Solución de problemas"** al final de cada lab
2. Pide ayuda al instructor
3. Revisa los logs de la plataforma Concert en `Configuración > Logs`
