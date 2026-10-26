# Qlik Thumbnail Generator

A single HTML file that makes clean, consistent thumbnails for Qlik Sense apps, sheets and stories, in the 8:5 aspect ratio that Qlik Sense expects. Works with Qlik Cloud and Qlik Sense Client-Managed.

Nothing to install, no account, no server. Everything runs in your browser and nothing you type leaves the page.

## Use it

**Open the live page: [kirilkirin.github.io/qlik-thumbnail-generator](https://kirilkirin.github.io/qlik-thumbnail-generator/)**

That is all most people need. The page is always the current version.

### Or keep a local copy

If you prefer a file on your own computer:

1. Open [`index.html`](https://github.com/kirilkirin/qlik-thumbnail-generator/blob/main/index.html) in this repository.
2. Click the **download** icon (next to the **Raw** button, top right of the file view) and save the file anywhere.
3. Double-click the saved file. It opens in your browser.

Clicking **Raw** shows the code as text, not the tool. If you land there, save the page with `Ctrl+S` (Windows) or `Cmd+S` (Mac) and open the saved file.

## Make a thumbnail

1. **Text** — type a title and, if you want, a second line. Long titles wrap and shrink to fit.
2. **Layout** — choose icon left and text right, icon above text, icon only, or text only.
3. **Colors** — pick a background and a foreground color, or click one of the Qlik palette presets. The swap button flips the two.
4. **Icon** — click **Change icon**. Browse by category, or search by name or meaning (for example `cash`, `delivery`, `forecast`). Click an icon to use it. Adjust its size and line weight with the sliders.
5. **Size and format** — choose an output size from 640 × 400 to 2560 × 1600 pixels, and PNG (Portable Network Graphics) or JPG (Joint Photographic Experts Group).
6. Click **Download**. The file is named after your title, for example `sales-dashboard-1280x800.png`.

## Use it in Qlik Sense

- **App thumbnail** — open the app details, click **Edit details**, click the thumbnail, and upload the image to the media library. You can only change the thumbnail of an unpublished app.
- **Sheet thumbnail** — in the app overview, edit the sheet and click its thumbnail to choose an image from the media library. You can only change the thumbnail of a private (unpublished) sheet.
- **Story thumbnail** — same as a sheet, from the stories view.

On Qlik Sense Client-Managed, images for the **Default** media folder are uploaded through the Qlik Management Console (QMC) content libraries. The **In app** folder accepts uploads from inside the app.

## Requirements

- A current browser: Chrome, Edge, Firefox or Safari.
- An internet connection when you open the page. The tool loads the icon library, icon categories and search tags from Lucide, and the Inter font from Google Fonts. If the icon library cannot load, text-only thumbnails still work.

The tool makes no other network requests. Titles, colors and downloads stay on your computer.

## Icons

Icons come from [Lucide](https://lucide.dev), an open-source icon set released under the ISC license. The tool always uses the latest Lucide 1.x release:

- Icon shapes load from the `lucide` package on a content delivery network (jsDelivr, with unpkg as a backup).
- Icon categories, category names and search tags load live from lucide.dev and Lucide's repository, so new icons and categories appear automatically.

Lucide does not include brand logos. For a Qlik-branded or company-specific icon, use the text-only layout for now, or open an issue to discuss adding custom icon support.

## Version history

| Version | Changes |
|---|---|
| v4 | Icon picker grouped by Lucide's categories, with a category list on the left. Library and metadata track the latest Lucide 1.x release. |
| v3 | Icon picker moved into a dialog. Search by name or meaning (Lucide tags). Wider settings panel. |
| v2 | Settings panel scrolls on its own; size and format moved under the preview. |
| v1 | First release: four layouts, color presets, icon search, PNG and JPG download. |

## Credits

- Icons, categories and search tags: [Lucide](https://lucide.dev) — ISC license.
- Typeface: [Inter](https://rsms.me/inter/) — SIL Open Font License.
