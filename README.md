# novar-media

The public pictures of www.novar.ai (Nova Rai's photographs, song covers and posters), served by GitHub Pages so search engines may index them.

The files keep the paths they have under `music/novarai/` in the site's Supabase storage. The site points at this host through one constant, `IMAGE_BASE` in `src/lib/media.ts` of Balzinho/novarai.

Only pictures already public on novar.ai belong here. Audio, films and downloads stay in Supabase.

To add new pictures after a release: `python3 ~/bonfire/novar_media_sync.py` (it reads the site's data, copies any missing picture here, commits and pushes).
