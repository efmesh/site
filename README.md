# efmesh.com — EF Meshtastic Community

An unofficial community guide for using Meshtastic at Electric Forest. Help festival-goers find their squad without cell service.

**Live site:** <https://efmesh.com>

**Not affiliated with or endorsed by Electric Forest, Insomniac, or Madison House Presents.**

---

## Stack

- [MkDocs](https://www.mkdocs.org/) with the [Material](https://squidfunk.github.io/mkdocs-material/) theme
- Hosted on GitHub Pages with a Cloudflare-backed CNAME for `efmesh.com`
- Built and deployed automatically by GitHub Actions on every push to `main`

## Local development

```bash
pip install mkdocs mkdocs-material mkdocs-minify-plugin
mkdocs serve
```

Then open <http://127.0.0.1:8000>.

To build a production bundle locally:

```bash
mkdocs build --strict
```

## Contributing

Open a pull request, or drop suggestions in the
[EF Meshtastic Discord thread](https://discord.com/channels/260909643574935553/1111482301730271232).

## License

Content is community-contributed. Code is MIT. Hardware brand names and logos belong to their respective owners.
