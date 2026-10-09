Public files the Tumtum app fetches at runtime. Published with GitHub Pages.
- `videos.json`: the YouTube Songs and Video Stories lists. Edit it here (on
  GitHub's web editor is fine) to add, remove or re-sort videos; phones pick up
  the change on their next launch. Regenerate it from the channels with
  `python tool/videos/build_video_list.py --site ../tumtum-content` in the app
  repo.
Schema: `{"version": 1, "updated": "YYYY-MM-DD", "videos": [{"id", "youtubeId",
"kind": "song" | "story", "lang": "en" | "ml", "title": {"en", "ml"},
"channel", "seconds"}]}`.
Videos play from YouTube in YouTube's own embedded player. They belong to
their creators, who earn from any ads in them; YouTube's Terms of Service
apply.
