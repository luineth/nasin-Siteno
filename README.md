# nasin Siteno
Toki Pona stenography theory and Plover implementation (sitelen + steno = siteno)

![Uni Sitelen Pona Render](/img/toki-uni-steno2.jpeg)

## nasin Siteno theory

All stenography systems have a theory, that is, a unifying way to simplify and type words on devices which only have 23 keys. In theory, you can type almost everything in toki pona using [only 7 keys](https://www.reddit.com/r/tokipona/comments/pc6bkn/nasin_tenokasi_the_way_of_stenography_7_key_input/), but this would require every word to be memorized rather than a few principles.

Stenography keyboards have three main sections:

1. Initials
2. Vowels
3. Finals

(If you don't have a stenography keyboard, don't worry! You likely can still use this input method using [Plover + a regular keyboard](https://github.com/openstenoproject/plover/wiki/Supported-Hardware#keyboards). Diagrams in this README will use the layout of my steno device, [The Uni v4](https://stenokeyboards.com/products/the-uni-v4), but translating these to other steno devices will be pretty straightforward. The number key in particular may be in a different location.

So, how do you type a word? Follow these steps!

### 1: Find a word's 3 letter abbreviation

All toki pona words can be chorded (pressing multiple keys simultaneously) in one stroke once you determine the three characters you need: the initial consonant, the initial vowel, and the final consonant.

The _initial consonant_ is just the first letter of a word. If the word begins with a vowel, the initial consonant is blank. For example:

- mi -> `m`
- ala -> (blank)
- kijetesantakalu -> `k`
- o -> (blank)

The _initial vowel_ is just that: determine the first vowel in a word. You may notice that there are only four vowel keys present, which is the only exception to keep in mind. If the first vowel is 'i', then leave the vowel blank. For example:

- mi -> (blank)
- ala -> `a`
- kijetesantakalu -> (blank)
- o -> `o`

The _final consonant_ is the last consonant in the word, _excluding_ a nasal 'n'. You can also think about the last consonant before the last letter of a word. For example:

- mi -> (blank)
- ala -> `l`
- kijetesantakalu -> `l`
- o -> (blank)
- lon -> (blank)
- nena -> `n` (because this 'n' is at the beginning of a syllable, we include it)

That's all you need!* Just sound the word out. Now you can learn the keyboard layout to type these letters.

(\* A few words require disambiguation with the *ante* key under the left pinkey. See step 3.)

### 2: The layout

The three groups of keys (6 consonants on the left, 4 vowels for the thumbs, and 6 flipped consonants on the right) match up to the three letter abbreviation you derived from the last step.

![Latin Layout](/img/layout-latin.png)

*But hey, there are only 6 keys, and toki pona uses 9 consonants?* Right, you are. The most frequently used 6 consonants are accessed by pressing the keys directly, and the less common consonants require pressing both the top and bottom key at the same time:

![Disambiguation](/img/layout-latin-comb.png)

You can use this sitelen pona chart as a mnemonic devise to remember the keys and combinations. Top row consonants by themselves are the first consonant in the respective sitelen pona, and the combination letters are the second consonant. So, pressing "**s**ike" would be the letter 's', and pressing "si**k**e" and the key below (li), is the combination for 'k'.

![Sitelen Pona Layout](/img/layout-sitelen.png)

### 3: Disambiguation with 'ante'

A few words would have the same chord. In these cases, the chord will generate the more frequently used word. To type the alternate word, press the 'ante' key along with the chord. These are the current words which require disambiguation:

| chord | default word | alternate (adding 'ante') |
|---|---|---|
| `nas` | nasa | nasin |
| `mu ` | mun | mu |
| `luk` | lukin | luka |
| `pok` | poka | poki |
| `pal` | pali | pakala |
| `pij` | pimeja | pije |
| `ko ` | kon | ko |
| `kam` | kama | kalama |
| `kas` | kasi | kanse |
| `sel` | seli | selo |
| `sil` | sitelen | sijelo |
| ` al` | ala | ali |

## Questions

### What is stenography?

Stenography is an input system used to type extremely accurately and extremely quickly using minimal effort. Its most common application is transcribing court proceedings, but there is a growing hobbyist community for hardware and software. For more, check out the [Open Steno Project](https://www.openstenoproject.org/plover/).

### I found a mistake!

I'm not suprised. Please let me know! Right now it's a proof of concept, and I'd love any feedback!

## To do

- [ ] multiword briefs
- [ ] numbers
- [ ] ability to spell
- [ ] punct & cartouches
