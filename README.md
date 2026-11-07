# Pevio catalogue

Static feed for the Pevio iOS app. The app fetches:

- `catalogue.json` — paper, frame, lab and weekly-pick records
- `images/<name>.jpg` — artwork named by the record's `cover` field

Base URL used by the app:

```
https://raw.githubusercontent.com/really530/Pevio/main
```

Publishing a change is just a commit: the client sends `If-None-Match` and
picks the new document up on the next refresh (Sizes tab, pull to refresh).
