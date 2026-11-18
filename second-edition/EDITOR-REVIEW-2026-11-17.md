# Editor's review: The Art of Options War, second edition

For Henry, before your own read. Read 17–18 November 2026.

**What I read:** the prologue, the 18 chapters and the 3 appendices, all 22 files, in English and in Chinese, plus both READMEs, `second-edition/BUYING-PLAN.md` and the Book 1 line in `qs-studio/books/INVENTORY.md`. I checked the Mai material and the test figures against `~/repo/the-counted-trade`. I did not edit any chapter. This memo is the only file changed.

**How to read this memo:** each finding has a number and a tag.

- **MUST:** fix before release.
- **SHOULD:** fix if you have the time.
- **NOTE:** your call; nothing is wrong as it stands.

Quotes are copied exactly from the files. "v." means the numbered verse, and "¶" means a commentary paragraph, counted from the top of the Commentary.

---

## The six must-fix items

| # | Where | Problem |
|---|---|---|
| 1 | zh ch. 14–18, `zh/README.md`, `README.md` | The Part V Chinese reads as a translation of the English, not as your Chinese. The zh README still opens with a draft banner, and the main README says both editions were "written by hand". |
| 2 | `en/chapter-10.md` v. 10 | The Sun Tzu line says the opposite of what Giles wrote. |
| 3 | `en/` and `zh/chapter-01.md` v. 3 | The five constants are re-ordered. In Chinese this misquotes the most famous list in the book. |
| 4 | `zh/chapter-15.md` commentary | "十赔一" reverses the odds; it should be 一赔十. |
| 5 | `en/` and `zh/chapter-07.md` ¶2, appendix C | The Spitznagel credit is accurate on the facts but unfair in tone, and "oldest statement" claims too much. |
| 6 | `en/` and `zh/chapter-12.md` commentary ¶6 | The "business below what it can survive at" idea is credited to Lewis's account of Mai. I could not find support for that, so verify it or cut the attribution. |

---

## 1. The four items already flagged for you

### 1a. The Part V Chinese (chapters 14–18)

**Finding 1 — MUST. This is a careful translation of the English, not your Chinese yet.** The Chinese is accurate, complete and readable, and it matches the English line for line. That is the problem: it follows the English sentence by sentence and clause by clause. It keeps English word order ("……的时候，也就是……的时候"), English images ("一个论题戴着五个代码", "被算到了"), and English abstractions turned into nouns ("一次测量而不是一句预言"). Parts I–IV are written in Chinese: verses in a terse classical register, four-character turns, and the general's own lines in his own words. Part V falls back to modern prose that follows the English. Against Parts I–IV and Appendix A, which are good, Part V reads as a different hand.

It also drifts on terms. Parts I–IV call the buyer's outlay 权利金. Part V uses 借方 as a noun: "每一笔借方都小到可以整笔输掉" (ch. 15 v. 21), "过大的借方" (ch. 16 v. 9), "付一笔新的借方" (ch. 16 v. 10), "买方的借方，任何开盘都放大不了" (ch. 15 commentary). 借方 is the left column of a ledger. Use 权利金 or 所付之数 for the money, and keep 借方价差 only as the name of the spread.

Two public statements depend on this:

- `zh/README.md` line 1 reads "第五部分中文为初稿，待作者审定。" Remove it once you have done your pass.
- `README.md` line 37 says "Both editions were written by hand. The Chinese is not a machine translation of the English." That is not yet true of Part V. Either rewrite Part V in your own Chinese first, or soften the sentence until you have.

**The ten weakest sentences, with a suggested rewrite for each.** These are suggestions in roughly your Parts I–IV register. Use them as a starting point, not as final text.

| # | File, place | As written | Suggested |
|---|---|---|---|
| 1 | ch. 14 commentary ¶2 | 而两方都要为这份特权给庄家交钱：买卖价差、佣金、滑点。 | 两边还都得给场子交钱：买卖价差、佣金、滑点。 *("For the privilege" is a calque, and in Chinese markets 庄家 means a manipulator, not the house.)* |
| 2 | ch. 14 v. 11 | 每一张借方价差都是一张多头期权加一张空头期权，那张空头就是买进买方单子里的一小块卖方生意。 | 借方价差，是一多一空两张期权；那张空头，是夹在买方单子里的一小份卖方生意。 |
| 3 | ch. 14 v. 16 | 习惯不是一种立场，而是没有立场，市场向它收的是攻者的价。 | 凭习惯守，算不得立场，只是没有立场；市场照样按攻者的价收他的钱。 |
| 4 | ch. 14 commentary ¶4 | 二十个交易日里，这道差价复合成一张跨式的价格 | 放到二十个交易日上，这点差价就落进了跨式的价钱里 *(this also fixes the maths; see Finding 21)* |
| 5 | ch. 14 commentary ¶6 | 按平均价付钱的买方，平均而言，就付了这笔钱。 | 照平均价买的人，长年下来，交的正是这份工钱。 |
| 6 | ch. 15 v. 3 | 只有进攻的权利被以过低的价格卖给他时，这次进攻才强。 | 进攻之强，只在于这份权利卖给他时卖贱了。 |
| 7 | ch. 15 v. 8 (same in ch. 17 v. 4) | 第四种地，是盾：买在一本股票仓位身后的看跌，买在一本卖出权利金仓位身后的翼。 | 第四种地，是盾：持股背后买的看跌，卖权利金之后补的那条翼。 |
| 8 | ch. 15 commentary, the funnel | 算术没错，身体却是死的。 | 算术没错，借来的却是一具旧尸。 *(This keeps the 借尸还魂 image the paragraph is built on.)* |
| 9 | ch. 16 v. 19 (and the end of commentary ¶5) | 没有按它来定规模的买方，不是运气差，而是被算到了。 | 没按它定仓位的买方，不是运气差；这笔账早就摆在那里，是他自己没算。 |
| 10 | ch. 16 commentary ¶1 | 方差溢价，也就是期权买方为保护付出的钱、习惯性地多于那些波动最终造成的损失，从卖方那一岸读，是他的工钱；从买方这一岸读，是对每一次进攻的征敛 | 买保护的人所付，向来多于日后波动真正造成的损失，这就是方差溢价。从卖方那岸看，是工钱；从买方这岸看，是每次进攻之前先缴的税。 |

These three are close behind: "按一次突袭来定进攻的规模，不按一次入侵" (ch. 15 v. 21; try 规模按奇袭定，不按倾巢定); "同一个板块里的五张看涨价差，是一个论题戴着五个代码" (try 只是一个论题换了五个代码); and "麦描述自己的方法所用的说法，本书会认得出来" (ch. 15 commentary; try 麦讲自己方法的那几句话，读到这里的人都不陌生).

### 1b. Spitznagel and *The Dao of Capital* (ch. 7 commentary ¶2, appendix C)

**Finding 5 — MUST.** The bibliographic facts are right: *The Dao of Capital: Austrian Investing in a Distorted World* (Wiley, 2013) and *Safe Haven: Investing for Financial Storms* (Wiley, 2021). It is also right that *Umweg*, the roundabout path, comes from the Austrian economists (Böhm-Bawerk's roundabout production).

Three things are off:

- **Tone.** "The idea is Sun Tzu's … and it should be credited to the general" reads as if Spitznagel failed to credit a Chinese source. He did not hide one. His book is named for the Dao and is built on Laozi and on classical Chinese strategy, including Sun Tzu's *shi* (势). Check the opening chapters of your copy, but as I remember it he makes this connection himself. Correcting a credit he never withheld is the unfair part.
- **"Oldest statement" (appendix C) and "The idea is Sun Tzu's" claim too much.** In Spitznagel the roundabout idea draws on Laozi as much as on Sun Tzu, and the two texts are roughly contemporary. 以迂为直 is a clear early statement, not provably the oldest.
- **The Chinese ch. 7 repeats the same sentence** ("这份功劳应当记在将军名下").

Suggested EN, replacing the last four sentences of ch. 7 ¶2 from "His name for it comes from the Austrian economists": *"He takes the name from the Austrian economists, and he traces the idea himself to Laozi and to Chinese strategy. One of its clearest early statements is here, in Sun Tzu's chapter on 军争, the contest of armies. Spitznagel applies it to capital across decades … This book applies it to the single trade and the single season … The horizons differ; the line in the general's chapter is where this book found it."*

Appendix C: change "credits its oldest statement, 以迂为直, to Sun Tzu's chapter" to "reads one of its earliest statements, 以迂为直, in Sun Tzu's chapter on manoeuvring." Make the same changes in `zh/chapter-07.md` and `zh/appendix-c.md`.

The *Safe Haven* sentence in ch. 17 is fair as it stands.

### 1c. Jamie Mai and the failed pre-registered test (against *The Counted Trade*)

**Finding 7 — no change needed. The numbers are accurate.** Every figure matches *The Counted Trade* exactly:

- **The test (ch. 15):** 2020–2025, 580 trades, twelve-month calls struck 30% out of the money, bought when realised volatility sat at a three-year low; about $0.58 back per $1; about 88% expired worthless; the same calls on ordinary stocks did about the same. This matches CT ch. 12 and ch. 25.
- **The stock-to-options study (ch. 5):** 87 cases, 10 tradeable, 1 winner. This matches CT ch. 6.
- **The rate decisions (ch. 12):** 38 decisions, median move below the priced straddle. This matches CT ch. 9.
- **The short-interest screen (ch. 15):** a short ratio "above 100%". CT ch. 14 says 117%, so this is consistent.
- **The pilot (ch. 16):** one spread +148%, median −94%. This matches CT ch. 29.

The framing is fair. The quiet stock was Mai's entry condition, not his edge, and "A screen can find quiet. It cannot borrow the eye that knows which quiet is load-bearing." That is the CT finding, credited as CT's.

**Finding 8 — SHOULD.** Nowhere does the book say where the pre-registration can be seen. A reader who wants to check "written down before the first run, and nothing was changed after" has nothing to check against. Add one line to appendix C pointing to the record (the CT chapter, or the dated document or repository).

**Finding 9 — SHOULD. "Risk one to make ten" is put in Mai's mouth.** In ch. 4 v. 25 and the commentary ("Mai's 'risk one to make ten' … In Schwager's interview the one comes first"), in ch. 8 commentary ("Mai's practice of risking one to make ten, as Schwager records it") and in appendix A no. 19, the phrase reads as a quotation from the interview. Confirm that the words are in *Hedge Fund Market Wizards*. If they are your summary, drop the quotation marks and the "as Schwager records it", and use the paraphrase ch. 15 already uses: "risk a little to make a lot".

**Finding 10 — SHOULD.** Ch. 15 commentary says "Jamie Mai is the clearest modern example of a buyer who attacked only on these grounds." Neither source says he attacked *only* on these five grounds, which are this book's own categories. Suggested: *"Jamie Mai, as Schwager and Lewis tell it, is one of the clearest modern examples of a buyer whose attacks fit these grounds."* Same fix in zh ("最清楚的现代例子" → "最清楚的现代例子之一").

### 1d. The Lewis anecdote

**Finding 11 — no change needed in the main telling (ch. 15 commentary, "the second voice").** It is introduced with "As Lewis tells it" and "In Lewis's telling". The facts match *The Big Short*'s Cornwall chapter:

- a small starting account;
- an early trade in long-dated calls on a lender whose fate hung on regulators (Lewis names Capital One; the book rightly does not need to);
- the options market pricing a smooth range where the outcome was really two-way;
- the later purchase of default insurance on the higher-rated slices of mortgage bonds.

**Finding 12 — SHOULD.** Two clauses in that paragraph sit outside the attribution, and they read as your own statement of fact:

- "which the sellers of that insurance priced as if they could not fail". Write "which, in Lewis's account, the sellers priced as if they could not fail."
- In the next paragraph, "His edge was the judgement of a particular event: which court, which regulator, which balance sheet". This is an interpretation, shared with CT. Write "As both books tell it, his edge was …".

**Finding 6 — MUST: verify or cut.** Ch. 12 commentary ¶6 says: "The second fire, the business sold below what it can be worth, is Mai's territory as Lewis describes it in *The Big Short*: no volatility screen finds it; it is read in the balance sheet." CT ch. 5 makes the same claim ("Lewis describes Mai and his partner looking for exactly this, businesses the crowd had sold past what they could be worth"). The Cornwall story as I know it is about binary outcomes, and about options that underprice large moves. It is not a deep-value or solvency hunt read from filings. Unless you can point to the page, the safe fix is to keep the idea and drop the attribution: *"The second fire, the business sold below what it can be worth, is not a volatility trade: no screen on the chain finds it; it is read in the balance sheet."* Make the same change in `zh/chapter-12.md` ("是刘易斯在《大空头》里所写的麦的地盘" → delete), and correct CT ch. 5 to match.

---

## 2. Accuracy

### Sun Tzu quotations

I checked every verse and italic passage that quotes the general: English against Giles (1910), Chinese against the received text (通行本 / 十一家注本). Most are verbatim or clearly marked adaptations. These are the exceptions.

**Finding 2 — MUST.** `en/chapter-10.md` v. 10:

> "When troops flee, are insubordinate, collapse, are disorganised, or are routed, it must be due to natural causes in the general."

Giles X.14 says the opposite: "an army is exposed to six several calamities, not arising from natural causes, but from faults for which the general is responsible." The Chinese verse has it right: 非天之灾，将之过也. Fix: *"When troops flee, are insubordinate, collapse, are disorganised, or are routed, it is not a calamity from natural causes but a fault of the general."*

**Finding 3 — MUST.** Ch. 1 v. 3, both editions.

- EN: "These are: the Sky, the Ground, the Commander, the Method, and the Cause."
- ZH: "五事者：一曰天，二曰地，三曰将，四曰法，五曰道。"

Sun Tzu's order is 一曰道，二曰天，三曰地，四曰将，五曰法 (Giles: Moral Law, Heaven, Earth, Commander, Method and discipline). Re-ordering for the trade is a fair choice. But the Chinese uses the general's exact formula with the order changed, which any Chinese reader will catch, and the commentary ("The Cause is placed last because it is the quietest") hides that the general put it first.

Fix:

- Keep the received order in the verse: ZH 一曰道，二曰天，三曰地，四曰将，五曰法; EN "the Cause, the Sky, the Ground, the Commander and the Method". Then read them in the book's order.
- Or keep the order and change the commentary to: *"The general put the Cause first. This book reads it last, because it is the quietest."* ZH: 将军把道放在第一；本书把它放在最后读，因为它最安静。

**Finding 13 — SHOULD.** `zh/chapter-09.md` v. 1: "处高阳而战，无登高而战。此处山之军也。" This is a back-translation of Giles into classical style, not the received text. Appendix C says the Chinese follows the received text. Fix: 视生处高，战隆无登，此处山之军也。

**Finding 14 — SHOULD.** `zh/chapter-07.md` v. 7: "其疾如风，其徐如林。砍仓要疾。仓位要密。" 徐 means measured or slow; it does not mean compact (密 comes from Giles's "compactness"). Fix: 砍仓要疾，入场要徐。 The English "Be rapid in cutting. Be compact in size." can stay as it is, since it follows Giles.

**Finding 15 — NOTE.** Small wording departures from Giles in adapted verses. None is presented as a quotation, so they are fine:

- ch. 5 v. 7 "timing is the release of the trigger" (Giles: "decision");
- ch. 6 v. 7 "like water" (Giles: "like unto water");
- ch. 4 v. 1 "to defeat" (Giles: "of defeating");
- ch. 3 commentary "supreme excellence is to win without fighting" (Giles: "breaking the enemy's resistance without fighting").

Ch. 1 v. 11, "All trading is based on positioning", adapts the most famous line in the book ("All warfare is based on deception") and changes its meaning. That is a fair choice, but consider one clause in the commentary saying so.

The verbatim italic or standalone quotes all match Giles: ch. 4 v. 17; ch. 14 v. 1; ch. 15 vv. 1, 3, 10, 12, 13, 29 and its commentary; ch. 16 v. 1; ch. 17 vv. 1, 3; ch. 18 vv. 1, 3.

**Finding 16 — NOTE.** Two Chinese passages follow common variant readings:

- ch. 13 v. 4 has 乡间. The 十一家注 text reads 因间; 乡间 is the standard emendation.
- ch. 6 v. 7 has 水之行. The 十一家注 text reads 水之形.

Both are defensible. Pick one edition and stay with it.

**Finding 17 — NOTE.** 守则不足，攻则有余 (ch. 4 v. 12 and v. 17, ch. 15 v. 3) is the received text, and Giles translates it. The Yinqueshan bamboo slips (银雀山汉简) read the reverse, 守则有余，攻则不足. Part V builds its argument on this line, so one footnote in appendix C would forestall a learned reader.

### The Thirty-Six Stratagems (appendix A)

**Finding 18 — NOTE: the names and numbers are correct.** All 36 names, all numbers (第1计–第36计), and all six set names (胜战、敌战、攻战、混战、并战、败战) are correct, in both languages. Every number cited in a chapter matches its stratagem.

No. 14's image ("The dead man is carried home…") is not the traditional story (Li Tieguai's soul entering a beggar's corpse). Appendix C does say the images are yours, so this is fine.

**Finding 19 — SHOULD. Six stratagems are never cited in a chapter.** Nos. 23, 24, 25, 26, 27 and 29 are never cited by number in any chapter, yet their "In this book" lines point to chapters (no. 23 → Chapter 5; no. 25 → Chapter 15; no. 29 → Chapter 16). This clashes with the prologue's "each cited by its number". Either add the citation in those chapters, or change those six lines to "the idea appears in Chapter N".

### Options statements that are wrong or misleading

**Finding 4 — MUST.** `zh/chapter-15.md`, commentary, the five sentences: "一张十赔一的单子，需要十一次里赢一次". In Chinese, 十赔一 means risking ten to win one, which is the opposite of what is meant. Fix: 一赔十的单子，十一次里赢一次才打平。

**Finding 20 — SHOULD. "Move" and "straddle" are used inconsistently between ch. 14 and ch. 15.** Ch. 14 separates the two: the one-standard-deviation move is price × vol × √t, so "about 4.5", and the straddle is 0.8 × that, so "about 3.6". Ch. 15 calls the straddle figure the move: "The straddle costs about … 4.6. That is the size of move … the market is charging for", and "The same formula, with 0.30 … gives a typical move of about 6.9" (that 6.9 includes the 0.8). Fix in ch. 15: "That is roughly the average move, up or down, the market is charging for", and "…gives a straddle worth about 6.9." Same in zh ("得出的典型波幅约为6.9" → "跨式约值6.9").

**Finding 21 — SHOULD.** Ch. 14 commentary ¶4: "Over twenty trading days the difference compounds into the price of a straddle". Nothing compounds here; the gap scales with the square root of time. Fix: "Over twenty trading days the difference shows up in the price of a straddle." ZH "复合成" is fixed by rewrite no. 4 in 1a.

**Finding 22 — SHOULD.** Ch. 12 v. 14: "Only the wing is guaranteed to be where you left it." ZH: "只有保护腿，保证还在你放下它的地方。" This breaks the brand rule on "guaranteed" and claims more than is true: a wing is a contract, but the spread can still be assigned early or closed out by the broker. Fix: "Only the wing is still where you left it." / 只有保护腿，还在你放下它的地方。

**Finding 23 — SHOULD.** Ch. 17 commentary ¶2, the insurance example. The text says that with the put, "the loss is the 10 down to the strike plus the 1 paid for that quarter's put, about 11." The same paragraph says the year's puts cost about 4. Fix: "…plus what the year's puts have cost, somewhere between 11 and 14, and the book needs to rise by about an eighth to a sixth." Same in zh.

**Finding 24 — SHOULD.** Ch. 15 commentary, the shape of the attack: "pay 2 for a spread 10 wide, and he must be right one time in five, not one in ten." The "one in ten" refers to nothing. Fix: "…one time in five, not three in ten as at a debit of 3 (Chapter 8)."

**Finding 25 — NOTE.** Ch. 2 v. 20, "the daily decay, multiplied by the days he expects to wait, is the price of his patience", understates the cost, because decay speeds up near expiry. Add "and more, because the decay quickens near the end". Ch. 2 commentary and ch. 16 v. 6 ("a twentieth a day") are stylised rates; "suppose" before them would make that clear.

**Finding 26 — NOTE.** Ch. 14 annualises with 252 trading days and ch. 15 with 365 calendar days. Both are right, but say once (ch. 15 or appendix C) that the clock has to match the volatility you use.

I checked the rest of the arithmetic, all of it correct:

- the ten-day realised volatility (16.36 → 1.28% → about 20%);
- 0.8^10 ≈ 0.107, and the chance of a run of ten losses in 100 trades at a 20% hit rate (about 93%, so "better than nine in ten" is right);
- 0.98^10 ≈ 82%; 0.9^10 ≈ 35%; −65% needs +186%;
- the 100/110 spread (3, 7, 103, three in ten);
- ten to one needing one in eleven;
- the combined ratio of 82;
- the tail put at a hundred to one;
- the 1987, 2018 and 2020 market facts.

---

## 3. English against Chinese

**Counts.** Every file has the same number of non-empty lines and the same number of numbered verses in both languages: all 22 files plus the README. Both `the-whole-book.md` files contain every line of their chapters. There is no structural drift.

These are the places where the two editions say different things:

| # | Where | EN | ZH | Fix |
|---|---|---|---|---|
| 2 | ch. 10 v. 10 | wrong ("due to natural causes") | right (非天之灾，将之过也) | fix EN, see Finding 2 |
| 27 (NOTE) | ch. 7 v. 4 | quotes Giles VII.8, the forced march with a tenth of the army | quotes a different line, 举军而争利，则不及；委军而争利，则辎重捐 | either is fine; choose one |
| 14 | ch. 7 v. 7 | compactness | 徐 (slowness) glossed as 密 | fix ZH |
| 13 | ch. 9 v. 1 | Giles | not the received text | fix ZH |
| 4 | ch. 15 commentary | "ten to one" | 十赔一 (reversed) | fix ZH |
| 28 (SHOULD) | ch. 18 commentary, last ¶ | quotes the first edition's closing sentence word for word as in ch. 13 | quotes it in different words from zh ch. 13 ("哪一方都不是对的一方；每一方都是一种错法" against ch. 13's "没有哪一边是对的那一边。每一边都是一种可以活下来的犯错方式") | make the zh ch. 18 quote match zh ch. 13 |
| 29 (SHOULD) | prologue, last ¶ but one | "Nothing here is a performance claim." | "书中没有任何业绩承诺" (a promise, which is narrower than a claim) | use 业绩之言, as appendix C does: 书中没有任何业绩之言 |
| 30 (SHOULD) | ch. 15, last ¶ | "They make sure that…" | "它们保证的是……" (adds "guarantee") | 它们能做到的只是…… |
| 1 | Part V throughout | debit | 借方 used as a noun | see 1a |
| 1 | `zh/README.md` line 1 | none | 第五部分中文为初稿，待作者审定。 | remove after your pass |

---

## 4. Repetition left over from merging three books

Some echoes are deliberate: the same Sun Tzu line read from both banks, and the "neither side is the right side" sentence at the close. These are the ones that read as the same rule or the same story told again because three books were merged.

**Finding 31 — SHOULD. "Never stack a second position on the same direction" / "one bet in two costumes."** It appears in:

- ch. 4 v. 15; ch. 5 v. 25;
- ch. 7 vv. 14, 15 and 26, and commentary ¶6;
- ch. 15 v. 35 and the seller's paragraph of the commentary;
- ch. 18 v. 12 and commentary ¶5;
- appendix A no. 23; appendix B.

Ch. 18 says "it is said a third time here". It is closer to the tenth. Appendix B says the rule line is "said once, here, because the first edition and its companions said it too often", which is ironic at that count. Keep ch. 7 (the seller's day) and ch. 18 (the rule that does not turn), cut ch. 7 v. 26 and the ch. 15 commentary sentence, and change "a third time" to "again".

**Finding 32 — SHOULD. "He has been a buyer since Chapter 4."** It appears in ch. 14 v. 14, the ch. 15 commentary (the shield), ch. 17 v. 15 and twice in the ch. 17 commentary. Ch. 6 v. 29 and its last paragraph already make the same point. Keep it once, at the end of ch. 17, where it lands.

**Finding 33 — SHOULD. Mai's "two-humped world priced as one hump" is told in full three times:** ch. 3 v. 24 and commentary ¶7; ch. 13 v. 27 and commentary ¶6; ch. 15 v. 34 and the "second voice" paragraph. Keep ch. 3 (the first telling) and ch. 15 (the full one). Cut ch. 13 commentary ¶6 to one clause pointing back to ch. 3.

**Finding 34 — SHOULD. "Risk one to make ten"** appears in ch. 4 v. 25 and its commentary, ch. 8 commentary ¶6 and appendix A no. 19. Ch. 4 and ch. 8 each explain it from the start. Keep ch. 4 and let ch. 8 refer back to it.

**Finding 35 — SHOULD. The variance premium is stated as a fresh discovery four times:** ch. 6 commentary ¶4, ch. 14 commentary ¶2, ch. 15 commentary ¶4 and ch. 16 v. 4 with commentary ¶1. Each time the wording is close to "buyers of protection have usually paid more than the moves … turned out to cost". After ch. 6, point back rather than restate.

**Finding 36 — SHOULD. The five sentences are explained twice in nearly the same words.** Ch. 1 commentary ¶7 says each sentence closes a door and that the time stop "costs nothing to promise and something to keep". The ch. 15 commentary ("The five sentences are said here in full, once") repeats the door image and that clause word for word, right after vv. 22–27 have already stated the sentences. Keep the verses and cut the ch. 15 commentary paragraph to its last two sentences.

**Finding 37 — SHOULD. Temporising ground** ("Whoever moves first is charged for the information the other side is about to receive for free") appears word for word in ch. 10 v. 5, ch. 18 v. 7 and the ch. 18 commentary ¶2. Ch. 18 commentary already says "as Chapter 10 said", so cut the repeat in v. 7.

**Finding 38 — NOTE. "Let half the army get across"** is read in ch. 14 v. 10 and v. 17, and then again in commentary ¶7, which restates both verses.

**Finding 39 — NOTE. Ch. 16 seller section.** Vv. 21–24 are repeated almost word for word in the last commentary paragraph ("The buyers pay a little most days; the seller pays a lot on a few. Both columns … are real.").

**Finding 40 — NOTE. The Part V introduction paragraph** appears in the README, again as ch. 14 commentary ¶1, and in shorter form in the prologue. Repeating it in the README is normal. Ch. 14 could open on its second paragraph.

**Finding 41 — NOTE. Recovery arithmetic** (−50 needs +100) appears in ch. 5 v. 15 and commentary, ch. 12 v. 19 and commentary, ch. 16 and ch. 17. Ch. 12 says the later chapters point back to it. Most do, so this is fine.

---

## 5. Brand rules

**Finding 42 — no change needed: no employers named.** In either language I found no Innovent/信达, no TCW, and no other firm you have worked at. The only real organisations named are Lloyd's (as history) and publishers. Cornwall Capital is not named.

**Finding 43 — no change needed: no performance claims.** Every research number is the record of a test, most of them failed, and is labelled as such (appendix C). The pilot's +148% is always printed beside its −94% median; keep it that way in any excerpt.

**"Guaranteed" / 保证:** Finding 22 (ch. 12 v. 14, both languages) and Finding 30 (zh ch. 15). Ch. 6 commentary, "It is not guaranteed", is a denial and is fine.

**Finding 44 — SHOULD. These verses read as signals.** Ch. 9 v. 9 ("When the ATR trail flips, the trend has spoken. Sell puts beneath a market that ratchets up.") and v. 20 ("the buyer may follow it: calls behind a market that has turned up…") read as a mechanical entry rule. Add a few words saying this is a reading of structure, given as an example, not a signal. For instance, v. 9: "When the ATR trail flips, the trend has spoken, as this book reads trend." The zh needs the same. Ch. 18 vv. 5–6 (the seasons) could read as timing calls on their own, but v. 4 ("The wheel is read, not forecast") and the commentary cover them.

**Finding 45 — NOTE. "Edge."** The English uses "edge" 47 times. Every use treats it as something that must be stated as a price, or denies it is there ("No shape is an edge", "a description, not a signal"). None claims that you or the reader has one. I would leave it. If the brand rule bans the word itself, that is a change across the whole book, and the decision is yours.

---

## 6. Verdict

**Not ready yet, but close.** Parts I–IV and the appendices are ready in both languages. The structure matches line for line, the stratagems are right, the arithmetic checks out, and the Counted Trade figures are carried over exactly.

Four things must change first:

- The Part V Chinese needs your own pass. It is a sound translation, not yet your Chinese, and both READMEs make claims about it that are not yet true.
- Fix three accuracy errors: the inverted Sun Tzu line in en ch. 10, the re-ordered five constants in ch. 1, and 十赔一 in zh ch. 15.
- Reword the Spitznagel credit so it does not imply he left out a source he names himself.
- Verify the "business below what it can survive at" attribution to Lewis, or cut it.

After that, the SHOULD items are a day's work: mostly trimming the repeated rules and stories, the straddle and insurance wording in Part V, and the two uses of "guaranteed".

**Totals:** 45 findings: 6 must-fix, 23 should-fix, 16 notes. Five of the notes (7, 11, 18, 42, 43) confirm that something is right and needs no change.

---

## Fixed 2026-11-18

Applied on Henry's approval ("approve, fix", then "finish the book"). All six MUST findings and all 23 SHOULD findings are fixed in both languages. Of the NOTEs, only 17 and 25 were applied, as asked. The other notes are left as they were. After every change, both `the-whole-book.md` files were re-spliced from the chapters. The structure check passes: every file, including both READMEs and both whole-book files, has the same number of non-empty lines and of numbered verses in `en/` and `zh/`.

Commits: `fcf0e82` (MUST 2, 3, 4, 6), `336c1be` (MUST 5 and the Parts I–IV fixes), `fa0a90c` (Part V English), `8bfa4c5` (MUST 1, the Part V Chinese and the READMEs). *The Counted Trade*: `78385ba` (ch. 5).

### MUST

| # | Status | What was done |
|---|---|---|
| 1 | fixed | Chapters 14–18 in `zh/` are written again in Chinese, against the final English. The verses use the terse register of Parts I–IV, and the commentary follows Chinese word order. The ten suggested rewrites and the three after them are used, some lightly changed. The money is 权利金 or 所付之数, and 借方 appears only in 借方价差. The wing is 翼 or 保护腿, and the surviving spy is 生间, as in Parts I–IV. The `zh/README.md` banner is removed. The `README.md` paragraph now says the two editions were written separately and that the Chinese is written as Chinese, not machine-translated; "written by hand" is gone. **Henry has not read the new Chinese yet.** |
| 2 | fixed | en ch. 10 v. 10: "it is not a calamity from natural causes but a fault of the general." |
| 3 | fixed | Ch. 1 v. 3 keeps the received order in both languages. The commentary says the general put the Cause first and this book reads it last. |
| 4 | fixed | zh ch. 15: 一赔十的单子，十一次里赢一次才打平。 |
| 5 | fixed | Ch. 7 ¶2 and appendix C, both languages, now use the suggested text. Spitznagel takes the name from the Austrian economists and traces the idea himself to Laozi and Chinese strategy. 以迂为直 is "one of its clearest early statements", not the oldest, and the sentence 这份功劳应当记在将军名下 is gone. *That he makes the Laozi connection himself rests on this memo's recollection; check it against your copy.* |
| 6 | fixed | Ch. 12 ¶6, both languages: the attribution is cut and the idea kept. *The Counted Trade* ch. 5 is corrected the same way, in en, zh and both whole-book files. The repository was unarchived for the push and archived again. CT ch. 6 has a second, milder Lewis line ("Lewis describes Mai buying the cheapest thing that expressed a view"); it fits the Cornwall story and was left. |

### SHOULD

| # | Status | What was done |
|---|---|---|
| 8 | fixed | Appendix C now points to the record: *The Counted Trade*, Chapters 12 and 25, in its public repository. Neither repository holds a separate dated pre-registration document. If one exists, link it there. |
| 9 | fixed | Schwager's book could not be checked, so the safe path was taken. Ch. 4 commentary and ch. 8 commentary drop the quotation marks and "as Schwager records it", and use the paraphrase "risking a little to make a lot" (以小博大). Ch. 4 v. 25 and appendix A no. 19 keep "Risk one to make ten" as the book's own maxim, unquoted and unattributed. |
| 10 | fixed | Ch. 15: "Jamie Mai, as Schwager and Lewis tell it, is one of the clearest modern examples of a buyer whose attacks fit these grounds" (zh 最清楚的现代例子之一). |
| 12 | fixed | "which, in Lewis's account, the sellers priced as if they could not fail". The edge sentence reads "As this book and *The Counted Trade* both read him, his edge was…" instead of "As both books tell it", because the reading belongs to this book and CT, not to Schwager or Lewis. |
| 13 | fixed | zh ch. 9 v. 1: 视生处高，战隆无登，此处山之军也。 |
| 14 | fixed | zh ch. 7 v. 7: 砍仓要疾，入场要徐。 |
| 19 | fixed | The six "In this book" lines for nos. 23–27 and 29 now say "the idea, not the number" (zh 不标计数). |
| 20 | fixed | Ch. 15: "roughly the average move… the market is charging for" and "a straddle worth about 6.9" (zh 跨式约值6.9). |
| 21 | fixed | Ch. 14: "shows up in the price of a straddle". The zh uses rewrite no. 4. |
| 22 | fixed | Ch. 12 v. 14: "Only the wing is still where you left it." / 只有保护腿，还在你放下它的地方。 |
| 23 | fixed | Ch. 17: "plus what the year's puts have cost, somewhere between 11 and 14… about an eighth to a sixth." The same in zh. |
| 24 | fixed | Ch. 15: "not three in ten as at a debit of 3 (Chapter 8)". |
| 28 | fixed | zh ch. 18 now quotes zh ch. 13 exactly: 没有哪一边是对的那一边。每一边都是一种可以活下来的犯错方式——只要算过。 |
| 29 | fixed | zh prologue: 书中没有任何业绩之言。 |
| 30 | fixed | zh ch. 15: 它们能做到的只是…… |
| 31 | fixed | Ch. 7 v. 26 is cut (old v. 27 is now v. 26), the two sentences in the ch. 15 seller's paragraph are cut, and ch. 18 says "again". Appendix B's "said once, here" is left. It is about the seller's rule line as a whole, which does still appear once there. |
| 32 | fixed | Cut from ch. 14 v. 14, the ch. 15 shield paragraph and ch. 17 v. 15. Kept once, at the end of ch. 17. |
| 33 | fixed | Ch. 13 commentary now has one clause pointing back to ch. 3. Ch. 3 and ch. 15 keep the full telling. |
| 34 | fixed | Ch. 8 now points back to ch. 4 instead of explaining it again. |
| 35 | fixed | Ch. 14 ¶2, ch. 15 ¶4 and ch. 16 v. 4 and ¶1 now point back to Chapter 6 instead of restating it. |
| 36 | fixed | The ch. 15 paragraph is cut to a pointer to the verses and Chapter 1, plus the breakeven arithmetic. The time-stop clause was dropped too, because it was the word-for-word repeat. |
| 37 | fixed | The repeat is cut from ch. 18 v. 7. The ch. 18 commentary keeps "as Chapter 10 said". |
| 44 | fixed | Ch. 9 v. 9: "as this book reads trend". V. 20: "as a reading of structure and not a signal". The same in zh. |

### NOTE

| # | Status | Why |
|---|---|---|
| 7, 11, 18, 42, 43 | no change needed | These confirm the text is right. |
| 17 | applied | Appendix C, both languages: the Yinqueshan slips read 守则有余，攻则不足, and Part V rests on the received reading. |
| 25 | applied, in part | Ch. 2 v. 20 adds "and more, because the decay quickens near the end". "Suppose" before the stylised rates was not added, per the brief. |
| 15, 16, 26, 27, 38, 39, 40, 41, 45 | not applied | Your call, per the brief. |

### For Henry to read himself

All of Part V in Chinese: `zh/chapter-14.md` to `zh/chapter-18.md`. It is new text that no one but its writer has read. Read the verses first, against Parts I–IV. Then read the four places where the English changed underneath: ch. 15 (the straddle, the shape, the five sentences and Mai), ch. 16 vv. 4 and 19, ch. 17 ¶2, and ch. 18 v. 7 and the last paragraph.
