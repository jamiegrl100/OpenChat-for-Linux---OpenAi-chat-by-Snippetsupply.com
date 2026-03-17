# Verifying Downloads

For each release, SnippetSupply provides a `SHA256SUMS.txt` file.

## Verify on Linux

1) Download the file you want (AppImage / .deb / tarball) and `SHA256SUMS.txt`.

2) In the folder where you downloaded them, run:

```bash
sha256sum -c SHA256SUMS.txt
You should see OK next to the file you downloaded.
If verification fails
Re-download the file and try again.
Make sure the filename matches exactly (including spaces/case).
If it still fails, contact support: jamie.folsom@proworkbench.com
