# Beyond WordPress

A WordPress Playground Blueprint that creates a landing page linking to 26 browser-based CMS, framework, application and library demos.

Download [launch.html](launch.html), open it in your browser, and select **Launch the directory in Playground**.

The directory itself runs in WordPress. It links to independent projects that reuse Playground’s PHP.wasm packages, build on Playground, cite it as inspiration, or use related PHP runtimes. Each entry opens its demo or source code in a new tab.

Created by Fellyph Cintra for the CMS Conf session “Your CMS in the Browser.”

## Explore

- Shared PHP tools include Joomla, Silverstripe, Laravel, Moodle, Shopware, Omeka S, Nextcloud, FacturaScripts and PortalDots.
- Symfony’s Package Radar boots from a Blueprint. TYPO3 has a documented adaptation of Playground.
- Frappe and Wagtail use Python and Pyodide and cite WordPress Playground as inspiration.
- Drupal, Twig, CakePHP, CodeIgniter, Laminas and BEAR.Sunday use related PHP runtimes.
- The directory also includes BPMN Canvas, PHP Arena, BoxPacker, PHPCoord, Wizardawn, CodeCompared and PHP Scholar.

[Project sources and browser checks](docs/projects.md) explain the relationships and current demo limitations. Joomla credits Herman Peeren, and Silverstripe credits Andy Adiwidjaja.

## Run

Open the downloaded launcher and select its launch button. The Blueprint installs a small block theme, creates the landing page, and sets it as the homepage. It bundles the small logos in the theme stylesheet.

The initial load needs internet access to download WordPress and the runtime. External demos have their own download, browser and persistence requirements. Some entries open a source repository.

To run locally with Node.js 20.18 or newer:

```sh
npx @wp-playground/cli@latest server --blueprint=blueprint.json
```

The launcher embeds the Blueprint in its link, so it works from a downloaded copy of this private repository.

## Update the directory

Edit `blueprint.json`:

- The `installTheme` step contains the theme stylesheet, template and PHP enqueue hook.
- The `runPHP` step creates the page from WordPress block markup.
- Each project uses a named link, a description, and a small logo through its CSS class.

Keep links and technical claims aligned with [the project sources](docs/projects.md). When adding an entry, identify its runtime relationship and verify its destination in a browser.

After editing the Blueprint, regenerate the embedded link in `launch.html` with the command below. Run it from the repository root.

```sh
python3 - <<'PYTHON'
import base64
import json
import re
from pathlib import Path

blueprint = json.loads(Path("blueprint.json").read_text())
encoded = base64.b64encode(
    json.dumps(blueprint, separators=(",", ":"), ensure_ascii=False).encode()
).decode()
url = "https://playground.wordpress.net/#" + encoded
launcher = Path("launch.html")
launcher.write_text(re.sub(
    r'https://playground\.wordpress\.net/#[^"]+',
    lambda match: url,
    launcher.read_text(),
))
PYTHON
```

## Credits and license

Original Blueprint code and documentation are licensed under MIT. WordPress and the linked projects retain their respective licenses. Project logos and trademarks belong to their owners. Their inclusion identifies the projects. [Logo sources](docs/directory-logos.md).

[WordPress Playground](https://github.com/WordPress/wordpress-playground) supplies the runtime and Blueprint infrastructure.
