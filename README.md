# Grav Markdown Font Awesome Plugin

The **Font Awesome plugin** for [Grav](http://github.com/getgrav/grav) allows you to use Font Awesome icons inline with markdown by wrapping the icon name in colons :emoji: style !!

**Updated to work with the last Font Awesome 5 !!** and support to additional `fa` classes such as `fa-spin` and `fa-2x`. _(Doesn't conflicts with Markdown Extra)_

# Examples

```
Font Awesome 5+ :
Grab a cup of :fas fa-coffee: and write some :fas fa-code: to extend :fab fa-grav fa-spin:

Font Awesome :
Grab a cup of :fa fa-coffee: and write some :fa fa-code fa-2x:
```

Will produce the following HTML:

```
Font Awesome 5+ :
Grab a cup of <i class="fas fa-coffee"></i> and write some <i class="fas fa-code"></i> to extend <i class="fab fa-grav fa-spin"></i>

Font Awesome :
Grab a cup of <i class="fas fa-coffee"></i> and write some <i class="fas fa-code fa-2x"></i>
```

# Prerequisites

The plugin works by looking for colon-wrapped icon names starting with the `:fa` prefix and converting them to `<i>` tags.

This plugin doesn't contain the actual Font Awesome fonts, so make sure you are using a plugin or theme (such as Learn2 or Antimatter) that include the Font Awesome assets.

# Manual installation

Download the latest [release](https://github.com/StellarisStudio/grav-plugin-markdown-fontawesome/archive/v1.0.2.zip) of this repository, unzip to `/your-grav/user/plugins` and rename the folder to `markdown-fontawesome`.

# Configuration

The markdown-fontawesome.yaml file contains only one configuration which turns the plugin on/off.

```
enabled: true
```

# Known limitations

- Icon names are not validated, so html tags are created even for non-existent icons like `:fa-not-a-real-icon:`

# Alternatives

If you prefer shortcode syntax `[fa=cog /]`, consider using the [Grav Shortcode Plugin](https://github.com/getgrav/grav-plugin-shortcode-core#fontawesome) which also supports Font Awesome.

# License

MIT license. See [LICENSE](LICENSE)

# Cred

This plugin is a fork of the original work of [Joshua Lotz](https://github.com/yoshikin) found here [markdown-fontawesome](https://github.com/yoshikin/grav-plugin-markdown-fontawesome).

This plugin was inspired by the python markdown extension [fontawesome-markdown](https://github.com/bmcorser/fontawesome-markdown) and the first version was based on code from the [Grav Markdown Color Plugin](https://github.com/getgrav/grav-plugin-markdown-color).
