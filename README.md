# Brand Association Mapping HSE Marketing
Для составления ассоциативных карт (методология научных исследований в менеджменте: методы научных исследований в маркетинге, МНИМ, ВШЭ, ОП "Маркетинг")

NB! Russian language only!

The code here is written in Python 3 (Jupyter Notebooks), it helps build association maps for brands and other concepts (e.g., bar/pub, restaurant, coffeeshop).

Associations are gathered through means of consumer survey (an example of questionnaire can also be found in this repository).
It is recommended to have at least 15 complete forms. Each form contains 12 primary associated words, 36 secondary associations (3 for each primary word), and 36 tertiary associations (1 for each secondary word).
Each column in such a table contains aggregated primary, secondary and tertiary words associated with the main concept.

As an input one should use a csv-table of 3 columns (a combination of all filled forms). As an output one will get 2 csv-tables:
1) a table of word frequencies (in their basic forms) for each column. Only words that appear more than 1 time have counts, otherwise the corresponding cell is left blank.
2) a table of incident vertices for the planned graph (adjacency list). Graph can be visualized via Gephi

Credits:
preprocessig function for Russian text was adopted from https://www.kaggle.com/alxmamaev/how-to-easy-preprocess-russian-text
