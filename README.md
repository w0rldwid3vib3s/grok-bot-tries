# Grok Bot Tries — distribution pack v1.1 slim

Nine short clips of Grok Bot (glossy white sphere, black eyes) for X and YouTube.
Give this whole folder, or the zip it came in, to the posting bot. The bot should read `manifest.json` first.

## What to post

| Order | File | Cut | Ask |
|---|---|---|---|
| 1 | `videos/01-goal.mp4` | Scores a goal. 6s, 9:16 | Reply with the next sport |
| 2 | `videos/02-coffee.mp4` | Before coffee / after coffee. 6s, 9:16 | Tag a friend |
| 3 | `videos/03-skate.mp4` | Ollie. 6s, 9:16 | Reply yes or no |
| 4 | `videos/04-pancake.mp4` | Flips a pancake. 6s, 9:16 | Comment the next meal |
| 5 | `videos/05-dance.mp4` | Club floor. 6s, 9:16 | Reply with a song |
| 6 | `videos/06-space.mp4` | Drifts off. 10s, 16:9 | Reply with a destination |
| 7 | `videos/07-fire.mp4` | Discovers fire. 6s, 9:16 | Comment the next invention |
| 8 | `videos/08-wheel.mp4` | Becomes the wheel. 6s, 9:16 | Tag who needs one |
| 9 | `videos/09-electricity.mp4` | Discovers electricity. 6s, 9:16 | Comment next invention |

Post **one a day**, in this order. Do not dump the pack in one hour.
Vertical files are YouTube Shorts. `06-space` is a normal widescreen upload.

## How the bot should behave

1. Upload `file` from the manifest (hooks and CTAs are already burned in for muted autoplay).
2. On X, paste `x.text` exactly. Native video, not a link.
3. On YouTube, set `youtube.title`, `youtube.description`, `youtube.tags`, and the matching file in `thumbnails/`. Pin `youtube.pinned_comment`.
4. One ask per post. It is already in the copy. Do not add a second follow-spam line.
5. After a post, set `status` to `posted` and write the URL into `posted_url`. Wait `gap_after_hours` (22).
6. If a post is quiet, reply once with the same question. Do not delete and repost the same day.
7. Do not post this README, the manifest, the zip, or the brand still.
8. Do not present the series as an official xAI ad. It is an original mascot series.

This zip has no `videos/clean/` folder. The captioned files are the only masters. That is intentional so the pack stays small enough for a bot to accept.

## Sound

Each clip already has generated sound (crowd, cafe, kitchen, club, a quiet space bed).
Keep it. On X you can swap in a trending sound only if the composer does not kill the picture.
On YouTube, do not lay a commercial song under the clip. If a claim hits, strip the audio from the same file and re-upload it.

`audio_vibe` in the manifest is a hint for picking a platform sound, not a track to download.

## Character notes

The face stays a white sphere with black eyes in every clip.
Skate and dance grow tiny feet so he can move. Pancake grows a little body so he can cook.
Goal, coffee, and space stay a pure sphere. That mix is intentional. Do not "fix" it in the caption.

Reference still: `brand/grok-bot-mascot.jpg`.

## Follower engine

Every caption already ends with a follow line, but the **first** line is a reply, tag, or comment ask.
Replies are the growth lever. The follow line is the closer. Leave that ratio alone.
When someone answers the question, the next pack should actually do that activity.

## Delivery

There is no zip. Each clip is its own URL in bot.txt and manifest.json.
Download one video, post it, then stop until the next day.

