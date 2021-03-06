# Ad-block for PDF tickets

As a matter of principle, we shouldn't pay with our toner or ink for someone
else to put ads on tickets we've paid for.

## Prerequisites

You will need *Inkscape* to generate or update the PDFs, and *pdftk* to block
ads.

For convenience, PDFs are included in the repository. (They're smaller than the
source SVG files!)

## Usage

    pdftk BoardingPass.pdf stamp easyjet.pdf output ad-blocked-pass.pdf

## Contributing

Make your own blockers using Inkscape. Create a new document of the same paper
size (this is sometimes surprising: EU-based EasyJet uses US Letter) with a
transparent background, and a white rectangle at the appropriate location, and
check that it works. Then open a PR!
