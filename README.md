# Moments to Rest — Audio Assets

Public audio repository for [moments to rest blog](https://www.momentstorestblog.com).

Files in `mp3/` are served via [jsDelivr](https://www.jsdelivr.com/) CDN and consumed by the On Air page on the Moments to Rest website.

## URL pattern

```
https://cdn.jsdelivr.net/gh/NeueStudio-Bailey/moments-to-rest-audio@main/mp3/[filename].mp3
```

Spaces and special characters in filenames are URL-encoded by the consuming JavaScript.

## To add a new segment

1. Drop the `.mp3` into `mp3/`
2. `git add mp3/<filename>.mp3 && git commit -m "Add <title>" && git push`
3. Within a few minutes, jsDelivr will serve the new file
4. Update the [on-air data Gist](https://gist.github.com/NeueStudio-Bailey/719444fbb1c7ccccf4d5d3c53381bea2) with a new entry pointing at the new URL

## Related

- **On Air data:** [Gist 719444fbb1c7ccccf4d5d3c53381bea2](https://gist.github.com/NeueStudio-Bailey/719444fbb1c7ccccf4d5d3c53381bea2)
- **Renderer:** Squarespace Code Block on `/on-air` on momentstorestblog.com
- **Project notes:** `~/Claude Code/Clients/Moments-To-Rest/Projects/on-air-system/`
