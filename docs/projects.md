# Browser project directory

Research updated November 13, 2026. The original survey identified 16 entries. This edition adds Wagtail, PortalDots, BEAR.Sunday and seven applications or libraries. The 26 entries count Wagtail with Django and Frappe with ERPNext. Multiple Laravel examples demonstrate different applications of one framework.

## Shared PHP tools

These projects use PHP.wasm packages maintained by WordPress Playground.

| Project | What to explore | Primary source |
|---|---|---|
| [Joomla](https://joomla-projects.github.io/joomla-playground/) | Open the CMS that Herman Peeren brought to the browser. | [Evidence](https://github.com/joomla-projects/joomla-playground/blob/main/package.json) |
| [Silverstripe](https://s2hub.github.io/silverstripe-cms-playground/) | Explore the page tree in Andy Adiwidjaja’s CMS prototype. | [Evidence](https://github.com/s2hub/silverstripe-cms-playground/blob/main/package.json) |
| [Laravel](https://liminal.aschmelyun.com/) | Edit a route or a Blade view in Andrew Schmelyun’s Liminal IDE. | [Evidence](https://github.com/aschmelyun/liminal/blob/main/package.json) |
| [Moodle](https://ateeducacion.github.io/moodle-playground/) | Explore course provisioning in a browser-based learning platform. | [Evidence](https://github.com/ateeducacion/moodle-playground) |
| [Shopware](https://playground.fos.gg/) | Try a storefront backed by MariaDB in WebAssembly. | [Evidence](https://github.com/FriendsOfShopware/shopware-playground) |
| [Omeka S](https://ateeducacion.github.io/omeka-s-playground/) | Explore the software that museums use to build digital collections. | [Evidence](https://github.com/ateeducacion/omeka-s-playground) |
| [Nextcloud](https://ateeducacion.github.io/nextcloud-playground/) | Try the file-sharing and collaboration platform. | [Evidence](https://github.com/ateeducacion/nextcloud-playground) |
| [FacturaScripts](https://facturascripts-playground.pages.dev/) | Explore invoicing and business management. | [Evidence](https://github.com/erseco/facturascripts-playground) |
| [PortalDots](https://github.com/PortalDots/PortalDots/tree/6.x/wasm-demo) | Explore the Laravel prototype for managing school festivals. The source includes a PHP worker and SQLite setup. | [Evidence](https://github.com/PortalDots/PortalDots/blob/6.x/wasm-demo/src/php-worker.js) |

## Built on Playground

One team runs a PHP app directly in Playground. Another adapted Playground for its own CMS.

| Project | What to explore | Primary source |
|---|---|---|
| [Symfony](https://playground.wordpress.net/?blueprint-url=https%3A%2F%2Fwordpress.github.io%2Fblueprints%2Fblueprints%2Fsymfony-package-radar%2Fblueprint.json) | Launch Package Radar from a Blueprint that boots Symfony directly. | [Evidence](https://developer.wordpress.org/playground/handbook/guides/php-frameworks/) |
| [TYPO3](https://github.com/macopedia/typo3-wasm-playground) | Read Macopedia’s proof of concept. The hosted demo currently requires sign-in. | [Evidence](https://news.typo3.com/article/budget-idea-report-one-click-typo3-playground) |

## Playground in Python

These teams cite WordPress Playground as inspiration and run Python with Pyodide.

| Project | What to explore | Primary source |
|---|---|---|
| [Frappe / ERPNext](https://frappe-playground.lubus.in/) | Explore the Frappe framework and its experimental ERPNext app with LUBUS’s Playground. | [LUBUS project overview](https://lubus.in/frappe-playground) · [Source code](https://github.com/lubusIN/frappe-playground) |
| [Wagtail / Django](https://bakerydemo-webassembly.netlify.app/) | Explore Wagtail’s bakery demo, where the CMS runs on Python and SQLite inside the browser. | [Evidence](https://wagtail.org/blog/a-wagtail-demo-in-your-browser/) |

## Other PHP runtimes

These projects use Sean Morris’s PHP-Wasm or PHP-CGI-Wasm toolchain.

| Project | What to explore | Primary source |
|---|---|---|
| [Drupal](https://wasm-drupal.mglaman.dev/) | Open Matt Glaman’s browser demo of Drupal. | [Evidence](https://github.com/mglaman/wasm-drupal) |
| [Twig](https://twig.symfony.com/play) | Edit a template and see its rendered output. | [Evidence](https://symfony.com/blog/introducing-the-new-twig-playground) |
| [CakePHP](https://seanmorris.github.io/php-wasm/install-demo.html?framework=cakephp-5) | Launch the CakePHP 5 example. | [Evidence](https://github.com/seanmorris/php-wasm#examples) |
| [CodeIgniter](https://seanmorris.github.io/php-wasm/install-demo.html?framework=codeigniter-4) | Launch the CodeIgniter 4 example. | [Evidence](https://github.com/seanmorris/php-wasm#examples) |
| [Laminas](https://seanmorris.github.io/php-wasm/install-demo.html?framework=laminas-3) | Launch the Laminas 3 example. | [Evidence](https://github.com/seanmorris/php-wasm#examples) |
| [BEAR.Sunday](https://koriym.github.io/wasm-todo/) | Try a to-do application that runs on PHP-CGI-Wasm and SQLite. | [Evidence](https://github.com/koriym/wasm-todo) |

## Applications and libraries

These tools use Playground’s PHP.wasm packages for specific tasks, from editing a diagram to converting coordinates.

| Project | What to explore | Primary source |
|---|---|---|
| [BPMN Canvas](https://solis-eduardo.github.io/bpmn-canvas/) | Model a process in a Laravel application. | [Evidence](https://github.com/solis-eduardo/bpmn-canvas/blob/main/demo/package.json) |
| [PHP Arena](https://loilo.github.io/php-arena/) | Run and share a PHP snippet from the editor. | [Evidence](https://github.com/loilo/php-arena) |
| [BoxPacker](https://www.boxpacker.io/en/master/visualiser.html) | Visualize how items fit into a shipping box. | [Evidence](https://github.com/dvdoug/BoxPacker/blob/master/playground/pack.worker.ts) |
| [PHPCoord](https://phpcoord.net/en/master/demo.html) | Convert coordinates between reference systems. | [Evidence](https://github.com/dvdoug/PHPCoord/blob/master/playground/convert.worker.ts) |
| [Wizardawn](https://truculent.org/wizardawn/) | Try the PHP generators for tabletop role-playing games. | [Evidence](https://github.com/KingAragorn/Wizardawn/blob/main/package.json) |
| [CodeCompared](https://codecompared.to/) | Explore the same programming examples across languages. Its PHP runtime uses Playground’s PHP.wasm packages. | [Evidence](https://github.com/CodeCompared/php-wasm) |
| [PHP Scholar](https://github.com/fellyph/php-exercise-playground) | Explore Fellyph Cintra’s source for a browser-based PHP exercise environment. | [Evidence](https://github.com/fellyph/php-exercise-playground) |

## Related implementation outside the browser directory

NativeBlade packages Laravel and Livewire in a Tauri WebView. Its runtime imports Playground’s PHP.wasm packages. The intended deployment is an installed application. [Runtime source](https://github.com/NativeBlade/NativeBlade/blob/main/js/runtime/wasm-php.js)

## Verification notes

Wagtail rendered its bakery homepage in a fresh Chrome session. In the BEAR.Sunday demo, a new task remained visible after a page reload. The published TYPO3 demo redirected to a sign-in page, so its directory entry opens the public source. PortalDots and PHP Scholar also link to source. The other entries cite project code or documentation. Their individual application workflows have not all been tested.


## Browser rehearsal, November 13, 2026

All 26 project destinations opened when navigated directly in the in-app Browser. Three entries intentionally open source repositories: PortalDots, TYPO3 and PHP Scholar. The remaining entries open demos, editors or launchers. A successful page load alone does not establish that the underlying CMS has finished booting.

| Observed result | Projects |
|---|---|
| Laravel welcome page rendered in the Liminal preview after reopening the address in a fresh tab | Laravel. The initial in-app tab had shown a browser response error. The directory also offers [Liminal source](https://github.com/aschmelyun/liminal). |
| Application, editor or tool page visible | BEAR.Sunday, PHP Arena, Twig, CodeCompared, BoxPacker and PHPCoord. This check did not exercise every tool. |
| Launch button and browser compatibility notes visible | Drupal. The user must select Launch to start the CMS. |
| Initial page or runtime loader visible; completion depends on downloading and starting the environment | Joomla, Silverstripe, Moodle, Shopware, Omeka S, Nextcloud, FacturaScripts, Symfony, Frappe, Wagtail, CakePHP, CodeIgniter, Laminas and BPMN Canvas. Wagtail completed a separate cold-start test during initial research. |
| Page title loaded but no usable interface was confirmed | Wizardawn. The directory also offers [the project source](https://github.com/KingAragorn/Wizardawn). |
| Source files visible | PortalDots, TYPO3 and PHP Scholar. |

The first Liminal failure occurred when opening it from the live directory. Direct navigation worked. For rehearsal, the directory also exposes its maintainers’ repository. [Open Liminal directly](https://liminal.aschmelyun.com/)

[Directory logo sources](directory-logos.md)
