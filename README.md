# raw-legis-md

The pages of Moldova's State Register of Legal Acts, [legis.md](https://www.legis.md): one HTML file per
consolidated version of an act.

- `documents/0155/0155991.html` is legis.md's document 155991, in folders of 1,000. Its page on legis.md is
  `https://www.legis.md/cautare/getResults?doc_id=155991&lang=ro`.
- A file is the act's page on legis.md: its details table, the list of its versions with their in-force dates,
  and the full text with notes naming the act behind each change. Files up to 155991 come from an earlier
  archive and are the bare fragment; later ones are the same fragment wrapped in `<html>`.
- New pages are added as legis.md publishes them. Files are never changed once added.

To get only part of it:

```sh
git clone --filter=blob:none --sparse https://github.com/nicu-chiciuc/raw-legis-md
cd raw-legis-md && git sparse-checkout set documents/0155
```

## Use

Anyone may copy, change, publish and use these files for any purpose, commercial or not, without asking.

Official texts such as laws and government decisions are not protected by copyright in Moldova (Law 230/2022 on
copyright and related rights, art. 8 lit. b),
[legix.md/lege/2022/230#art_8__point_b](https://legix.md/lege/2022/230#art_8__point_b)). Everything else in this
repository, this README and the layout of the files, is dedicated to the public domain under
[CC0 1.0](LICENSE).

This is not an official publication.
