# wxWidget Releases

This directory contains wxWidgets Gitian build results, signed by multiple people.

The layout of this directory is:

    <release-name>/
      <signer>/
        wxwidgets-build.assert - the result file produced by the signer's build process
        wxwidgets-build.assert.sig - the signer's signature certifying the result

This directory is created by the Gitian `gsign` command, after a successful `gbuild`.  It can be verified with `gverify`.

The source is wxWidgets-2.9.1 obtained from the wxWidgets site.

Normally, all output manifests in the result files should be identical between different signers.

See also:

* [Gitian builder](https://github.com/devrandom/gitian-builder)
