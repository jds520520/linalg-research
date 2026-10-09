# Modeling a Polar Food Web with Adjacency Matrices

A linear algebra project that uses matrix powers to measure which
species dominate a ten-species marine food web.

## Question
Which species have the most influence in the food web once indirect
(two-step) feeding relationships are counted along with direct ones?

## Method
- Built a 10 × 10 adjacency matrix M, where an entry of 1 means the
  row species eats the column species
- Computed M² to count two-step paths (a predator's prey's prey)
- Summed A = M + M² and used row and column sums as dominance scores

## Findings
- The orca has the highest dominance score: 12 direct and two-step
  paths to other species, twice the next-highest score of 6
- Plankton and krill have no dominance and the most paths leading to
  them (10 each), which marks them as the base of the web
- Arctic cod and silverfish are the main link between the base and
  the predators above them

## Limitations
- The species list combines Arctic animals (polar bear, walrus,
  Arctic cod) with Antarctic ones (penguin, leopard seal), so the web
  is a simplified teaching model and not one real ecosystem
- All feeding links are weighted equally, and only ten species are
  included

## Files
- The full report (PDF)

Completed as a class project at Korea International School.
