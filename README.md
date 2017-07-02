# ACF Price Field

ACF Price field with number formatting.

-----------------------

### Description

**How it works**
- Plugin will store your "price" as float so any time you will change desire number format there will be no reformatting problems.
- Best column type in database for "price" related fields is decimal. As WordPress keep meta as type "text"  I can only cast it to float. Keep it in mind.
- Field validation is "live" thanks to https://github.com/teamdf/jquery-number.
- When you use `get_field` function you will get preformatted number based on your settings.

**Options**
`format`

Available formats:
- `1 337.55`
- `1 337,55`
- `1,337.55`
- `1.337,55`
- `1337`
- `1 337`


**Default parameters result**
`1 337.00`

### Compatibility

This ACF field type is compatible with:
* ACF 5

### Installation

1. Copy the `acf-price` folder into your `wp-content/plugins` folder
2. Activate the Price plugin via the plugins admin page
3. Create a new field via ACF and select the Price type
4. Please refer to the description for more info regarding the field type settings

### TODO
[ ] composer.json
[ ] readme.txt for WP plugin repository
[ ] `apply_filter` for format choices
[ ] Translations

### CHANGELOG
##### [1.1.0] 2017-06-17
- added `format` option
- removed support for ACF 4 (temporary)

##### [1.0.0] 2015-02-02
- Initation of plugin, no configuration. Only live validation.