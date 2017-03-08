Setting Theme Default Buttons
Since the library is enabled on all BoldGrid themes, default styles are applied using various settings from the configs, such as the colors in the palette.  You can define the base styles that you wish to use for .button-primary, and .button-secondary to extend.  T

```php
$boldgrid_framework_configs['components']['buttons']['variables']['button-primary-classes'] = '.btn';
```

On the backend what is essentially happening is that .button-primary extends each of the modifying classes specified to inherit the styles in the compiled CSS output.  The classes are used to say what the buttons will look like.  This can also be used for .button-secondary:

```php
$boldgrid_framework_configs['components']['buttons']['variables']['button-secondary-classes'] = '.btn';
```

With both of these configs applied, .button-primary and .button-secondary are now extending .btn - which is the base class in the BoldGrid Theme Framework Button Library.
Setting Default Button Colors

Button colors are set in a similar way as the color classes can be used to identify which color from the palette should be prominent.  This is done with .btn-color-{#}. Where {#} is, is the color position in your palette.

This example would give .button-primary the first color in your palette, and give .button-secondary the second color in your palette:

```php
$boldgrid_framework_configs['components']['buttons']['variables']['button-primary-classes'] = '.btn, .btn-color-1';
$boldgrid_framework_configs['components']['buttons']['variables']['button-secondary-classes'] = '.btn, .btn-color-2';
```

Setting Button Sizes
Button sizes can be set using the variables configuration option as well.  

The button sizes are:

- Tiny: .btn-tiny
- Small: .btn-small
- Normal: (no class applied)
- Large:  .btn-large
- Jumbo:  .btn-jumbo
- Giant:  .btn-giant

This configuration would set the primary-button to be “tiny” size:

```php
$boldgrid_framework_configs['components']['buttons']['variables']['button-primary-classes'] = '.btn, .btn-color-1, .btn-tiny';
```

Setting Button Shapes
- Squared: (no class applied/default)
- Rounded: .btn-rounded
- Pills: .btn-pill

This would give .button-primary a jumbo sized button using the second color in your palette, in a pill shape:

```php
$boldgrid_framework_configs['components']['buttons']['variables']['button-primary-classes'] = '.btn, .btn-color-2, .btn-jumbo, .btn-pill';
```

Setting Additional Button Styles

The BoldGrid Theme Framework’s button library includes a variety of different styles that can be applied directly to the button-primary and button-secondary classes.  These settings can change the look and feel of the buttons that are used as defaults in the theme.

This example would give the primary-button the third color in the palette, make it a 3D button and give it rounded corners:

```php
$boldgrid_framework_configs['components']['buttons']['variables']['button-primary-classes'] = '.btn, .btn-3d, .btn-color-3, .btn-rounded';
```
