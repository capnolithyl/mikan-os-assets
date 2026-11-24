# MikanOS · Candlelight

A cozy cocoa-and-amber Windows 11 theme collection, with matching browser, editor and terminal themes, glowing paw-print icons and stardust artwork.

## v1.0 — November 24, 2026

The curated restore kit is named **MikanOS-Candlelight-v1.0.zip**. The archive was prepared and validated in ChatGPT; uploading the binary ZIP to this repository is still pending. Its SHA-256 is:

~~~text
a3418b7ca0a4b5e9c745a0550160ee961979e25407b18c61aa982d7a6ff762ad
~~~

| Component | Preset |
| --- | --- |
| ChatGPT | Stylus CSS v1.12 |
| Vivaldi | Native theme ZIP and custom UI CSS |
| VS Code | Mikan Cocoa Glow v1.1.0 VSIX and glow CSS v1.2 |
| Taskbar | Working sparkle preset |
| Start menu | Native-hover preset |
| File Explorer | Styler v1.1, optional GPU XML |
| Notification Center | v1.6, opaque v1.4 fallback |
| System icons | Resource Redirect v2.2 |
| File types | Audio, code, PDF INI |
| Windows Terminal | Candlelight scheme/theme and PowerShell prompt |
| Lock screen | Ultrawide rainy-night cat wallpaper |

## Restoration

1. Extract the restore kit. Copy the contents of its Assets directory into C:\Vivaldi\Mikan. Preserve filenames.
2. Use dark Windows mode and manual accent #FFAD5C. Enable accent on title bars and window borders; leave Start/taskbar accent off. Set Wallpapers/rainy_night_cat_library_nook.png as the lock-screen picture.
3. ChatGPT: install Stylus, disable Stylish, import ChatGPT/mikan-chatgpt-v1.12.css, scoped to chatgpt.com.
4. Vivaldi: import the theme ZIP through Settings > Themes. Enable custom UI CSS if needed, set the CSS directory in Appearance settings, restart.
5. VS Code: install the VSIX, select Mikan Cocoa Glow, optionally configure Custom CSS and JS Loader with file:///C:/Vivaldi/Mikan/mikan-vscode-glow.css (copy the v1.2 CSS there). Merge the provided color override with user settings. The loader modifies VS Code installation files and may need reapplying after updates.
6. Windhawk: back up existing settings first, then import each matching JSON in Advanced > Mod settings. Use the working taskbar preset, native-hover Start Menu preset (with StartAllBack disabled), File Explorer Styler v1.1, and Notification Center Styler v1.6. Use notification v1.4 if the hosted image fails.
7. Optional GPU-accelerated Explorer view: use the supplied custom XML. Drag-and-drop failed with this mod enabled on the original PC; switch to native view or disable the mod if necessary. Explorer TreeItem Tweaker can enlarge sidebar icons (suggested 24 px icons / 38 px rows, or 32 / 44; exact live values not exported).
8. Resource Redirect: extract the icon pack into C:\Vivaldi\Mikan, select no built-in theme, set the theme path to C:\Vivaldi\Mikan\Mikan-Resource-Redirect-v2.2. Leave experimental redirect-all disabled initially. Refresh icon cache. Do not copy resource DLLs into System32. For File Type Properties Customization, enable Load INI preset and select file-types.ini in that same directory. Audio and JSON worked; PDF thumbnails may override icons.
9. Terminal: merge the provided settings fragment at the root of existing settings, preserving other profiles and schemes. Review the optional prompt script, copy it to C:\Vivaldi\Mikan and dot-source from the PowerShell profile if desired. Do not globally weaken execution policy.

The complete archive also contains a more detailed README and a per-file SHA256SUMS.txt manifest.

## Hosted artwork

Keep [mikan-notification-stardust-v13.png](mikan-notification-stardust-v13.png) at the repository root: the notification preset references its raw GitHub URL. Moving or renaming it breaks the existing theme.

## Scope and known limitations

This is a backup of generated theme assets, not an export of the live PC. Personal screenshots, browser exports, credentials, full live Terminal profiles, cursor experiments and system sounds are excluded. Manual settings changes and installed mod versions may need separate private backups. Root Desktop, connected phone and Google Drive retain native icons. The GPU Explorer drag-and-drop issue remains unresolved.

Apply components individually and retain the previous settings for rollback. No Windows system file replacement is necessary.
