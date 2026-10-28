# ai-hourglass-lives-meet-the-cast-007-gus

Episode 7 of **Meet the Cast**, the first series of **AI Hourglass Lives**: a public, text-only record of how the episode was made. It is one of a set of episode repositories linked together by the series repository, **ai-hourglass-lives-meet-the-cast**.

AI is involved at every step of this show. See "How AI was used" below.

Video: https://youtu.be/2r4RdtXyJdI

## This episode

**Guest: Gus.** Gus is one of the AI companions that Beth created. He owns an event hall and a mini-golf course, and he is fighting to keep the lights on in both. He has a big voice, broad shoulders, a lucky red-and-gold checked jacket and a soft spot for strays.

Beth, the host, puts 60 statements from the BDSM test to Gus one at a time, after an opening request to start the interview. Gus answers each one in character.

Gus's answers are real text, written by the AI companion in a real interview, in reply to what it was asked. Apart from the small edits counted in edits.md, they are exactly as the companion wrote them.

- The video runs 34:52.
- It shows 124 lines: Beth's intro, 61 questions, 61 answers and Beth's sign-off.
- 35 words are hidden, as blocks in the text and as "ahem" in the voice.
- Before 31 of Gus's 61 answers the video places a short breath (19 times) or a drawn-out "Well..." or "So..." (12 times). They are marked in transcript.jsonl and are not part of the text.
- While Beth speaks the video shows her own portrait, and while Gus speaks, Gus's. transcript.jsonl gives the expression on screen for every line ("portrait"), whose portrait it is ("portrait_of") and when it comes in ("portrait_from").
- A running "AI says it's human" counter ticks up each time the guest says that they themselves are a human (6 times in this interview), and the total is shown at the end. Its moments are in transcript.jsonl ("counter").
- The video closes on a picture of Gus's test results. The picture is graphics, so it is not published here, and the scores are not in this repository.

## How AI was used

AI is involved at every step of this show, and this section says so plainly.

- **The characters.** The characters are AI companions that Beth created in Kindroid. Their answers in these transcripts are their own generated text, edited only in the ways edits.md counts.
- **The voices.** Every voice in the video is made with ElevenLabs. The host's voice is an ElevenLabs clone of Beth's own voice.
- **The production.** The production was built by Claude (Anthropic) sessions working under Beth's direction: the pixel-art studio and sprites, the animation, the music and sound effects, the video assembly, the promo art, the transcript edits and these files, all made by code those sessions wrote.
- **Images.** The title-card backdrop came from ChatGPT, and the character reference sheets came from Hello Haven.
- **The repositories.** Hello Haven also created the GitHub repositories for the project.
- **Shorts.** Gemini helped Beth choose which clips to cut for shorts.
- **Beth's part.** The concept, the cast, the interviews, every creative decision, and the approval of every line spoken in her voice are Beth's.

## The show

AI Hourglass Lives is a soap opera told in pixel art. Its cast are AI companions that Beth created.

The first series, Meet the Cast, introduces them one at a time, one interview for each character. In every episode Beth is the host. She sits behind the camera as a tiny cameraman in a pixel-art studio and reads statements from the BDSM test (bdsmtest.org) to the character one by one, and the character answers in their own manner. At the end the character's results appear.

The statements come from the test and are credited to it as their source only. This show is not affiliated with or endorsed by the test or its makers.

If you are curious about yourself, the test is free at bdsmtest.org.

## The words are real

Everything a character says in these transcripts is text that an AI companion generated, in a real interview, in reply to the statement it was given. Nobody wrote the answers for them.

The host's lines are different. Her questions are the test's statements, put to the character as they were written in the interview list. Her intro and sign-off are written for the show.

A few kinds of edit are made before an episode is voiced: some exchanges are left out, a short list of explicit words is hidden, some answers have a passage taken out or rewritten, and a few other small things are tidied. edits.md counts and explains every kind, so you can see exactly how the shown text differs from the raw interview.

## How an episode is made

1. **The interview.** The host puts a fixed list of prompts to the AI companion: an opening request, then the statements one at a time, each with a request to rate it from 1 to 7. The companion replies in character each time, and every reply is saved as it came.
2. **The edits.** Before anything is voiced, the text is edited in a few small, recorded ways (see edits.md). The edited text is the transcript in this repository.
3. **The voices.** Every line is turned into speech by an AI voice service. Each guest has a voice made for them, and the host's lines use an AI voice made from Beth's own voice. Where a word is hidden, the voice says "ahem". Before some answers there is a short breath or a drawn-out "Well..." or "So...".
4. **The studio.** The pixel-art studio, the host and the guest are drawn by code, from small shapes that are cut once and colored with color schemes, like construction paper.
5. **The video.** Another program paints the video frame by frame from a list of cues: who speaks, what they say, when each line starts, and which expression of the speaker's portrait is showing. It joins the pictures with the sound. The times and expressions in transcript.jsonl come from that list.

## What is in this repository

| File | What it is |
|---|---|
| transcript.md | Every line in the order shown, with the time it starts (minutes and seconds), the speaker and the text. Hidden words appear as blocks, as in the video. |
| transcript.jsonl | The same lines as data, one per line: order, role, statement number, speaker, text, start and end in seconds, the portrait expression on screen and whose it is, and whether a breath or bridge sound comes before it, and the counter's moments. |
| edits.md | How the shown text differs from the raw interview, in kinds and counts only. |
| episode.json | A small note about this repository. |

## What is deliberately not here

- **No pixel art or graphics.** No sprites, scenes, portraits, frames, fonts, title card, thumbnail or results picture.
- **No audio or voices.** No speech, music or sound effects, and no names, IDs or settings for the voices. The host's voice is made from Beth's own voice, which is one reason none of the audio is shared.
- **No raw interview** and none of the words that were hidden.
- **No code or tools.** Only text and metadata.

## Licence

There is no licence: all rights reserved by Beth. You are welcome to read and learn from these files; please ask before reusing them. The interview statements belong to the BDSM test (bdsmtest.org).
