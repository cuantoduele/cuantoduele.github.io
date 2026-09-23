¿Cuánto duele? ⏱️

**Convertí cualquier precio en horas, días o meses de tu trabajo.**

¿Cuánto duele? es una aplicación web que te muestra lo que realmente te cuesta algo: no en pesos, sino en tiempo de tu vida trabajando. Además te ayuda a planificar cómo ahorrar para eso, a decidir si conviene pagar en cuotas o de contado, y a seguir tu progreso en una lista de deseos.

🔗 **Probala acá:** [manununez1010.github.io/cuanto-duele](https://manununez1010.github.io/cuanto-duele/)

---

## ¿Por qué la hice?

Cuando vemos un precio pensamos en plata, pero la plata es tiempo que pasamos trabajando. Ver que unas zapatillas cuestan "3 días de laburo" cambia completamente la forma de decidir una compra. Quise crear una herramienta simple, gratuita y pensada para el contexto argentino, donde la inflación y las compras en cuotas son parte del día a día.

## Funcionalidades

- **Cálculo en tiempo de trabajo.** Cargás tu sueldo (mensual, quincenal, semanal o por hora) y tu jornada, y cualquier precio se convierte en minutos, horas, días, meses o años de trabajo, eligiendo automáticamente la unidad más clara.
- **Visualización por días.** Una grilla donde cada cuadrado representa una jornada (o semana, o mes, según el tamaño del resultado) que se va llenando.
- **Plan de ahorro diario.** Indicás cuánto podés guardar por día y la app calcula en cuánto tiempo lo tenés y la fecha aproximada en la que llegarías.
- **¿Cuotas o contado?** Compara el precio de contado con un plan de cuotas ajustando por la inflación mensual estimada (valor presente de las cuotas) y da un veredicto claro.
- **Lista de deseos con progreso.** Guardás lo que querés comprar, vas sumando o sacando lo ahorrado y ves una barra de progreso con lo que falta, en plata y en horas de trabajo.
- **Precios actualizables.** Podés editar el precio de un deseo y la app muestra cuánto subió desde que lo anotaste, algo clave con inflación.
- **Historial** de los últimos cálculos.
- **Privacidad total.** No hay registro, cuentas ni servidores: todos los datos se guardan solo en el dispositivo de cada usuario.
- **Diseño adaptable** a celular y computadora, con modo claro y oscuro automático.

## Cómo funcionan los cálculos

| Concepto | Fórmula |
|---|---|
| Horas por mes | horas por semana × 4,33 (52 semanas / 12 meses) |
| Valor de tu hora | sueldo ÷ horas trabajadas en ese período |
| Tiempo de trabajo | precio ÷ valor de tu hora |
| Tiempo de ahorro | precio ÷ ahorro diario (redondeado hacia arriba) |
| Valor hoy de las cuotas | Σ cuota ÷ (1 + inflación mensual)ᵏ, para k = 1…n |

Si el valor actual de las cuotas es menor que el precio de contado, conviene pagar en cuotas; si es mayor, conviene de contado. Si la diferencia es menor al 1%, la app indica que da casi lo mismo.

## Tecnologías

- **HTML, CSS y JavaScript** puros, sin frameworks ni dependencias.
- **localStorage** para guardar los datos en el navegador del usuario.
- **Web Share API** y **Clipboard API** para recomendar la app.
- **Intl / toLocaleString** para el formato de números, moneda y fechas en español de Argentina.
- **CSS Grid, Flexbox** y variables CSS para el diseño responsive y el modo oscuro.
- Tipografía **Archivo** de Google Fonts.
- Publicada con **GitHub Pages**.

Todo está en un único archivo (`index.html`), lo que la hace liviana y rápida de cargar.

## Cómo usarla en tu compu

1. Descargá o cloná este repositorio.
2. Abrí `index.html` con cualquier navegador.

No hace falta instalar nada.


## Autor

**Manu Núñez** · [GitHub](https://github.com/manununez1010)
