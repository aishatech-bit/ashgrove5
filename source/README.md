# Updating the Ashgrove site

The site is one page: `../index.html`, built from `index.src.html` by `build.py` (Python 3, no packages needed).
Edit the source, then run `python3 build.py` and re-upload `index.html` (and `assets/` if the video changed).

## Customer testimonials and photos
- Edit the `REVIEWS` list in `index.src.html`: name, estate, review text.
- Add a photo: save it as `images/<key>.webp` (a clear, face-centred square, at least 256x256),
  then add `img:'<key>'` to that testimonial and rebuild. Without a photo, an initials circle is shown (never a broken image).
- Star ratings are only shown when a testimonial has `r:1-5`.

## Team
- Edit the `TEAM` list: `{n:'Full Name', r:'Role', img:'<key>'}`; save the photo as `images/<key>.webp` and rebuild.
- If a photo is missing, the card shows initials instead of a broken image.
