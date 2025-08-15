# Translation Guide

This guide explains how to add translated transcripts to Open Source Stories.

## Adding a New Language

The system automatically detects available translations without requiring Hugo configuration changes. Simply create the translated content files and the language switcher will appear automatically.

**Note**: For languages other than Spanish, you may need to add them to Hugo's language configuration in `config.toml`:

```toml
[languages.fr]  # Example for French
  languageCode = "fr"
  languageName = "Français"
  title = "Histoires Open Source"
  weight = 3
```

## Translating Content

### Story Transcripts

To translate a story transcript:

1. **Create Language Directory**:

   ```
   content/
   ├── stories/           # English (default)
   └── es/               # Spanish translations
       └── stories/
   ```

2. **Translate Content**: Copy the original story file and translate:

   ```
   content/es/stories/2021/aaron-patterson.md
   ```

3. **Link Translations**: Ensure both files have the same filename to be automatically linked.

### Front Matter

Keep the same front matter structure but translate user-facing content:

```yaml
---
title: 'Título Traducido'
date: 2021-01-01
author: 'aaron patterson'
bio: 'Biografía traducida...'
# Keep technical fields unchanged
storycorps: '12345'
---
```

## File Structure Example

```
content/
├── stories/
│   └── 2021/
│       └── aaron-patterson.md     # English (original)
├── es/
│   └── stories/
│       └── 2021/
│           └── aaron-patterson.md # Spanish translation
└── fr/
    └── stories/
        └── 2021/
            └── aaron-patterson.md # French translation
```

## Testing Translations

1. Run Hugo locally: `hugo server`
2. Navigate to translated content: `http://localhost:1313/es/stories/2021/aaron-patterson/`
3. Verify language switcher appears and works correctly
4. Test switching between languages using the dropdown

## Language Switcher Behavior

- **Automatic Detection**: The system automatically detects available translations without manual configuration
- **Default Language**: English (en) is always the default selection
- **Available Languages**: Only languages with actual translated content appear in the dropdown
- **No Duplicates**: Each language appears only once in the dropdown
- **Dynamic Display**: The switcher only appears when translations exist for that specific content

## Notes

- The language switcher automatically detects Spanish translations in the `/es/` directory
- Audio content remains the same across all language versions
- Only translate the transcript content, not technical metadata
- Each user sees only the languages available for their specific content
