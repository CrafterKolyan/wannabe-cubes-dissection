# Wannabe Cube Dissection
(Original video)[https://youtu.be/bHHVXD3pbJQ?si=qmWNOmCML-XWdQVC]

## Wannabe Cube
Wannabe cube is cuboid with sequential integer lengths (e.g. $41 \cross 42 \cross 43$)

## Questions
### Question A
Is there any dissection of 3D wannabe cube by smaller *distinct* wannabe cubes apart from cuboid $5 \cross 6 \cross 7$?

### Question B
Can 41x42x43 wannabe cube be dissected?

## Answers
### Question A (not solved)
All 3D cuboids up to $45 \cross 46 \cross 47$ can't be dissected in smaller cuboids except for $5 \cross 6 \cross 7$.

### Question B
No, it can't be dissected. Prove by program which uses SAT solver under the hood.

## Dependencies
- `z3`
- `numpy` (can be removed after refactoring of answer printing, nothing really important depends on it)
- `more-itertools` (can be removed by changing `more_itertools.distinct_permutations` to `itertools.permutations`, but don't want to use unoptimized `permutations` function)

## Installation
```bash
pip install -r requirements.txt
jupyter notebook
```
Run all cells in `main.ipynb` notebook.