# consumer-rights-cell

**Live: https://sjgant80-hub.github.io/consumer-rights-cell/**

Answers questions about the Consumer Rights Act 2015, Part 1 from its own text only: the best-supported sentence, word for word, with its passage and character offsets. Refuses questions outside its lane.

A cell folded by [genome-fold](https://github.com/sjgant80-hub/genome-fold) from 5 document(s) in `corpus/` (372 passages). No language model: the answer is a sentence of the corpus, word for word, with the passage it came from and its character offsets, so anyone can check it.

## Ask it

```bash
echo '{"question":"Where is oral implied explained?"}' | node genome/act.mjs
```

A question outside the lane is refused and escalated; an answer leaves only when the judge verifies it.

## The birth check

This repository is admitted as a cell of the estate genome only when its four traits hold on its own hooks: it describes itself (`seed.json`), its judge tells a real answer record from the same record with one word altered, its health and reversible tombstone work, and its lane takes an in-lane question and refuses an off-topic one. CI runs the check on every push (`uses: sjgant80-hub/estate-genome@v1`).

```bash
git clone https://github.com/sjgant80-hub/estate-genome && node estate-genome/bin/genome-check.mjs .
```

## The lane

in lane when at least 50% of the question's content words appear as whole words in the indexed passages. The share was chosen on half of the questions generated from this corpus's own words and a fixed off-topic set, and measured on the other half: in-lane accepted 1, off-topic refused 0.8667. The questions are in `data/lane-questions.json`.

## Licence

The code (`kernel/`, `genome/`) is MIT, `LICENSE`, by Simon Gant. The corpus (`corpus/`) is not: it is under the Open Government Licence v3.0; see `CORPUS-LICENCE.md`.

Supplied by [AI Native Solutions](https://www.ai-nativesolutions.com). Support is agreed per deployment, in each deployment's agreement.
