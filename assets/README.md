# Drop your images here

The scrapbook page at the end of the site looks for these files. Anything
missing just doesn't render — no broken image icons — so you can add them
one at a time and reload.

Names must match exactly (lowercase).

## The board

| File | What it is |
|---|---|
| `board.webp` | The maroon "17" collage. If present it replaces the drawn version entirely. |
| `main-photo.jpg` | Goes inside the polaroid's black window. Roughly square crops best. |

If you don't add `board.webp`, the page draws its own version — maroon
backdrop, 17 balloons, disco ball, cherries, love note, lipstick print,
star and hibiscus — and the polaroid sits on top of that.

## The stickers

| File | Which picture |
|---|---|
| `cats-glasses.png` | Two cats in red + blue glasses |
| `kissi-dedo.png` | "kissi dedo" anime baby |
| `jack-cat.png` | Cat with the bow and the whiskey bottle |
| `kawaii-cats.png` | Sheet of little drawn cats |
| `condom-cat.png` | The cat meme |
| `brush-heart.png` | Pink brush-textured heart with sparkles |
| `birthday-kitten.png` | Kitten in a party hat with cake and tulips |
| `my-girl-heart.png` | Torn "my girl" paper heart |
| `tangled.png` | The Tangled frame |
| `hotel-transylvania.png` | The Hotel Transylvania frame |
| `monkey-heart.png` | Monkey in a party hat making a heart |
| `suit-cat.png` | Cat in a suit holding roses |
| `buff-cat.png` | Cat with the arms |

## Which ones need transparency

These are set as **cut-outs** — they get a white sticker outline traced
around the artwork, so they want a transparent background (PNG or WebP):

`suit-cat` · `birthday-kitten` · `monkey-heart` · `jack-cat` ·
`brush-heart` · `my-girl-heart` · `condom-cat` · `buff-cat`

The rest are treated as normal photos and get a plain white sticker border,
so a rectangular JPG/PNG is fine for them.

## Moving things around

Positions live in the `STICKERS` array in `index.html` — search for
`const STICKERS`. Each entry has a CSS position, a width as a percentage
of the stage, and a rotation in degrees. Editing those is all it takes to
rearrange the layout.
