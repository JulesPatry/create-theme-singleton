# Theme Singleton

A simple function that builds a theme object to solidify design system rules.

## Root Props

| Prop                        | Description                                                                                                                                                                                                      |
| :-------------------------- | :--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [`palette`](#palette)       | All the colors on the application belong here. Palette begins with: `primary`, `secondary`, `success`, `error`, `info`, `warning`, `text` color.objects.                                                         |
| [`spacing`](#spacing)       | All spacing units belong here. These units should be variables for only `margin` and `padding` styles. For global width and heights refer to [sizing].                                                           |
| [`shape`](#shape)           |                                                                                                                                                                                                                  | (#sizing) |
| [`typography`](#typography) |                                                                                                                                                                                                                  |
| [`breakpoints`](#palette)   | All breakpoints such as `xs`, `sm`, `md`, `lg`, `xl` and `custom` edge cases. Custom edge cases should be specific layout for feature of an application.                                                         |
| [`movement`](#palette)      | All css transitions are stored here.here.                                                                                                                                                                        |
| [`shadows`](#shadows)       |                                                                                                                                                                                                                  |
| [`zIndex`](#zIndex)         |                                                                                                                                                                                                                  |
| [`heights`](#sizing)        | All global heights can be accessible here. A common example is giving other components access navbar height. These height / width rules should be defined by your design system.                                 |
| [`widths`](#sizing)         | All global widths belong here. A common example is maximum width for paragraph styles (It's challenging to read from a 1200 width document). These height / width rules should be defined by your design system. |

## Palette

All the colors on the application belong here. Palette begins with: `primary`, `secondary`, `success`, `error`, `info`, `warning`, `text` color objects.

### Color object (`primary`, `secondary`, `success`, `error`, `info`, and `warning`)

| Key            | Description                                                                                                                      |
| :------------- | :------------------------------------------------------------------------------------------------------------------------------- |
| `allure`       | A lighter color of the default value. Common use cases should be on button hover, on focus, switch on, and radio button selected |
| `default`      | Default color                                                                                                                    |
| `deter`        | A lighter color of the default value. Common use cases should be on mouse down, switch off, radio not selected, and disabled.    |
| `contrastText` | Refer to text object colors. This value should mirror either the `text.onLightSurface` or `text.onDarkSurface`.                  |

### Text object

| Key              | Description                                                                                                   |
| :--------------- | :------------------------------------------------------------------------------------------------------------ |
| `default`        | Default color for whole application. This value should mirror either the `onLightSurface` or `onDarkSurface`. |
| `onLightSurface` | The default text color applied to text on a white or light background                                         |
| `onDarkSurface`  | The default text color applied to text on a black or dark background                                          |

### Common Colors object

| Key      | Description                        |
| :------- | :--------------------------------- |
| `white`  | Global white color. `#fff`         |
| `black`  | Global black color. `#212121`      |
| `gray`   | Global gray color. `#d3d3d3`       |
| `border` | Uses global black color. `#212121` |

## Spacing

| Key    | Description                                                                                                                                          |
| :----- | :--------------------------------------------------------------------------------------------------------------------------------------------------- |
| `unit` | The default unit for spacing. These units should be variables for only `margin` and `padding` styles. For global width and heights refer to [sizing] |

## Breakpoints

## Movement

## Sizing

All global widths and heights belong here. A common example is maximum width for paragraph styles (It's challenging to read from a 1200 width document). These height / width rules should be defined by your design system. Sizing is separating into two different keys to prevent confusion occurring on naming conventions. Rather than having a root sizing object with names like navBarHeight and cardWidth, it works better when height and width are the key that represent these values. The default value for width nd heights are `{}`
