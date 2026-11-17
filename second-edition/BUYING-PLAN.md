# The Art of Options War: a plan for the buyer's half

A working plan for the second edition. It is not part of the book and not a chapter file. The chapter files in `en/` and `zh/` are still generated from the app edition, and any text here goes into the book there.

This book is education, not advice. Nothing in this plan or in the draft chapter recommends a trade or promises a result.

## 1. The gap

### What already exists

The book is less one-sided than it was. The 9 November edition gave each of the thirteen chapters a **The Buyer** section after **The Seller**, with commentary on both. It added the buyer's five sentences (edge, catalyst, maximum loss, time stop, breakeven win rate), the time stop, the ladder of entries, cheap volatility in place of rich, and the warning against buying the spike. The companion book [The Counted Trade](https://github.com/henryzhangpku/the-counted-trade) covers the buyer at full length in thirty-six stratagems.

So the problem is no longer that the buyer is missing. The problem is that **the buyer is a mirror, not a combatant.** He shows up after the seller in every chapter and is described as the seller turned inside out.

### Where the book is still one-sided

| Where | What it says | Why it tilts |
|---|---|---|
| Part I intro | "the one idea that turns the whole book: the highest skill is to win without fighting — to be paid without having to be right." | It crowns the seller's thesis as the book's thesis. |
| Ch. 1 commentary | "The rest of this book assumes the second man" (the one paid to hold a line). | This is said outright, and nothing later takes it back. |
| Ch. 2, v. 2 | "The seller collects the rent. This is the whole of the seller's advantage." | The buyer is introduced as the one who pays rent, never as the one who sometimes buys at a discount. |
| Ch. 3 commentary | "the seller's whole thesis… He has simply refused the fight the buyer insists on." | Buying is framed as insisting on a fight, not as choosing one. |
| Part II intro | "For the premium seller, that is the entire trade." | The buyer is added in a second sentence. |
| Ch. 4, v. 7 | "Let him stand on the defensive and be content." | Sun Tzu's next lines, on attack, are never read. |
| Ch. 9, v. 5 | "A seller who prefers the low ground and the dark is a buyer who has not yet noticed." | Here the buyer stands for a mistake. |
| Ch. 13 commentary | "Neither side is the right side." | The balance arrives in the last paragraph of the last chapter. |

### What the buyer sections do not cover

- **Hedging and insurance.** The only long option discussed at any length is the wing left after a cut. The book never looks at the protective put behind a stock book, or at the wing as insurance bought on purpose rather than kept by accident.
- **Convexity and tails.** There is no treatment of the cheap, far, long-dated option held for a rare event, or of why the seller's catastrophe is the buyer's harvest.
- **Implied against realised, measured.** "Buy cheap volatility" is stated but never computed. No worked comparison of the move an option charges for with the move the market is delivering.
- **Why most buyers lose, as one argument.** Theta, overpaying for volatility, wrong timing and size are spread across chapters 2, 6, 10 and 12. They are never set out together, with the discipline that answers each.
- **Shape.** Long single option, debit spread and straddle are named but never chosen between.
- **When to attack and when to defend.** This is the general's own question (Ch. IV: "Security against defeat implies defensive tactics; ability to defeat the enemy means taking the offensive"), and the book never asks it. Seller and buyer are the two sides of one battle. The price of the option (implied volatility against what is delivered) decides which side is paid, and so which side a trader should stand on, if either.

## 2. The fair case for buying

These are the arguments the new part must make in full, each with its limits stated in the same breath.

1. **Defined risk, paid in advance.** The debit is the whole risk. No gap, halt or margin call can enlarge it. The seller's spread is also capped, but at its width, and it can reach that cap overnight. The buyer's worst morning was settled at the time of purchase.
2. **Convexity and tail events.** A long option gains more for each further unit of the move. A put far out of the money, bought for a tenth of a point, can pay a hundred to one on a crash. That is checkable arithmetic, not a forecast. The cost is that most such options expire worthless, so the buyer must be able to fund the long wait. Index puts are usually the richest options on the board (skew), so the tail is cheap only where sellers have stopped charging for it.
3. **Cheap optionality around catalysts.** A dated event, bought before the crowd prices it, costs the rent of an ordinary week. The early buyer can be paid in two ways: by the move, or by the rise in the option's price as the date draws near. The late buyer pays the spike and receives the crush.
4. **Hedging.** A put behind stock, or a wing behind short premium, is insurance. It loses money on average by design, like house insurance, and pays for the survival of the sequence (Ch. 12: minus fifty needs plus a hundred).
5. **When implied is cheap against realised.** The edge, where there is one, is a price: the move the option charges for is smaller than the move the market is delivering. Usually the gap runs the other way, and that gap is the seller's wage. Sometimes it inverts, typically after a long calm. That inversion is the buyer's only open gate.
6. **Small-premium asymmetric bets.** If the debit is small, the buyer can be wrong many times and still be present on the day he is right. The breakeven win rate (debit ÷ payoff when right) is the number he must beat, and he must say it before paying.
7. **Buying as insurance for sellers.** Every defined-risk seller in this book already owns a long option: the wing. Seeing the seller as a buyer of the far wing makes the second edition one book, not two.

### Why most buyers lose

- **Theta.** Rent is charged every day, whether or not the move comes. An option that loses a twentieth of what is left each day is about half gone in two weeks.
- **Overpaying for volatility.** Implied volatility usually sits above what is later delivered (the variance premium). A buyer who pays the average price, on average, pays the seller's wage.
- **Wrong timing.** Buying after the move, buying into the pre-event spike, and buying without a date at all.
- **Size.** A low win rate means long losing runs. At a 20% hit rate, ten losses in a row is ordinary arithmetic. A buyer sized for a few attempts is beaten before his door opens.
- **The roll.** Rolling a dead thesis into next month pays rent twice on the same reason.

### The discipline that changes this

Each failure has a rule against it:

- Name the edge as a price: implied against realised, or a dated event the market has not priced.
- Buy no more time than the catalyst needs, and set a time stop.
- Size so that a long run of total losses is boring.
- Take profit in pieces, and never roll a reason that has died.
- Keep a journal that counts the forty losers beside the one winner.

None of this makes buying profitable. It removes the ways of losing that have nothing to do with the market.

## 3. Recommendation: a second edition, with a new Part V

**Recommend a second edition, not a companion volume.**

- **The companion already exists.** The Counted Trade is the buyer's full book. A third book on buying would split the reader and repeat the stratagems.
- **What is missing can only live here.** The missing piece is the meeting of the two sides: the price at which defence becomes attack, and the seller who is also a buyer. This book is the one that holds both sides of the ticket, so this is the only place that synthesis fits.
- **The format allows it without breaking the thirteen.** Sun Tzu's thirteen chapters stay in his order. Part V comes after *Spies* because the chapter on knowing comes before the choice of stance: you cannot choose between attack and defence until you have read the inward spy, implied volatility.
- **The app edition, PDF and EPUB already regenerate from one source,** so a second edition is a rebuild, not a reprint.

### Second-edition changes

**New Part V — Attack and Defence 《攻守》**, chapters 14–18, after Spies. In Part V, *The Buyer* section comes before *The Seller*, reversing the order of Parts I–IV, so the book's structure makes the argument.

**Reframing edits to Parts I–IV** (light edits; the thirteen keep their verses):

- **Part I intro:** "the highest skill is to win without fighting" becomes the seller's highest skill. Add a sentence saying the buyer's highest skill, to attack only where the enemy is unguarded, is the subject of Part V.
- **Ch. 1 commentary:** change "The rest of this book assumes the second man" to say the book follows both men and tells you which one to be in Part V.
- **Ch. 4:** add a buyer verse reading IV.5–7 in full (defence and attack as one sentence).
- **Ch. 9, v. 5:** soften so the buyer is not used as a figure of error.
- **Part II intro:** give the buyer his own sentence, not a second clause.
- **Ch. 13 commentary:** point forward to Part V.
- **README:** update both READMEs, "thirteen chapters" to "thirteen chapters and a Part V on attack and defence", and the Counted Trade README cross-link to match.

**Chinese.** The 中文 edition is written by hand, not translated. Part V needs Henry's own Chinese text. The 中文 titles below are suggestions only.

## 4. The new outline: Part V — Attack and Defence 《攻守》

> *The good fighter is able to secure himself against defeat, but cannot make certain of defeating the enemy.* — Sun Tzu, IV (Giles, 1910)

**Part V intro (draft).** The general's thirteen chapters are done. They taught the seller to make himself unbeatable and the buyer to survive his own arithmetic. They did not answer the general's own question: when to defend, and when to attack. Seller and buyer are not two trades. They are the two banks of one river, and the option's price is the water between them. When the price of fire is high, the defender is paid to stand. When it is low, the attacker is paid to cross. The last five chapters are about reading the water.

### 14. The Two Banks 《两岸》

Every option has two owners, and every premium is paid by one to the other. The chapter sets the seller and the buyer on opposite banks of one river and shows that each is the other's provisions. The seller forages on the buyer's need for protection and love of direction. The buyer forages on the seller's comfort after a long calm. The line of battle is implied volatility. Above the fire the market goes on to deliver, the defender is paid. Below it, the attacker is. The seller's spread is itself a short option and a long one: every seller in this book has been a buyer since Chapter 4, through the wing. The chapter ends the false choice between being "a seller" and "a buyer." A trader chooses a stance for a price, not an identity for a career.

### 15. When to Attack 《攻》 *(written: [en/chapter-15.md](../en/chapter-15.md))*

The general's lines on attack, read for the buyer: attack only unguarded places, and only with an advantage you can name as a price. Five grounds on which the buyer may attack:

- **cheap fire:** implied below realised
- **the dated door:** a catalyst bought before the crowd
- **the long night:** a tail priced as impossible
- **the shield:** insurance against one's own ruin
- **the gap-proof ticket:** a debit no open can enlarge

The chapter also covers the refusal of bait (the move on the screen), the choice of shape (single option, debit spread, both doors), and buying no more time than the catalyst needs. The seller reads it as a list of days he must not be found on the field.

### 16. The Attacker's Tax 《攻者之税》

Why most attacks fail. The variance premium is the seller's wage and therefore the buyer's tax: on most days and in most names, the option charges for more fire than comes. The chapter counts the four ways the tax is paid: rent (theta), paying the spike (overpaying for volatility), the late or dateless entry (timing), and the oversized debit (size). The fifth, the roll, pays rent twice on one reason. Each failure is paired with its discipline, and the chapter closes on the arithmetic of the losing run: at a 20% hit rate, ten losses in a row is ordinary. The buyer who has not sized for it has not been unlucky; he has been counted. The seller reads it as the source of his wage, and as the reason the wage is small.

### 17. The Wing in the Baggage Train 《辎重之翼》

Buying as defence. The protective put behind stock, the wing behind short premium, and the far tail bought as fire insurance are all buying in the service of survival, not profit. Insurance loses on average by design, and the chapter says so plainly. It then shows the arithmetic it buys: minus fifty needs plus a hundred, so a small regular expense that removes the minus fifty pays for the sequence, not for the trade. It covers how much insurance to carry, where it is cheap (where skew has forgotten the tail) and where it is dear (where every institution buys the same put), and the seller's rule restated as a buyer's one: leave a wing in every spread. The seller reads it as the chapter in which he learns he has been a buyer all along.

### 18. The Turn of the Wheel 《攻守之轮》

When to change sides. Defence and attack lead to each other like the direct and the indirect, a circle without end (Ch. V). The chapter reads the regimes:

- **Long calm with volatility starting to rise:** the attacker's season.
- **High volatility that has peaked and is falling:** the defender's season.
- **The hour before the number:** neither.

The trader with one account and both stances keeps one rule from Chapter 7 above all: never hold both on the same direction. A long call and a short put on one name are one bet. The journal, the surviving spy, decides the turn, because only a written count can say whether a stance has been paid. The book closes on its own sentence, enlarged: neither side is the right side; each is a way of being wrong that can be survived, if it is counted, and the skill is knowing which way of being wrong the price is paying for today.

## 5. Next steps

1. Henry reviews this plan and the Chapter 15 draft.
2. Draft Chapters 14, 16, 17 and 18 in the same format.
3. Write the Chinese Part V by hand.
4. Apply the reframing edits at the app edition and regenerate `en/`, `zh/`, the PDF and the EPUB.
5. Update both READMEs.

Sun Tzu quotations in Part V are from the Lionel Giles translation (1910), in the public domain.
