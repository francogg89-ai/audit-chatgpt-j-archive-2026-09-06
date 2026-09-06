# BOOTSTRAP — AUDITOR

## Constitución

```text
WORK_ID=prueba-orquestador-30-vueltas-ai
CARRIL=J
ROL=AUDITOR
```

Este archivo registra hechos de constitución del trabajo. No representa estado vivo.

## Manifiesto de constitución

```text
MANIFEST_REPO=https://github.com/francogg89-ai/manifiestos-trabajo-ai
MANIFEST_PATH=manifiestos/prueba-orquestador-30-vueltas-ai/MANIFIESTO_TRABAJO.md
MANIFEST_SHA=4b03bb6dd93658d473f24d957134752bd35c9aeb
PROJECT.md=NO_EXISTE
```

## Método gobernante

```text
METHOD_REPO=https://github.com/francogg89-ai/revolutions-orchestra-ai
METHOD_SHA=e05b24cc501ce839ffabee6d9666d069e056255c
METHOD_PATHS=
- metodo/REVOLUTIONS.md
- metodo/ROL-AUDITOR.md
- metodo/ROL-CONSTRUCTOR.md
```

## Repositorios constitutivos

```text
WORK_REPO=https://github.com/francogg89-ai/work-claude-j
AUDIT_REPO=https://github.com/francogg89-ai/audit-chatgpt-j
```

Fuentes de autoridad congeladas por esta constitución:

- `https://github.com/francogg89-ai/revolutions-orchestra-ai` en `METHOD_SHA`.
- `https://github.com/francogg89-ai/manifiestos-trabajo-ai` en `MANIFEST_SHA`.

Referencias operativas declaradas por la constitución, sin SHA adicional suministrado en el paquete:

- `https://github.com/francogg89-ai/rules-orchestrator-ai`.
- `https://github.com/francogg89-ai/metodo-manifiestos-ai`.

## Raíz y rutas locales declaradas

```text
ROOT_LOCAL=C:\Franco_Metodos_AI

RULES_ORCHESTRATOR=C:\Franco_Metodos_AI\rules-orchestrator-ai
WORK=C:\Franco_Metodos_AI\work-claude-j
AUDIT=C:\Franco_Metodos_AI\audit-chatgpt-j
METODO_MANIFIESTOS=C:\Franco_Metodos_AI\metodo-manifiestos-ai
MANIFIESTOS=C:\Franco_Metodos_AI\manifiestos-trabajo-ai
METHOD=C:\Franco_Metodos_AI\revolutions-orchestra-ai
```

## Entornos relevantes

- **ORQUESTADOR**: ejecución local; transporta entre los actores conforme a `REGLAS-ORQUESTADOR.md`.
- **CONSTRUCTOR**: Claude Code local sobre Windows, trabajando desde `C:\Franco_Metodos_AI\work-claude-j`.
- **AUDITOR**: conversación de ChatGPT con acceso a GitHub, trabajando sobre `audit-chatgpt-j`.

## Capacidades inicialmente delegadas

### CONSTRUCTOR

- lectura y sincronización de los repositorios declarados necesarios para reconstruir el trabajo;
- operación local mediante Claude Code;
- lectura del método y del manifiesto exactos congelados por esta constitución;
- creación, modificación, verificación, commit y publicación de material exclusivamente en `work-claude-j` dentro del alcance del trabajo;
- uso de Git para derivar la situación conforme a REVOLUTIONS.

Frontera estructural de escritura: no puede modificar `audit-chatgpt-j`, `revolutions-orchestra-ai`, `rules-orchestrator-ai`, `metodo-manifiestos-ai` ni `manifiestos-trabajo-ai`.

### AUDITOR

- lectura de los repositorios GitHub declarados necesarios para reconstruir y auditar;
- lectura del método y del manifiesto exactos congelados por esta constitución;
- creación, modificación, commit y publicación de material exclusivamente en `audit-chatgpt-j` dentro del alcance del trabajo;
- auditoría de las entregas de `work-claude-j` conforme a REVOLUTIONS;
- uso de Git como fuente autoritativa para derivar entregas, intervenciones y cadencias;
- decisión de próximas acciones y relevos metodológicamente habilitados;
- declaración de `NECESIDAD DEL HUMANO` cuando corresponda;
- declaración del cierre únicamente cuando los criterios del manifiesto estén satisfechos.

Frontera estructural de escritura: no puede modificar `work-claude-j`, `revolutions-orchestra-ai`, `rules-orchestrator-ai`, `metodo-manifiestos-ai` ni `manifiestos-trabajo-ai`.

## Credenciales y secretos

La constitución declara que no existen credenciales ni secretos necesarios para esta prueba.

## Políticas de ejecución iniciales

- El trabajo material debe ser deliberadamente trivial.
- El CONSTRUCTOR debe producir el PLAN mínimo compatible con REVOLUTIONS.
- Después del PLAN, debe usarse una única unidad sencilla y determinista.
- La corrida debe alcanzar treinta entregas principales del CONSTRUCTOR.
- Cada entrega del CONSTRUCTOR debe ser auditada antes de continuar.
- No debe existir un contador durable paralelo de vueltas.
- Las cantidades y cadencias se derivan desde las historias Git conforme al método.
- Relevo periódico de CONSTRUCTOR: cada 10 entregas del CONSTRUCTOR, sobre múltiplos absolutos.
- Relevo periódico de AUDITOR: cada 12 intervenciones del AUDITOR, sobre múltiplos absolutos.
- Un relevo manual no reinicia ni desplaza ninguna de las dos grillas.
- El ORQUESTADOR no cuenta ni decide cuándo corresponde un relevo.
- El actor metodológicamente competente determina el relevo y lo expresa mediante `next_instance`.
- El HUMANO puede durante la corrida ordenar `DETENER` y posteriormente emitir `RELEVAR CONSTRUCTOR`, `RELEVAR AUDITOR` o `CONTINUAR`, conforme a las reglas del ORQUESTADOR y REVOLUTIONS.
- Un relevo humano adicional tampoco reinicia las cadencias periódicas.
- No se debe abrir artificialmente una instancia fresca por un relevo periódico si el trabajo ya está cerrando y no existe una nueva intervención que entregar a ese actor.
- El AUDITOR no puede declarar `final=true` antes de que existan treinta entregas principales del CONSTRUCTOR, la trigésima haya sido auditada y no exista una entrega pendiente.
- Una falla real del transporte debe exponerse y detenerse conforme al comportamiento fail-closed; no debe ocultarse para alcanzar artificialmente las treinta entregas.

## Intervención constitutiva del AUDITOR

```text
PERIMETRO_ULTIMA_MODIFICACION=CONSTITUCION
PROXIMA_ACCION=Constituir el primer CONSTRUCTOR como instancia fresh mediante el sobre inicial turn_id=1; deberá crear su BOOTSTRAP.md preservando la identidad exacta de este bootstrap y producir el PLAN mínimo compatible con REVOLUTIONS y el manifiesto.
```
