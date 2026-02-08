# Special Treats For Christmas

Email template for promoting special treats and discounts during the Christmas season, applicable to retail and hospitality industries.

![Thumbnail](./thumbnail.png)

## Template Details

- **Industries:** Hospitality, Retail
- **Message Type:** Marketing
- **Tags:** christmas special offers, holiday promotion

## Files
- `index.html`: The improved, localized, and branded HTML template.
- `template.blade.php`: Ready-to-use Laravel Blade template with `asset()` helpers.
- `assets/`: Directory containing localized images and styles used in the template.

## Usage in Laravel

### 1. Store the Template
Place the `index.html` content in a Blade view (e.g., `resources/views/emails/special-treats-for-christmas.blade.php`).

### 2. Handle Assets
Move the content of `assets/` to your public directory (e.g., `public/vendor/mail-templates/special-treats-for-christmas/`) and update the paths in the HTML to use the `asset()` helper.

### 3. Send Email
```php
Mail::to($user)->send(new \App\Mail\GenericEmail([
    'view' => 'emails.special-treats-for-christmas',
    'data' => [
        // Your dynamic data here
    ]
]));
```

---
*Created with ❤️ by **[LaravelMail.com](https://laravelmail.com)** - Your source for professional email templates.*
