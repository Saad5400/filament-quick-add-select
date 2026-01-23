# Contributing to Filament Quick Add Select

Thank you for considering contributing to Filament Quick Add Select! We welcome contributions from the community.

## How Can I Contribute?

### Reporting Bugs

Before creating bug reports, please check the existing issues to avoid duplicates. When creating a bug report, include as many details as possible:

- **Clear title** - Use a descriptive title
- **Steps to reproduce** - Detailed steps to reproduce the issue
- **Expected behavior** - What you expected to happen
- **Actual behavior** - What actually happened
- **Environment** - PHP version, Laravel version, Filament version
- **Screenshots** - If applicable

### Suggesting Enhancements

Enhancement suggestions are tracked as GitHub issues. When creating an enhancement suggestion:

- **Use a clear title** - Describe the enhancement
- **Provide detailed description** - Explain why this enhancement would be useful
- **Include examples** - Show how it would work

### Pull Requests

We actively welcome your pull requests:

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Make your changes
4. Follow the coding standards (see below)
5. Write or update tests if applicable
6. Update documentation if needed
7. Commit your changes (`git commit -m 'Add amazing feature'`)
8. Push to the branch (`git push origin feature/amazing-feature`)
9. Open a Pull Request

## Development Guidelines

### Coding Standards

This project follows the Laravel coding standards:

- Use **Laravel Pint** for code formatting
- Follow **PSR-12** coding style
- Use **type hints** for parameters and return types
- Write **clear, descriptive** variable and method names

### Running Pint

Format your code before committing:

```bash
composer format
# or
./vendor/bin/pint
```

### Code Style Examples

**Good:**
```php
public function quickAdd(bool $enabled = true, ?string $label = null): static
{
    if (! $enabled) {
        return $this;
    }

    // Clear, readable code
}
```

**Avoid:**
```php
public function quickAdd($enabled = true, $label = null) // Missing types
{
    if(!$enabled) return $this; // Poor formatting
}
```

### Translation Contributions

Adding new languages is highly appreciated!

1. Create a new directory in `lang/{locale}/`
2. Copy `lang/en/quick-add.php`
3. Translate the strings
4. Submit a pull request

Example for Dutch:
```php
// lang/nl/quick-add.php
<?php

return [
    'add' => '+ Toevoegen ":term"',
];
```

### Testing

While this plugin doesn't have automated tests yet, please:

- Test your changes manually in a Filament application
- Test with both single and multiple selects
- Test in light and dark modes
- Verify translations work correctly

### Documentation

- Update the README.md if you add new features
- Add code examples for new functionality
- Keep documentation clear and concise
- Use proper grammar and spelling

## Pull Request Process

1. **Update documentation** - Ensure README reflects any changes
2. **Update CHANGELOG** - Add your changes under "Unreleased"
3. **Test thoroughly** - Manually test all affected functionality
4. **Format code** - Run Pint before committing
5. **Clear description** - Explain what and why in your PR description
6. **Link issues** - Reference any related issues

### PR Title Format

Use clear, descriptive titles:
- `feat: Add support for custom icon`
- `fix: Resolve issue with multiple selects`
- `docs: Update installation instructions`
- `refactor: Simplify label generation logic`

## Code of Conduct

### Our Standards

- **Be respectful** - Treat everyone with respect
- **Be welcoming** - Welcome newcomers and encourage contributions
- **Be constructive** - Provide constructive feedback
- **Be patient** - Everyone has different experience levels

### Unacceptable Behavior

- Harassment or discriminatory language
- Trolling or insulting comments
- Personal or political attacks
- Publishing others' private information

## Questions?

- **Discord** - Ask in the Filament Discord #quick-add-select channel (after plugin approval)
- **GitHub Issues** - Open an issue for technical questions
- **Twitter** - Reach out to [@cocoricosmos](https://twitter.com/cocoricosmos)

## Recognition

All contributors will be recognized in the README.md file.

Thank you for contributing to Filament Quick Add Select! 🎉
