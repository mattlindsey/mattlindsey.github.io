# Jekyll Site Knowledge

## Core Info
- Running Jekyll 4.3.4
- Uses kramdown markdown processor
- Uses Sass/SCSS for styling

## Configuration
- Site is configured via _config.yml
- Uses standard Jekyll directory structure (_includes, _layouts, _posts, etc.)

## Styling
- SCSS files are in _sass directory
- Main SCSS entry point is css/main.scss
- Mixins must be defined before they are used
- Using traditional @import syntax instead of newer @use/@forward for Jekyll compatibility
- Color functions use deprecated lighten/darken - acceptable for now despite warnings
- Sass deprecation warnings expected and can be ignored
- Bootstrap classes (text-center) do not reliably center images
- Image centering requires both display:block AND margin:auto AND parent container width control
- Avoid relying on Bootstrap utilities for core layout - use direct CSS/SCSS instead

## Dependencies
- Requires csv gem for Jekyll 4.3.4
- Requires base64 gem for safe_yaml
- Uses webrick for serving

- Accepting Sass deprecation warnings to maintain compatibility
## Common Issues
- SCSS compilation errors often occur if mixins aren't properly defined/imported
- Color module syntax (color.adjust) is not compatible - use traditional Sass color functions
