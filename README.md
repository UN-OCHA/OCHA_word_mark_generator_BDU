# OCHA Wordmark Generator

Creates branded wordmarks using UN OCHA Humanitarian Icons organized by category.

## Files

- **icon-curator.html** - Curate icons by category and configure vertical adjustments
- **ocha-wordmark-generator.html** - Main wordmark generator
- **Humanitarian_icons_2026.csv** - Category definitions from your Excel file (required)
- **curated-icons.json** - (Generated) Your curated icon list with settings

## Quick Start

### 1. Curate Icons

1. Open `icon-curator.html`
2. Icons are auto-organized into 19 categories from your Excel:
   - Clusters
   - Disasters, hazards and crises
   - People
   - Activities Strategy
   - Health
   - Logistics
   - UX UI
   - ...and 12 more

3. For each category:
   - Click category header to collapse/expand
   - Use "All" checkbox to select/deselect entire category
   - Edit category names if needed
   - Delete categories (icons move to "Uncategorized")

4. For each icon:
   - Check/uncheck to include in wordmark generator
   - Set vertical adjustment (-20 to +20 px) for balance
   - Move icons between categories using dropdown

5. Click **Export JSON** → saves `curated-icons.json`

### 2. Generate Wordmarks

1. Place `curated-icons.json` in same folder as generator
2. Open `ocha-wordmark-generator.html`
3. Icons appear organized by category
4. Select icon → type text → preview updates
5. Download SVG or PNG

## Category Management

**Add Category**: Creates new empty category

**Expand/Collapse All**: Show/hide all category contents

**Select All (per category)**: Check header checkbox to include/exclude entire category

**Delete Category**: Removes category, icons move to "Uncategorized"

**Rename Category**: Click category name to edit

**Move Icons**: Use dropdown on each icon card to change category

## Icon Settings

**Include checkbox**: Add to curated list

**V.Adj (Vertical Adjustment)**:
- Negative values = move up
- Positive values = move down
- 0 = centered (default)
- Range: -20 to +20 pixels

**Category dropdown**: Reassign icon to different category

## Auto-Categorization

Icons are automatically categorized by loading `Humanitarian_icons_2026.csv`:
- Exact category mappings from your Excel file
- 386 icons pre-categorized into 19 families
- Icons not in CSV go to "Uncategorized"
- You can manually adjust any categorization
- **Important**: Keep the CSV file in the same folder as the curator

## Import/Export

**Export**: Saves categories + selected icons with adjustments

**Import**: Load previously exported JSON to continue editing

## Generator Features

- **Icon box**: 48×48px square, right-aligned, vertically centered
- **Font**: Roboto Bold, 36px black
- **Icon color**: UN Blue (#009edb)
- **Spacing**: 12px between icon and text
- **Layout**: Icon left, text right
- **Export**: SVG (vector) + PNG (2× resolution)

## Tips

- Start with all 19 categories pre-loaded from your Excel
- Deselect entire categories you don't need for logos
- Test icons in generator before setting vertical adjustments
- Keep adjustments subtle (±4 to ±6px usually enough)
- Re-export JSON anytime you make changes

## Categories from Your Excel

19 categories with 386 icons total:
- **UX UI** (63 icons) - Interface elements
- **Activities Strategy** (35 icons) - Program activities
- **Disasters, hazards and crises** (32 icons)
- **Damage** (30 icons) - Facility damage states
- **General infrastructure** (27 icons)
- **Food and non-food items** (26 icons)
- **People** (26 icons) - Demographics
- **Health** (20 icons)
- **Logistics** (17 icons)
- **Security and incident** (16 icons)
- **Telecommunications and technology** (14 icons)
- **Water sanitation and hygiene** (13 icons)
- **Clusters** (11 icons)
- **Others** (11 icons)
- **Product type** (11 icons) - Document types
- **Socioeconomic and development** (10 icons)
- **Lockdown** (10 icons)
- **Physical barriers** (8 icons)
- **Camp** (6 icons)

Plus **Uncategorized** for any additional icons from the repository.
