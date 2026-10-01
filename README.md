# Personal academic website

A single-page site written in plain HTML and CSS. There is nothing to install or build: open `index.html` in a browser to preview it.

## Folder layout

```
index.html          the whole site (content, styles, a little JavaScript)
assets/
  cv.pdf            put your CV here (the "Download CV" buttons point to it)
  img/              put your photo and figures here
```

## Adding pictures

Every dashed box on the page shows the file name it expects. Save your image into `assets/img/` with exactly that name and the box fills in automatically. No HTML editing is needed. If one image is used in two places (for example the TED paper figure appears under Research and Publications), a single file fills both.

| File name | Used for |
|---|---|
| `photo.jpg` | Your portrait (square crop works best) |
| `hbn-quantum-sensing.png` | M.Sc. thesis: VB- defects in h-BN |
| `soi-ri-sensor.png` | Adjoint-optimized refractive index sensor (Research and Publications) |
| `fet-alcs-sip.png` | alpha-CS and SiP FETs (Research and the TED paper) |
| `thz-differentiator.png` | THz temporal differentiator |
| `opamp-biomedical.png` | ICCIT op-amp paper |
| `self-balancing-robot.png` | RAAI paper and the robot project |
| `remote-sensing-dl.png` | Deep learning for remote sensing |
| `webcam-spectroscopy.png` | Webcam spectroscopy |
| `riscv-spi.png` | SPI interface for RISC-V |
| `toggle-sot-mram.png` | Toggle SOT-MRAM project (for example the mz toggling plot or toggle range vs beta) |

Use `.png` or `.jpg` as written in the table. To use a different format, change the file name in the matching `<img src="...">` in `index.html`. The captions under the Research figures are suggestions that only appear once an image is present, so edit them to match your figure.

## Adding links

Links marked `data-todo` (Google Scholar, LinkedIn, GitHub, ORCID, and the DOI and PDF links on each paper) stay hidden until you replace `href="#"` with the real address. To see which slots are still empty, add `?edit` to the page address (for example `index.html?edit`); empty slots appear outlined in orange.

## Colors

The page always opens in a bright light theme, whatever your computer's setting is. The moon button in the header switches to a dark theme for visitors who prefer it. To change the palette, edit the color values at the top of the `<style>` block in `index.html` (`--accent`, `--band-sky`, `--band-sun`, `--band-mint`, `--band-peach` and the `--hero` gradient).

## Before you publish

1. Add your CV as `assets/cv.pdf`. Consider using a copy without your phone number, since the site is public.
2. Fill in the links you want to show (above).
3. Check the paper titles and author lists against the published versions.
4. If you do not want the "Applying for fully funded PhD positions" line, delete the `<div class="status">` in the hero section.

## Hosting for free on GitHub Pages

1. Create a GitHub account and a new public repository named `your-username.github.io`.
2. Upload everything in this folder (`index.html`, `assets/`, `README.md`).
3. In the repository, open Settings, then Pages, choose the `main` branch and the root folder, and save.
4. After a minute or two the site is live at `https://your-username.github.io`.

A custom domain such as `yourname.com` can be added later under the same Pages settings.
