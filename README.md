# route-builder
Typescript class to declaratively and simply create organized navigation paths


## Example

```typescript
const rb = new RouteBuilder()
const dashboardPages = rb.root({
  basepath: '/dashboard',
  nodes: [
    rb.node('Escuelas', '/escuelas'),
    rb.node('Comisiones de evaluación', '/comisiones'),

    rb.node('Turnos', '/turnos'),
    rb.node('Evaluaciones', '/evaluaciones'),
    rb.node('Estudiantes', '/estudiantes'),
    rb.node('Comisiones', '/comisiones'),
    rb.node('Roles', '/roles'),
  ]
}).buildRoute()
```
