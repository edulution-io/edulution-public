# SOGo themes

Public mirror of the edulution SOGo webmail themes.

These CSS files are the source of truth the edulution platform fetches to check
for and apply SOGo theme updates. They are mirrored from the (private)
`edulution-io/edulution-mail` repository at `build/templates/sogo/`.

| File | `@theme` |
| --- | --- |
| `custom-theme.css` | `edulution-dark` |
| `light-theme.css` | `edulution-light` |

Each file carries a header the platform parses:

```css
/* @theme edulution-dark
   @version 0.1.9
*/
```

When the theme changes in `edulution-mail`, update these files (and bump the
`@version`) so deployments detect the new version.
