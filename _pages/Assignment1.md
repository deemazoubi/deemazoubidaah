---
permalink: /Assignment-1/
title: "Assignment-1"
---


Exploring Language in Science Fiction Through Computational Analysis

Group Work: Deema and Jane

1. Background & Expectations


Before beginning our analysis, we expected science fiction to focus mainly on superpowers, aliens, creatures, supernatural characters, and futuristic technology. We imagined that the language would mostly reflect imaginative beings, extraordinary abilities, and space exploration. We were interested in seeing whether particular words would appear more frequently in the tags we associated with them, such as war in War, Mars in Mars, and space-related vocabulary in Space Travel. We started with the custom words already there (“robot”, "alien", "spaceship", "mars", "war"), then moved to random words that seemed relatable ("faculty", "creature", "sword", "power", "fight"), then moved to 2 sets of more categorized words: space related ("firmament", "void", "cosmos", "orbit", "atmosphere") and war related ("bombardment", "invasion", "fleet", "defense", "sovereignty").
We expected that words associated with war would appear most frequently in the War category and same for the other tags. We first analyzed the prewritten custom words and our results mostly supported this expectation: war had its highest relative frequency in the War tag, at 0.58 occurrences per 1,000 words. However, it also appeared frequently in Society, at 0.37, and Action, at 0.29. We were expecting to see war in Society because conflict is often represented in stories about social life and organization, and it was a nice validation when we saw it there.

<figure>
  <img
    src="{{ '/assets/images/figure%201.png' | relative_url }}"
    alt="Figure 1"
    style="max-width: 100%; height: auto;">

  <figcaption>Figure 1</figcaption>
</figure>

Words such as fleet, invasion, defense, bombardment, and sovereignty were the major words that shifted our understanding of science fiction. We were surprised to see how political the genre is beyond futuristic technology and imaginative creatures or going to mars/moon.

<figure>
  <img
    src="{{ '/assets/images/figure%202.png' | relative_url }}"
    alt="Figure 2"
    style="max-width: 100%; height: auto;">

  <figcaption>Figure 2</figcaption>
</figure>


2. Computational Insights
Patterns across our word groups
Computational analysis allowed us to compare word frequencies across many texts, tags, and historical periods without reading every book from beginning to end. Reading all the texts cover-to-cover would not have been feasible within our lifetime (especially knowing that the books were written in the old English). The notebook allowed us to explore the corpus and identify patterns that might have been difficult to notice by reading, one because the sample size will be too little, and two because we will most likely be too caught up in the storylines to notice any word occurrences.
Space-related vocabulary
We used our space-related vocabulary to explore how science fiction describes space and the universe, including both familiar scientific terms and more traditional or literary vocabulary.
The clearest pattern was the dominance of atmosphere. It was the most frequent word in this group across the tags, with a relative frequency of 0.17 occurrences per 1,000 words in Mars and 0.15 in Space Travel. It also appeared across Society, Action, and War.

<figure>
  <img src="{{ '/assets/images/figure%203.png' | relative_url }}"
       alt="Figure 3"
       style="max-width: 100%; height: auto;">
  <figcaption>Figure 3</figcaption>
</figure>

This was interesting because we initially associated the word most strongly with space exploration and the galaxy, but the results showed that it appeared in all five categories. The word could refer to the earth’s environment when used in War, Society or action, and maybe referring to the void in space when used in Space Travel and in Mars.
Orbit was another relatively prominent word, especially in Space Travel and Mars which makes sense since it’s mostly used to describe the planets orbiting the sun. In contrast, cosmos was among the least frequent words, with displayed relative frequencies of zero in Society and Mars. Firmament was also uncommon in most categories, although it reached 0.02 in Mars. We were expecting cosmos to perform better than firmament because we have only encountered it in the old English texts to mean sky. It was surprising because we expected words associated with the universe to be more prominent in science fiction. These findings showed us how much our results depend on the vocabulary we choose. The words selected for analysis shape the patterns we can discover.
Comparing historical periods
Comparing the space-related vocabulary in the 1800-1900 and 1950-1960 revealed interesting differences. Atmosphere remained dominant in both periods, but its displayed relative frequency was higher in the 1950-1960 subset for Mars, Space Travel, Society, and Action. War was the exception, with a higher displayed frequency in the earlier period.
We also noticed an interesting contrast between firmament and cosmos. In the 1950-1960 graph, firmament was displayed at zero across all five tags. In the 1800-1900 graph, cosmos was displayed at zero across all five tags. In the later period, cosmos appeared at 0.02 in Space Travel, 0.03 in War, and 0.01 in Society and Action. In the earlier period, firmament appeared at 0.01 in War.

<figure>
  <img src="{{ '/assets/images/figure%204.png' | relative_url }}"
       alt="Figure 4"
       style="max-width: 100%; height: auto;">
  <figcaption>Figure 4</figcaption>
</figure>

We couldn’t explain why this happened but maybe it was an adaptation of vocabulary. The differences could suggest that the vocabulary used to describe space may have varied between the two historical subsets. However, we cannot conclude that a word was completely absent simply because its displayed frequency was zero. Values may have been rounded, and differences in the books included in each subset may also have affected the results.
Military and political vocabulary
We had two custom word groups that explored words associated with power, conflict, and the universe. The group containing faculty, creature, sword, power, and fight helped us examine how words relating to abilities, beings, and conflict appeared across the tags. Power appeared relatively frequently across the categories, reaching 0.60 occurrences per 1,000 words in both Space Travel and War. In contrast, faculty was rare, while creature was somewhat more frequent in Mars which was unexpected. We expected it to have the highest frequency in Society or Action. 

<figure>
  <img src="{{ '/assets/images/figure%205.png' | relative_url }}"
       alt="Figure 5"
       style="max-width: 100%; height: auto;">
  <figcaption>Figure 5</figcaption>
</figure>

Our other group of words contained bombardment, invasion, fleet, defense, and sovereignty, which helped us explore the military and political dimensions of science fiction.
One of our clearest observations concerned invasion. In 1800-1900, its frequency reached 0.10 per 1,000 words in Mars and 0.07 in Space Travel, compared with 0.01 and 0.02, respectively, in 1950-1960. We kind of expected invasion to be dominant in Mars but we also assumed that Society would be the second one. It was weirdly interesting that it happened to be the last one since there are a lot of inventions in societies. 
In the late 19th century, the concept of space travel was tightly bound to imperialism and colonization and could be because 19th-century geopolitics revolved around empires invading and conquering territory, humans projected this onto Mars. However, by 1950, astronomy had proven Mars was a dead, desolate plane and the mystery was gone. Furthermore, the focus of space travel shifted from being invaded to active human exploration (the dawn of the Space Race).
We also found that fleet increased in the War tag from 0.07 to 0.15 across the two periods, raising questions about how military language changed over time. In the 19th century, a fleet was mostly ships on water but in the 1950s, the term expanded due to the emergence of air forces (fleets of bombers). Because warfare came to land, sea, air, and theoretical space, the word fleet became a much more dominant and versatile way to describe military might.
Unexpectedly, defense and bombardment had zero displayed frequency across tags in 1800-1900. In 1950-1960, defense ranged from 0.03 to 0.08, while bombardment appeared at 0.01 across all five tags. Following WWII and entering the cold war, global powers rebranded their military focus toward deterrence. For example, the US changed its Department of War to the Department of Defense in 1949 which could be the reason for the rise in the word defense in the 1950s reflecting a geopolitical landscape obsessed with containment, nuclear deterrence, and national defense strategies rather than outright colonial conquest.
Our analysis showed that science fiction included themes of military power, territorial control, and political authority alongside imaginative creatures and technological developments.

<figure>
  <img src="{{ '/assets/images/figure%206.png' | relative_url }}"
       alt="Figure 6"
       style="max-width: 100%; height: auto;">
  <figcaption>Figure 6</figcaption>
</figure>

What the computational approach revealed, and what it could not
Computational analysis helped us identify patterns across a large collection of texts by comparing word frequencies across tags and historical periods. For example, we might not have noticed the difference in the frequency of invasion between the two historical subsets if we had only read a few books.
However, the process was a bit challenging. We struggled with the notebook especially because we could not autosave our work to continue later, interpreting distinctive words, and finding custom word groups that clearly differentiated categories. More importantly, word frequencies lacked context. For example, fleet appeared frequently, but we could not determine how authors used it without examining individual passages. Similarly, words like war and invasion might reflect specific historical events that our results could not identify.
We also realized that authors from earlier periods might have used different vocabulary to express ideas we describe differently today. For example, we initially considered using superpower but questioned whether it accurately represented the language of our texts. This showed us that our analysis could overlook important concepts simply because we were unfamiliar with the words used to describe them.
This connects to Ted Underwood’s discussion of the risks of distant reading. Computational methods reveal patterns across many texts, but these patterns depend on our word choices, tags, and historical categories. Low word frequency does not necessarily mean a concept was unimportant, just as high frequency does not automatically reveal a story’s main themes.
With a smaller collection, we could have examined individual passages and explored the historical contexts behind our findings. We learned that computational analysis is useful for identifying patterns and generating questions, but close reading is necessary to understand those patterns and develop stronger interpretations.

<figure>
  <img src="{{ '/assets/images/figure%207.png' | relative_url }}"
       alt="Figure 7"
       style="max-width: 100%; height: auto;">
  <figcaption>Figure 7</figcaption>
</figure>

3. Transferability
This exercise taught us to think more carefully about language, historical context, and the assumptions we bring to data analysis. We learned to question whether our chosen vocabulary accurately represented the ideas we wanted to investigate, accounting for synonyms and changes in meaning across periods and contexts.
We can apply this lesson to future courses and research projects by treating patterns as starting points rather than conclusions. Instead of assuming that high word frequency proves something, we should investigate possible explanations, consider alternatives, and look for supporting evidence.
We also learned that computational and qualitative approaches complement each other. Computational analysis reveals broad patterns across large datasets, while close reading helps explain their meaning and historical or social context. Combining both approaches allows us to draw more careful conclusions.
This assignment showed us that data analysis is not entirely objective simply because it uses numbers. Our questions, word choices, and categories influence the results, so we must recognize both our assumptions and the limitations of our data.

4. Contribution & AI:
We began by each choosing a group of words, then analyzing our findings together. Afterward, we each analyzed an additional word group individually and discussed our observations and notes. We brainstormed our ideas together before organizing them into a complete essay.
We used ChatGPT to help us identify synonyms and alternative words that authors might have used during the historical periods we studied. We also used it to troubleshoot errors in our R code when needed. However, we discussed and interpreted our findings together to develop our own analysis and conclusions.


