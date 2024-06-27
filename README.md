# Theme Name

## Features

### Shortcodes

Shortcodes use the [Hugo shortcode syntax] (i.e.: `{{< shortcode params >}}` or `{{% shortcode params %}}`):

| Shortcode                    | Description        |
|------------------------------|--------------------|
| [`resume`][shortcode.resume] | Renders the resume |

[shortcode.resume]: #resume

[Hugo shortcode syntax]: https://gohugo.io/content-management/shortcodes/

#### Resume

Rendered using the `resume` shortcode. Renders the resume as it would be in the `/about/` page, by using the `resume.toml` file in your assets directory.

## Installation

## Configuration

Configuration is done by putting keys in the `[params]` dictionary:

| Key                             | Type       | Description                                                                                                      |
|---------------------------------|------------|------------------------------------------------------------------------------------------------------------------|
| `home.pageCount`                | `integer`  | Limits the number of recent posts displayed under the main content, including the spotlight post.                |
| `home.paginate`                 | `string[]` | List of sections that can be paginated in the home page.                                                         |
| `home.spotlight.characterLimit` | `integer`  | Limits how many characters get rendered in the spotlight view (without cutting out words or breaking HTML tags). |
| `home.resume`                   | `boolean`  | Enables or disables the resume being rendered in the home page.                                                  |
| `subtitle`                      | `string`   | The subtitle for the website (which is rendered underneath the website title).                                   |

### Populating Your Resume

To configure your resume, you need to create a `resume.toml` file in your assets directory and populate it with the appropriate key/value pairs.
