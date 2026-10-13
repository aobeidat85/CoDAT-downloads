# CoDAT for IntelliJ IDEA

CoDAT (Code Documentation and Analysis Tool) adds structured Java comments, comment navigation, AI analysis, and method sketch and specification generation to IntelliJ IDEA.

This repository contains the installable plugin ZIP. Source code is maintained separately.

## Download

[Download CoDATv2-latest.zip](https://github.com/aobeidat85/CoDAT-downloads/raw/refs/heads/main/CoDATv2-latest.zip)

You can also open `CoDATv2-latest.zip` in this repository and click **Download raw file**. Keep the ZIP intact; do not extract it before installation.

## Install in IntelliJ IDEA

1. Download `CoDATv2-latest.zip` using the link above.
2. Open IntelliJ IDEA's **Settings**:
   - Windows or Linux: **File > Settings**.
   - macOS: **IntelliJ IDEA > Settings**.
3. Select **Plugins**.
4. Click the **gear icon** and choose **Install Plugin from Disk...**.
5. Select the downloaded `CoDATv2-latest.zip` and confirm installation.
6. Restart IntelliJ IDEA if prompted.
7. Open a Java project and search Settings for **CoDAT Plugin Settings**.

See the [official JetBrains plugin installation instructions](https://www.jetbrains.com/help/idea/managing-plugins.html#install_plugin_from_disk) for more details.

## Supported IntelliJ IDEA versions

CoDAT declares a minimum IntelliJ IDEA version of **2024.1** (platform build **241**). Java language support must be enabled. Versions older than 2024.1 are not supported.

The recorded binary compatibility verification from **September 23, 2026** covered the following IDE distributions:

| IntelliJ IDEA version | Distribution checked | Exact build |
| --- | --- | --- |
| 2024.1 | Community | 241.14494.240 |
| 2024.2 | Community | 242.20224.300 |
| 2024.3 | Community | 243.21565.193 |
| 2025.1.4.1 | Community | 251.27812.49 |
| 2025.2 | Community | 252.23892.409 |
| 2025.3 | Unified IntelliJ IDEA | 253.28294.334 |
| 2026.1 | Unified IntelliJ IDEA | 261.22158.277 |
| 2026.2 | Unified IntelliJ IDEA | 262.8665.258 |
| 2026.3 EAP | Unified IntelliJ IDEA, pinned EAP | 263.5153.40 |

All listed targets passed binary compatibility checks for the package tested on that date. These are historical verification results, not a claim that every subsequent plugin build or IDE patch has been checked. No upper IDE build limit is declared; future versions and later EAP builds require verification. The 2026.3 result applies only to the exact EAP build listed above.

## First use

Comment navigation and highlighting work without an AI API key.

For AI analysis or generation:

1. Open **Settings > CoDAT Plugin Settings**.
2. Configure and enable an AI provider with your API key and model.
3. Review the **Prompt Templates**, including **Sketch**, **SP Generator**, and **Code Analysis**.
4. Open a Java file. Use the **M** gutter icon for method actions or the **CC** icon beside a method's Javadoc or block comment to generate SP specifications.

Generated text appears in a review dialog before you apply it. TODO comments are developer notes and do not have code analysis actions.

## Update CoDAT

Download the latest ZIP and repeat **Install Plugin from Disk...**, then restart IntelliJ IDEA if prompted.

Builds with the built-in updater also provide **Settings > CoDAT Plugin Settings > Plugin Update > Update CoDAT**. This downloads the latest published ZIP from this repository and stages installation for the next IDE restart.
