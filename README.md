# Wannabe Cube Dissection
[Original video](https://youtu.be/bHHVXD3pbJQ?si=qmWNOmCML-XWdQVC)<br>
[Solution to question B](main.ipynb)

## Wannabe Cube
Wannabe cube is cuboid with sequential integer lengths (e.g. $41 \times 42 \times 43$)

## Questions
### Question A
Is there any dissection of 3D wannabe cube by smaller *distinct* wannabe cubes apart from cuboid $5 \times 6 \times 7$?

### Question B
Can $41 \times 42 \times 43$ wannabe cube be dissected?

## Answers
### Question A (not solved)
All 3D cuboids up to $45 \times 46 \times 47$ can't be dissected in smaller cuboids except for $5 \times 6 \times 7$. 43rd-45th wannabe cubes are not shown in the notebook in the repository but were checked by running code in the notebook for them separately.

### Question B
No, it can't be dissected. Prove by program which uses SAT solver under the hood.<br>
See [main.ipynb](main.ipynb) for details.

## Dependencies
- `z3`
- `jupyter` (can be removed by refactoring into the script)
- `tqdm` (can be removed by removing progress bar)
- `numpy` (can be removed after refactoring of answer printing, nothing really important depends on it)
- `more-itertools` (can be removed by changing `more_itertools.distinct_permutations` to `itertools.permutations`, but don't want to use unoptimized `permutations` function)

## Reproduction
```bash
pip install -r requirements.txt
jupyter notebook
```
Run all cells in `main.ipynb` notebook.