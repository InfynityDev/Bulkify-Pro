# Bulkify Pro by Infynity.Dev — Transform Products into Wholesale Power Pages

Bulkify Pro is a professional WordPress/WooCommerce plugin designed to transform selected WooCommerce products into fully interactive wholesale or service-order pages. The plugin replaces standard "Add to Cart" functionality with customizable WhatsApp contact buttons, custom contact buttons, itemized pricing tables, quantity controls, and bulk discount tables — perfect for B2B stores, wholesale businesses, and service providers who prefer direct contact over traditional e-commerce checkout.

**Plugin Type:** WooCommerce Extension  
**Version:** 1.0.0  
**Author:** Infynity.Dev  
**Text Domain:** bulkify-pro  
**Slug:** bulkify-pro

---

## Table of Contents

1. [Overview](#overview)
2. [Key Features](#key-features)
3. [System Requirements](#system-requirements)
4. [Installation](#installation)
5. [Quick Start](#quick-start)
6. [Admin Interface & Navigation](#admin-interface--navigation)
7. [Configuration & Settings](#configuration--settings)
8. [Usage Examples & Workflows](#usage-examples--workflows)
9. [Shortcodes](#shortcodes)
10. [Hooks](#hooks)
11. [Advanced Technical Details](#advanced-technical-details)

---

## Overview

Bulkify Pro enables WooCommerce store owners to convert any product page into a custom contact-driven sales page. Instead of traditional e-commerce checkout, customers interact with WhatsApp buttons, custom contact buttons, or bulk discount tables that encourage direct communication for quotes and orders.

The plugin is ideal for:
- **Wholesale businesses** that require custom pricing based on quantity
- **B2B stores** that prefer direct contact over automated checkout
- **Service providers** offering customized quotes
- **Multi-vendor platforms** where each vendor needs unique contact methods

Key capabilities include:
- Replace "Add to Cart" with WhatsApp or custom contact buttons
- Display customizable pricing information with unit labels
- Create tiered bulk discount tables with quantity-based pricing
- Support for multiple languages and RTL (Right-to-Left) layouts
- Extensive customization options for colors, fonts, and appearance
- Product-level customization that overrides global settings


---

## Key Features

- **WhatsApp Integration** — Direct WhatsApp contact buttons with customizable message templates
- **Custom Contact Buttons** — Create custom buttons linking to contact forms, phone calls, or other URLs
- **Bulk Discount Tables** — Display tiered pricing tables with quantity breaks and savings calculations
- **Custom Pricing Display** — Override WooCommerce prices with custom text, starting prices, and unit labels
- **Multi-language Support** — WPML and Polylang compatible with RTL language support (Arabic, Hebrew, etc.)
- **Extensive Customization** — 11 color schemes plus custom color options, font size controls, and appearance settings
- **Product-Level Control** — Per-product settings that override global defaults
- **Shortcodes** — Embed WhatsApp buttons, custom buttons, and bulk discounts anywhere
- **License Management** — Built-in license validation system for support and updates
- **Performance Optimized** — Caching system and optimized asset loading
- **HPOS Compatible** — Compatible with WooCommerce High-Performance Order Storage

---

## System Requirements

| Requirement | Minimum | Recommended |
|-------------|---------|-------------|
| PHP | 8.0 | 8.1+ |
| WordPress | 6.0 | Latest |
| WooCommerce | 8.0 | Latest (10.3.3+) |
| MySQL | 5.6 | 5.7+ |

**Additional Notes:**
- **Multisite:** Compatible with WordPress Multisite installations
- **RTL Support:** Fully supports RTL languages (Arabic, Hebrew, Farsi, Urdu)
- **Translation Ready:** Includes `.pot` file for translations
- **HPOS Compatible:** Declares compatibility with WooCommerce High-Performance Order Storage

---

## Installation

### Standard Installation

1. **Download the Plugin**
   - Download the plugin ZIP file from your purchase location

2. **Upload via WordPress Admin**
   - Navigate to `Plugins → Add New → Upload Plugin`
   - Select the ZIP file
   - Click `Install Now`
   - Activate the plugin

3. **Verify WooCommerce**
   - Ensure WooCommerce is installed and activated
   - The plugin will display a notice if WooCommerce is missing


### Manual Installation (FTP)

1. Extract the plugin ZIP file
2. Upload the `bulkify-pro` folder to `/wp-content/plugins/`
3. Activate the plugin from `Plugins → Installed Plugins`

---

## Quick Start

1. **Access Settings**
   - Navigate to `WooCommerce → Bulkify Pro` in the WordPress admin menu

2. **Configure Default WhatsApp Number**
   - Go to `General Settings` tab
   - Enter your WhatsApp number in international format (e.g., `905xxxxxxxxx`)
   - Save settings

3. **Enable on a Product**
   - Edit any WooCommerce product
   - Scroll to the `Bulkify Pro` meta box
   - Enable WhatsApp button or bulk discounts
   - Configure product-specific settings (optional)
   - Save/update the product

4. **View Result**
   - Visit the product page on the frontend
   - The "Add to Cart" button will be replaced with your configured buttons
   - Custom pricing and bulk discounts will display automatically


---

## Admin Interface & Navigation

### Main Menu

**Location:** `WooCommerce → Bulkify Pro`

The settings page is accessible to users with `manage_woocommerce` capability.

### Settings Page Tabs

The settings page includes five main tabs:

1. **General Settings** — Core functionality and default WhatsApp configuration
2. **Appearance** — Color schemes, font sizes, and display settings
3. **Text Settings** — Button labels, message templates, and localization strings
4. **Advanced** — Performance and caching settings
5. **License** — License key activation and validation

### Product Meta Box

**Location:** Product Edit Screen (`Products → Edit Product`)

The `Bulkify Pro` meta box appears on all WooCommerce product edit screens and includes five tabs:

1. **WhatsApp Button** — Product-specific WhatsApp settings
2. **Custom Button** — Product-specific custom button configuration
3. **Pricing** — Custom pricing display settings
4. **Bulk Discounts** — Tiered pricing table configuration
5. **Shortcodes** — Ready-to-use shortcodes for embedding elements


---

## Configuration & Settings

### General Settings

| Setting Key | Label | Type | Default | Description |
|-------------|-------|------|---------|-------------|
| `default_whatsapp_number` | Default WhatsApp Number | Text | Empty | International format without + sign (e.g., 905xxxxxxxxx) |
| `unit_position` | Unit Position | Select | `after` | Position of unit label relative to price (`after`, `before`, `newline`) |
| `unit_separator` | Unit Separator | Text | ` / ` | Text between price and unit label |
| `animations` | Animations | Checkbox | `true` | Enable smooth animations and transitions |
| `responsive_design` | Responsive Design | Checkbox | `true` | Enable responsive design for mobile devices |

### Appearance Settings

| Setting Key | Label | Type | Default | Description |
|-------------|-------|------|---------|-------------|
| `color_scheme` | Color Scheme | Select | `modern` | Pre-defined color scheme (`theme`, `modern`, `whatsapp`, `minimal`, `vibrant`, `ocean`, `sunset`, `forest`, `royal`, `elegant`, `custom`) |
| `product_page_font_size` | Product Pages Font Size | Select | `inherit` | Font size for product pages (`inherit`, `small`, `medium`, `large`, `xlarge`, `custom`) |
| `custom_product_font_size` | Custom Font Size (px) | Number | `14` | Custom font size in pixels (8-48) |
| `widget_font_size` | Other Pages & Widgets Font Size | Select | `inherit` | Font size for shop/category pages |
| `custom_font_size` | Custom Font Size (px) | Number | `14` | Custom font size in pixels (8-48) |
| `single_product_font_size` | Custom CSS Font Size | Text | Empty | Override with custom CSS values (e.g., `1.05rem`, `18px`) |
| `show_unit_label_outside_product` | Show Unit Label | Checkbox | `false` | Display unit label on shop/category pages |
| `show_price_text_outside_product` | Show Price Text | Checkbox | `true` | Display custom price text outside product pages |
| `show_starting_price_outside_product` | Show Starting Price | Checkbox | `true` | Display starting price outside product pages |

### Custom Colors (when `color_scheme` is `custom`)

| Setting Key | Label | Type | Default | Description |
|-------------|-------|------|---------|-------------|
| `primary_color` | Primary Color | Color | `#6366f1` | Main brand color |
| `primary_dark` | Primary Dark | Color | `#4f46e5` | Hover state color |
| `accent_color` | Accent Color | Color | `#8b5cf6` | Secondary accent color |
| `button_background` | Button Background | Color | `#25D366` | WhatsApp button background |
| `button_hover` | Button Hover | Color | `#128C7E` | Button hover state |
| `button_text_color` | Button Text Color | Color | `#ffffff` | Button text color |
| `card_background` | Card Background | Color | `#ffffff` | Background of discount cards |
| `card_border` | Card Border | Color | `#e2e8f0` | Border color of cards |
| `card_shadow` | Card Shadow | Color | `#6366f1` | Shadow color for cards |
| `title_text` | Title Text | Color | `#1e293b` | Title and heading text |
| `label_text` | Label Text | Color | `#1e293b` | Label and description text |
| `quantity_text` | Quantity Text | Color | `#6366f1` | Quantity display text |
| `price_text` | Price Text | Color | `#059669` | Price display text |
| `secondary_text` | Secondary Text | Color | `#64748b` | Secondary and muted text |
| `link_color` | Link Color | Color | `#6366f1` | Link and clickable text |
| `badge_background` | Badge Background | Color | `#eef2ff` | Badge background color |
| `badge_text` | Badge Text | Color | `#4338ca` | Badge text color |
| `badge_border` | Badge Border | Color | `#c7d2fe` | Badge border color |
| `discount_background` | Discount Background | Color | `#6366f1` | Discount badge background |
| `discount_text` | Discount Text | Color | `#ffffff` | Discount badge text |
| `separator_color` | Separator Color | Color | `#f1f5f9` | Line separator color |
| `divider_color` | Divider Color | Color | `#e2e8f0` | Section divider color |

### Text Settings (Localization)

| Setting Key | Label | Type | Default | Description |
|-------------|-------|------|---------|-------------|
| `button_text` | Button Text | Text | `Chat on WhatsApp` | WhatsApp button label |
| `template` | Message Template | Textarea | `Hello, I'd like to inquire about: {title} (ID: {id}{sku_opt}) — Here is the link: {url} | From {site}` | WhatsApp message template with variables |
| `price_prefix` | Price Prefix | Text | `Starting from` | Text displayed before price |
| `unit_label` | Unit Label | Text | Empty | Default unit label (e.g., `per item`) |
| `bulk_title` | Table Title | Text | `Bulk Savings (buy more, save more)` | Bulk discount table title |
| `bulk_unit_price_label` | Unit Price Label | Text | Empty | Label for unit price (`Each:`) |
| `bulk_regular_price_label` | Regular Price Label | Text | Empty | Label for regular price |
| `bulk_total_price_label` | Total Price Label | Text | Empty | Label for total price |
| `bulk_save_label` | Save Label | Text | Empty | Label for savings amount |
| `bulk_savings_percentage_label` | Savings Percentage Label | Text | Empty | Label for savings percentage |
| `bulk_best_value_text` | Best Value Badge Text | Text | Empty | Text for "Best Value" badge |
| `bulk_discount_off_label` | Discount "OFF" Label | Text | Empty | Label for discount percentage |
| `bulk_default_label_template` | Default Label Template | Text | Empty | Template for bulk tier labels (use `{qty}` placeholder) |
| `bulk_whatsapp_button_text_template` | Button Text Template | Text | Empty | Template for WhatsApp button text in bulk table (use `{qty}` placeholder) |
| `bulk_whatsapp_message_template` | Message Template | Textarea | Empty | Template for WhatsApp message from bulk table (placeholders: `{qty}`, `{product_name}`, `{total_price}`, `{unit_price}`, `{product_url}`) |

### Custom Button Settings

| Setting Key | Label | Type | Default | Description |
|-------------|-------|------|---------|-------------|
| `custom_button_text` | Button Text | Text | `Contact Us` | Default custom button text |
| `custom_button_url` | Button URL | URL | Empty | Default custom button URL |
| `custom_button_color` | Button Color | Color | `#007cba` | Default button background color |
| `custom_button_text_color` | Button Text Color | Color | `#ffffff` | Default button text color |
| `custom_button_icon_svg` | Button Icon | Media | Empty | SVG icon URL from Media Library |

### Bulk Discounts Display Options

| Setting Key | Label | Type | Default | Description |
|-------------|-------|------|---------|-------------|
| `bulk_show_unit_price` | Show Unit Price | Checkbox | `true` | Display unit price in bulk table |
| `bulk_show_regular_price` | Show Regular Price | Checkbox | `true` | Display regular price in bulk table |
| `bulk_show_total_savings` | Show Total Savings | Checkbox | `true` | Display total savings amount |
| `bulk_show_savings_percentage` | Show Savings Percentage | Checkbox | `true` | Display savings percentage |
| `bulk_show_whatsapp_button` | Show WhatsApp Button | Checkbox | `true` | Show WhatsApp button for each tier |

### Advanced Settings

| Setting Key | Label | Type | Default | Description |
|-------------|-------|------|---------|-------------|
| `enable_caching` | Enable Caching | Checkbox | `true` (disabled) | Caching is always enabled for performance |

### License Settings

| Setting Key | Label | Type | Default | Description |
|-------------|-------|------|---------|-------------|
| `bulkify_purchase_code` | Purchase Code | Text | Empty | CodeCanyon purchase code for license activation |
| `bulkify_license_status` | License Status | Select | `invalid` | License validation status (`valid`, `invalid`, `pending`) |


---

## Usage Examples & Workflows

### Workflow 1: Enable WhatsApp Contact for a Product

**Goal:** Convert a product page to use WhatsApp contact instead of "Add to Cart"

**Steps:**
1. Navigate to `WooCommerce → Bulkify Pro`
2. In the `General Settings` tab, enter your default WhatsApp number (e.g., `905551234567`)
3. Customize the `Message Template` in the `Text Settings` tab if needed
4. Save settings
5. Edit a product (`Products → Edit Product`)
6. In the `Bulkify Pro` meta box, go to the `WhatsApp Button` tab
7. Enable the "Enable WhatsApp Contact" toggle
8. Optionally override the WhatsApp number or message template for this product
9. Save/update the product
10. Visit the product page on the frontend

**Expected Result:**
- The "Add to Cart" button is replaced with a WhatsApp button
- Clicking the button opens WhatsApp with a pre-filled message containing product details
- Custom pricing display replaces standard WooCommerce price if configured

### Workflow 2: Create a Bulk Discount Table

**Goal:** Display tiered pricing with quantity breaks

**Steps:**
1. Edit a product (`Products → Edit Product`)
2. Navigate to the `Bulk Discounts` tab in the `Bulkify Pro` meta box
3. Enable "Enable Bulk Discounts"
4. Click "Add Bulk Tier" to create discount tiers
5. For each tier, configure:
   - **Quantity:** Minimum quantity for this tier
   - **Discount Type:** Percentage or flat amount
   - **Discount Value:** Discount amount (e.g., `10` for 10% or $10 flat)
   - **Label:** Optional custom label (e.g., "Buy 10+ items")
6. The plugin automatically calculates:
   - Unit price after discount
   - Total price for the quantity
   - Total savings amount
   - Savings percentage
7. Save/update the product

**Expected Result:**
- A styled bulk discount table appears on the product page
- Each tier shows quantity, unit price, total price, and savings
- The tier with the highest discount is marked as "Best Value"
- WhatsApp buttons are available for each tier (if enabled)

### Workflow 3: Customize Appearance with Color Schemes

**Goal:** Match the plugin appearance to your store's branding

**Steps:**
1. Navigate to `WooCommerce → Bulkify Pro → Appearance`
2. Select a pre-defined color scheme from the dropdown:
   - `Theme Default` — Inherits theme colors
   - `Modern` — Modern indigo/purple theme
   - `WhatsApp Style` — WhatsApp green theme
   - `Minimal` — Clean, minimal design
   - `Vibrant` — Bold gradient colors
   - `Ocean Blue`, `Sunset Orange`, `Forest Green`, `Royal Purple`, `Elegant Dark` — Themed color schemes
   - `Custom` — Use custom colors
3. If selecting `Custom`, configure individual colors:
   - Primary colors (Primary, Primary Dark, Accent)
   - Button colors (Background, Hover, Text)
   - Card colors (Background, Border, Shadow)
   - Text colors (Title, Label, Quantity, Price, Secondary, Link)
   - Badge & discount colors
   - Separator colors
4. Adjust font sizes if needed
5. Save settings

**Expected Result:**
- All Bulkify Pro elements match your selected color scheme
- Changes apply immediately to all product pages
- Custom colors override default theme colors

### Workflow 4: Multi-language Setup with WPML

**Goal:** Configure different WhatsApp messages for different languages

**Steps:**
1. Ensure WPML is installed and activated
2. Navigate to `WooCommerce → Bulkify Pro → Text Settings`
3. The plugin automatically detects the current language
4. Configure text settings for each language:
   - Switch languages in WPML language switcher
   - Enter language-specific button text and templates
   - Save settings
5. On product pages, the plugin uses the appropriate language settings based on WPML's language detection

**Expected Result:**
- WhatsApp messages and button labels display in the correct language
- RTL languages (Arabic, Hebrew) automatically use RTL layout
- Product-specific settings can override language-specific defaults


---

## Shortcodes

Bulkify Pro provides shortcodes for embedding WhatsApp buttons, custom buttons, and bulk discount tables anywhere in your content.

### WhatsApp Button Shortcode

**Shortcode:** `[bulkify_whatsapp_button]` or `[bulkify_whatsapp]`

**Attributes:**
- `product_id` (optional) — Product ID. If omitted, uses current product context.

**Usage Examples:**
```
[bulkify_whatsapp_button]
[bulkify_whatsapp product_id="123"]
```

**Description:** Displays a WhatsApp contact button. Only renders if WhatsApp is enabled for the specified product.

### Custom Button Shortcode

**Shortcode:** `[bulkify_custom_button]` or `[bulkify_custom]`

**Attributes:**
- `product_id` (optional) — Product ID. If omitted, uses current product context.

**Usage Examples:**
```
[bulkify_custom_button]
[bulkify_custom product_id="123"]
```

**Description:** Displays a custom contact button. Only renders if custom button is enabled for the specified product.

### Bulk Discounts Shortcode

**Shortcode:** `[bulkify_bulk_discounts]` or `[bulkify_bulk]`

**Attributes:**
- `product_id` (optional) — Product ID. If omitted, uses current product context.

**Usage Examples:**
```
[bulkify_bulk_discounts]
[bulkify_bulk product_id="123"]
```

**Description:** Displays the bulk discount table. Only renders if bulk discounts are enabled for the specified product.

### Shortcode Usage in Product Content

Shortcodes can be embedded directly in product descriptions or short descriptions. If a shortcode is used in product content, the automatic rendering is disabled for that element to prevent duplicates.

**Example:**
Add `[bulkify_whatsapp_button]` in the product description to position the button exactly where you want it.

---

## Hooks

Bulkify Pro provides WordPress hooks (actions and filters) for developers to extend functionality.

### Actions

| Hook | When it runs | Parameters | Purpose |
|------|--------------|------------|---------|
| `bulkify_plugin_initialized` | After plugin initialization | `$plugin` (Plugin instance) | Allows other plugins to hook into plugin initialization |
| `bulkify_activated` | On plugin activation | None | Fired when plugin is activated |
| `bulkify_deactivated` | On plugin deactivation | None | Fired when plugin is deactivated |
| `bulkify_styles_refreshed` | After dynamic styles are refreshed | None | Allows clearing external caches when styles change |

### Filters

| Hook | Purpose | Parameters | Return value |
|------|---------|------------|--------------|
| `bulkify_button_wrapper` | Modify WhatsApp button wrapper HTML | `$wrapper_html` (string), `$button_html` (string), `$product` (WC_Product) | Modified wrapper HTML |
| `bulkify_button_html` | Modify WhatsApp button HTML | `$button_html` (string), `$product` (WC_Product) | Modified button HTML |
| `bulkify_custom_button_wrapper` | Modify custom button wrapper HTML | `$wrapper_html` (string), `$button_html` (string), `$product` (WC_Product) | Modified wrapper HTML |
| `bulkify_custom_button_html` | Modify custom button HTML | `$button_html` (string), `$product` (WC_Product) | Modified button HTML |
| `plugin_locale` | Override plugin locale | `$locale` (string), `$domain` (string) | Modified locale string |

### WooCommerce Hooks Used

The plugin hooks into the following WooCommerce actions and filters:

**Actions:**
- `woocommerce_single_product_summary` — Removes default "Add to Cart" and renders custom buttons/bulk discounts
- `before_woocommerce_init` — Declares HPOS compatibility

**Filters:**
- `woocommerce_get_price_html` — Modifies price display on product pages
- `woocommerce_is_purchasable` — Disables purchase capability when Bulkify features are enabled

### Example Usage

**Modify WhatsApp Button HTML:**
```php
add_filter('bulkify_button_html', function($button_html, $product) {
    // Add custom class
    $button_html = str_replace('class="bulkify-button"', 'class="bulkify-button my-custom-class"', $button_html);
    return $button_html;
}, 10, 2);
```

**Hook into Plugin Initialization:**
```php
add_action('bulkify_plugin_initialized', function($plugin) {
    // Your custom code here
});
```

---

## Advanced Technical Details

### Multi-language Support

- **WPML Integration** — Automatically detects current language via `wpml_current_language` filter
- **Polylang Integration** — Uses `pll_current_language()` function
- **Language-Specific Settings** — Separate settings groups for Arabic (`bulkify_ar_settings`) and English (`bulkify_en_settings`)
- **RTL Detection** — Automatically detects RTL languages (Arabic, Hebrew, Farsi, Urdu) and applies RTL layout
- **Translation Ready** — Includes `.pot` file for translations

---

## Support & Resources

Support: https://infynity.dev/contact-us/

Documentation: https://github.com/InfynityDev/Bulkify-Pro

Purchase: https://infynity.dev/bulkify-pro/

Author Website: https://infynity.dev



Documentation generated © 2025 Bulkify Pro by Infynity.Dev. All rights reserved.

Last Updated: 2025

