# ownCloud Documentation (v2)

This project is a port of the ownCloud documentation, that was previously generated using [Sphinx-Doc](http://www.sphinx-doc.org), to [Antora](./docs/what-is-antora.md).
Fundamentally, not that much has changed.

All of the same information is still available.
However, here's what has changed:

1. The platform (and tools) used to build the documentation, which is [Antora](./docs/what-is-antora.md).
2. The file format that the documentation is written in, which is [AsciiDoc](./docs/what-is-asciidoc.md).
3. The <abbr title="User Interface">UI</abbr> & <abbr title="User Experience">UX</abbr> of the documentation

## Quick Start Guide

If you're looking for the <abbr title="To Long; Didn't Read">tl;dr</abbr> guide to getting started with the docs, this is it.

1. Either install [the AsciiDoc Live Preview plugin](https://asciidoctor.org/docs/editing-asciidoc-with-live-preview/) for Firefox, Google Chrome, or Opera or [an AsciiDoc Live Preview plugin](https://asciidoctor.org/docs/editing-asciidoc-with-live-preview/#using-a-modern-text-editoride), if your text editor or IDE has one.
2. In a feature branch, branched from master, change the relevant [AsciiDoc](./docs/what-is-asciidoc.md) files.
3. Push your feature branch to the repository and create a PR from it.
4. Make any requested changes.
5. Your PR will be merged.

## Contributing to the Docs

If you've been contributing to the previous version of ownCloud's documentation, which used reStructuredText and Sphinx-Doc, here's how to get started contributing to the new version of the documentation.
Unlike the previous version of the documentation, you don't, necessarily, need to install a large number of tools and packages just to review your changes.

### Only Making Text Changes?

If you're only making text changes, then add the AsciiDoc Live Preview plugin:

1. To your [browser](https://asciidoctor.org/docs/editing-asciidoc-with-live-preview/) (The supported browsers are: *Firefox*, *Google Chrome*, or *Opera*).
2. To your [text editor or IDE](https://asciidoctor.org/docs/editing-asciidoc-with-live-preview/#using-a-modern-text-editoride), *if it has one*.

Using one, or both, of these, you can quickly check if the changes you make are what you expect, and if there are any render errors.
If the document renders as you expect, then you can commit the changes and push them to the docs repository.
**Please note:** any links to internal files will not render correctly.
The next section discusses this in more detail.

### Are You Working With Inline Code Examples, Images, and Attachments?

If, however, you're linking to local files, such as inline code examples, images, and attachments, then you need to [install Antora's command-line tools](./docs/install-antora.md).
This is because the Live Preview plugin won’t know the complete path to the local file, so won’t be able to correctly render a link to it.
All other kinds of links should work properly, however.

In this case, you need to use Antora to regenerate the documentation and manually check if there are any broken links or if something looks amiss.
Alternatively, you could use a tool, such as [NPM’s broken-link-checker](https://www.npmjs.com/package/broken-link-checker), to check broken links for you, on the pages that you changed.

Next, you need to learn how to [build the docs](./docs/build-the-docs.md) from the command line and how to review the changes in your browser.

### Now You're Ready to Contribute

Now that you've installed the required tools, you're ready to contribute.
So it’s time to learn [the AsciiDoc basics](./docs/what-is-asciidoc.md).
Then, you can create meaningful commits and a PR with your changes.

## Styling the Docs

If you want to make suggestions or provide corrections to the look and feel of the ownCloud documentation, then please refer to [the docs-ui repository](https://github.com/owncloud/docs-ui/blob/master/README.adoc).
