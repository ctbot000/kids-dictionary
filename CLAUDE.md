# Writing rules

This repository is an English dictionary for Korean-speaking kids. Read
[README.md](README.md) for the layout and the steps for adding a word.

The reader is a young child who is still learning English.

## Pronunciation

The line under the title says the word two ways: American English in IPA, then
the same sounds in Hangul for a kid who cannot read IPA yet.

- IPA between slashes, with ˈ before the loudest syllable: /bəˈnænə/.
- Where Americans say the vowel two ways, write /ɔː/: *dog* is /dɔːɡ/, not
  /dɑːɡ/, so the same vowel looks the same in every entry.
- Hangul that follows the English sounds, not the Korean loanword: *banana* is
  버**내**너, not 바나나. Bold the loudest syllable.

## English meaning

The meaning must be easier to read than the word it explains.

- Two to four sentences, ten words or fewer each.
- Common, everyday words only. If a word in the meaning is harder than the
  word being explained, use a simpler one.
- Start with what it is, as a full sentence — *An apple is a round fruit.* —
  then say what it looks like, what it does, or what it is for.
- Concrete over abstract: things a kid can see, hear, touch, taste, or do.

## 한국어 뜻

- The everyday word a Korean child would say: *mom* is 엄마, not 어머니.
- Only the meanings a kid needs. Leave out rare, technical, and adult senses.

## Examples

- One to three short sentences a kid might say or hear.
- Each has a natural Korean translation, with 나 for *I* and a friendly 해요
  ending: 나는 사과를 좋아해요.
- Bold the word in the English sentence and its meaning in the Korean one.
  Keep punctuation outside the bold — `"**사과**"를`, not `**"사과"**를`:
  bold that ends in punctuation cannot close right before a Korean letter,
  and GitHub shows the asterisks instead.

## Title emoji

Put one emoji before the word when one clearly shows it: 🍎 apple. Leave it
out when none does — a misleading picture is worse than none.

## Quiz

Three questions that check the English meaning, so a kid finds out whether
they understood it.

- Ask only about what the English meaning says, in its words or easier ones:
  *What does a cat say?*
- Three choices per question, exactly one right. Make the wrong ones plainly
  wrong — silly is fine — never half true: a banana is not "black", because
  old ones are.
- Vary where the right choice sits. The site shuffles them anyway.
- List the answers in order in the `<details>` block, written exactly like the
  right choice. The site checks taps against it, and leaves a quiz whose
  answers do not match as plain text.

## More than one meaning

Give a word a second meaning only when a kid needs both — *orange* is the
fruit and the color. Then number the meanings and keep the numbers lined up:

- 한국어 뜻 and English meaning are numbered lists, one item per meaning.
  Each English item follows the rules above on its own.
- Examples has one example per meaning, numbered the same way.
- The quiz asks about every meaning.
- The part-of-speech line lists every part of speech the meanings use:
  *noun, adjective* · 명사, 형용사.
- The README row lists every Korean meaning: 오렌지, 주황색.

[words/orange.md](words/orange.md) is the model.

## Keeping it consistent

If a word needs something these rules do not cover yet — an irregular plural,
say — write the rule in the same change, and update [TEMPLATE.md](TEMPLATE.md)
too if every entry should follow it. Every later entry then takes the same
shape.

## Site

Pushing to `main` publishes the dictionary to
<https://ctbot000.github.io/kids-dictionary/> through GitHub Pages. The README
is the home page and each file in `words/` becomes a page with no front matter
needed; `_config.yml` explains the build. On word pages, a 🔊 button says the
word with the browser's own English voice, and the quiz choices become buttons
to tap; both are done by the layout, so an entry needs nothing extra for them.
After pushing a new word, check its page on the site.

## Git

Commit and push to `main` once the entry and its row in the README table are
both in.
