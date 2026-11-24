# Mòdul Odoo: School

![CFGS DAM](https://img.shields.io/badge/CFGS-Desenvolupament%20d%27Aplicacions%20Multiplataforma%20%28DAM%29-green?style=for-the-badge)
![SGE](https://img.shields.io/badge/assignatura-Sistemes%20de%20Gesti%C3%B3%20Empresarial-purple?style=for-the-badge)
![Odoo](https://img.shields.io/badge/Odoo-M%C3%B2dul-714B67?style=for-the-badge&logo=odoo&logoColor=white)

Mòdul d'Odoo per gestionar una escola: cursos, edicions, assignatures, professorat i la seva docència. Pràctica 1 de l'assignatura de Sistemes de Gestió Empresarial (SGE) del CFGS de Desenvolupament d'Aplicacions Multiplataforma (Institut Milà i Fontanals, Igualada), curs 2025-2026.

La pràctica 2 amplia aquest mòdul: [SGE_P2_Odoo_modul_school_plus](https://github.com/sarapratsm/SGE_P2_Odoo_modul_school_plus).

## Models

| Model | Descripció |
|---|---|
| `school.course` | Cursos. |
| `school.course.edition` | Edicions (convocatòries) d'un curs. |
| `school.subject` | Assignatures. |
| `school.course.subject` | Assignatures que componen cada curs, amb el seu ordre. |
| `school.thematic` | Temàtiques. |
| `school.teacher` | Professorat, amb les assignatures que està autoritzat a impartir. |
| `school.teaching` | Docència: qui imparteix què en cada edició. |
| `school.teacher.salary.history` | Historial salarial del professorat. |
| `school.statistics` | Model transitori per a estadístiques. |

## Funcionalitats

- Grups de seguretat: *Nothing*, *Teacher* i *Manager*.
- Assistent (*wizard*) que compta quantes edicions d'un curs comencen entre dues dates.
- Informes PDF de curs, edició i professor.
- Quadres de comandament (`board`).
- Traducció al català (`i18n/ca_ES.po`).

## Instal·lació

1. Copia la carpeta al directori `addons` d'Odoo **amb el nom `school`** (el mòdul d'ampliació en depèn per aquest nom).
2. Reinicia el servidor, actualitza la llista d'aplicacions i instal·la **School**.
3. Dependències: `base` i `board`.

## Autoria

Grup DAM2, curs 2025-2026 · Llicència LGPL-3
