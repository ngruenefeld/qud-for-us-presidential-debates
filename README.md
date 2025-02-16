<h1 align="center" id="title">QUD Parsing for Political Science</h1>

<p id="description">The code for this project is provided in ipynb notebooks. Each step of our implementation is contained in it's own notebook. Manual steps must be done by directly editing the generated csv files containing individual debates. Follow the following steps to reproduce our results from scratch:</p>

<h2>Reproduction Steps:</h2>

<p>1. Data Acquisition</p>

```
Download US presidential debate transcripts from Martherus et al. (2020) https://github.com/jamesmartherus/debates
```

<p>2. Data Preparation</p>

```
Execute the script us_debates_dataset.ipynb (providing the correct filepaths)
```

<p>3. Question Assignment</p>

```
Create a new column in each individual debate csv named "question". For all direct responses of the candidates to a moderator question paste the corresponding moderator question into the question column of the corresponding row.
```

<p>4. QUD Parsing</p>

```
Execute the script us_debates_qud_parsing.ipynb
```

<p>5. Question Cleaning</p>

```
Execute the script us_debates_question_cleaning.ipynb
```

<p>6. Embedding Differences</p>

```
Execute the script us_debates_embedding_difference.ipynb
```

<p>7. QUD Alignments</p>

```
Create two new columns in each individual debate csv named "qud_answer_fit" and "qud_question_fit". For every row with a clean question and direct response fill these columns according to our alignment scale.
```

<p>8. Evaluation</p>

```
Execute the script us_debates_metrics.ipynb
```