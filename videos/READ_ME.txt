HOW TO ADD / REMOVE PROJECT PREVIEW VIDEOS
============================================

This folder is where your "Featured Projects" preview clips live.
The website is already wired to look for these 3 files:

  videos/motion-graphics.mp4          -> "Kinetic Titles & Motion Reel" card
  videos/corporate-brand-video.mp4    -> "Corporate Brand Video" card
  videos/real-estate-video.mp4        -> "Real Estate Walkthrough" card

TO ADD YOUR OWN VIDEO TO AN EXISTING CARD:
  1. Export/compress your clip as an MP4 (H.264), ideally under ~8-15MB,
     short (5-15 sec loop works best), no audio needed since it plays muted.
  2. Name it exactly as listed above (or update the filename in index.html,
     see step 3).
  3. Drop the file into this "videos" folder.
  4. Refresh the website - it will autoplay on loop whenever that project
     card is visible on screen. If the file is missing, the card just shows
     its colored gradient thumbnail instead (nothing breaks).

TO ADD A BRAND NEW PROJECT CARD:
  1. Open index.html and find the <!-- HOW TO ADD / REMOVE PROJECT VIDEOS --> 
     comment right above the "proj-grid" section (Featured Projects).
  2. Copy one whole block from <div class="proj-card"> to the matching
     closing </div>.
  3. Paste it right after, and change:
       - the gradient class (g1, g2, g3, g4, g5, or g6) for a different color
       - the <source src="videos/your-file.mp4"> path
       - the category tag text (e.g. "Wedding", "YouTube", "Reels")
       - the title (<h3>) and description (<p>)
  4. Add your new video file into this folder with the matching name.

TO REMOVE A PROJECT CARD:
  1. Open index.html, find the project you want to remove inside the
     "proj-grid" section.
  2. Delete everything from its opening <div class="proj-card"> to its
     matching closing </div>.
  3. (Optional) delete the matching video file from this folder.

That's it — no other code changes are needed.
