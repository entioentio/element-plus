# Layout

Quickly and easily create layouts with the basic 24-column.

:::tip

The component uses flex layout by default, no need to set `type="flex"` manually.

Please note that the parent container should avoid using `inline` related styles,
which will cause the component to not fill up its width.

:::

## Basic layout

Create basic grid layout using columns.

:::demo With `row` and `col`, we can easily manipulate the layout using the `span` attribute.

layout/basic-layout

:::

## Column spacing

Column spacing is supported.

:::demo Row provides `gutter` attribute to specify spacings between columns, and its default value is 0.

layout/column-spacing

:::

## Hybrid layout

Form a more complex hybrid layout by combining the basic 1/24 columns.

:::demo

layout/hybrid-layout

:::

## Column offset

You can specify column offsets.

:::demo You can specify the number of column offset by setting the value of `offset` attribute of Col.

layout/column-offset

:::

## Alignment

Default use the flex layout to make flexible alignment of columns.

:::demo You can define the layout of child elements by setting `justify` attribute with start, center, end, space-between or space-around.

layout/alignment

:::

## Responsive Layout

Taking example by Bootstrap's responsive design, five breakpoints are preset:
xs, sm, md, lg and xl.

:::demo

layout/responsive-layout

:::

## Utility classes for hiding elements

Additionally, Element Plus provides a series of classes for hiding elements under
certain conditions. These classes can be added to any DOM elements or custom components.
You need to import the following CSS file to use these classes:

```js
import 'element-plus/lib/theme-chalk/display.css'
```

The classes are:

- `hidden-xs-only` - hide when on extra small viewports only
- `hidden-sm-only` - hide when on small viewports and down
- `hidden-sm-and-down` - hide when on small viewports and down
- `hidden-sm-and-up` - hide when on small viewports and up
- `hidden-md-only` - hide when on medium viewports only
- `hidden-md-and-down` - hide when on medium viewports and down
- `hidden-md-and-up` - hide when on medium viewports and up
- `hidden-lg-only` - hide when on large viewports only
- `hidden-lg-and-down` - hide when on large viewports and down
- `hidden-lg-and-up` - hide when on large viewports and up
- `hidden-xl-only` - hide when on extra large viewports only

## Row Attributes

| Attribute | Description                         | Type   | Accepted Values                             | Default |
| --------- | ----------------------------------- | ------ | ------------------------------------------- | ------- |
| gutter    | grid spacing                        | number | —                                           | 0       |
| justify   | horizontal alignment of flex layout | string | start/end/center/space-around/space-between | start   |
| align     | vertical alignment of flex layout   | string | top/middle/bottom                           | top     |
| tag       | custom element tag                  | string | \*                                          | div     |

## Col Attributes

| Attribute | Description                                         | Type                                      | Accepted Values | Default |
| --------- | --------------------------------------------------- | ----------------------------------------- | --------------- | ------- |
| span      | number of column the grid spans                     | number                                    | —               | 24      |
| offset    | number of spacing on the left side of the grid      | number                                    | —               | 0       |
| push      | number of columns that grid moves to the right      | number                                    | —               | 0       |
| pull      | number of columns that grid moves to the left       | number                                    | —               | 0       |
| xs        | `<768px` Responsive columns or column props object  | number/object (e.g. {span: 4, offset: 4}) | —               | —       |
| sm        | `≥768px` Responsive columns or column props object  | number/object (e.g. {span: 4, offset: 4}) | —               | —       |
| md        | `≥992px` Responsive columns or column props object  | number/object (e.g. {span: 4, offset: 4}) | —               | —       |
| lg        | `≥1200px` Responsive columns or column props object | number/object (e.g. {span: 4, offset: 4}) | —               | —       |
| xl        | `≥1920px` Responsive columns or column props object | number/object (e.g. {span: 4, offset: 4}) | —               | —       |
| tag       | custom element tag                                  | string                                    | \*              | div     |
