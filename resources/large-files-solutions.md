# Large files hosting solutions

I need to upload a file that is larger than 100MB, but [GitHub does not allow
that](https://docs.github.com/en/repositories/working-with-files/managing-large-files/about-large-files-on-github#about-size-limits-on-github).
How can I make my large files available?

- If your file is at most 2GB, GitHub recommends
  [using Git LFS](https://docs.github.com/en/repositories/working-with-files/managing-large-files/about-git-large-file-storage).
- If your file is at most 50GB, then you should consider [hosting it as a record
  on
  Zenodo](https://support.zenodo.org/help/en-gb/1-upload-deposit/80-what-are-the-size-limitations-of-zenodo)
  for example. Artifacts have also used
  [Huggingface](https://huggingface.co/docs/hub/en/storage-limits) successfully
  to host large ML models.
- If directly uploading your (compressed) file to one of the aforementioned
  platforms does _not_ work, then you may split the file into multiple chunks.
  You can also contact the artifact chairs if you have trouble with this step.
- Do _not_ use Google Drive or Dropbox links; they are not version-controlled or
  persistent in any way.
