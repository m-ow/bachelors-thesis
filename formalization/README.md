# Confluencia de la reducción $\eta$ en Lean

En este trabajo los términos del cálculo $\lambda$ se escriben mediante la representación *locally nameless*: 
las variables libres conservan sus nombres y las ligadas se expresan mediante índices de de Bruijn.

El resultado final es el teorema de Church-Rosser para la reducción $\eta$, el cual expresa
que dos sucesiones finitas de reducciones $\eta$ con el mismo origen pueden extenderse hasta alcanzar un término en común.

## Organización

| Archivo | Contenido |
| --- | --- |
| `Formalization/Relations.lean` | Relaciones, clausuras, propiedad del diamante y confluencia. |
| `Formalization/Lambda.lean` | Términos, variables libres, apertura, cierre, clausura local y sustitución. |
| `Formalization/Eta.lean` | Reducción $\eta$ y lemas auxiliares. |
| `Formalization/ChurchRosser.lean` | Demostración de la confluencia de la reducción $\eta$. |

### Versiones

- Lean: `4.35.0-rc3`. 
- Mathlib: `v4.35.0-rc3`. 

### Compilación

Se requieren git y [elan](https://github.com/leanprover/elan). 

Desde la raíz del repositorio: 

```sh
cd formalization
lake exe cache get
lake build
```
