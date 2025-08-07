How It Works

1.	Loads the CNN/DailyMail dataset.
2.	Preprocesses the data by prefixing "summarize: " to each article.
3.	Trains t5-small for 3 epochs using beam search during generation.
4.	Evaluates on validation and test sets with ROUGE metrics.
5.	Generates summary for a specific test example.

 Example ROUGE Scores (on Test Subset)

 ## Training Results

| Epoch | Training Loss | Validation Loss | ROUGE-1 | ROUGE-2 | ROUGE-L | ROUGE-Lsum | Generated Length |
|-------|---------------|-----------------|---------|---------|---------|------------|------------------|
| 1     | 3.526400      | 3.052274        | 35.3409 | 10.7941 | 20.1728 | 20.1589    | 135.516          |
| 2     | 3.262300      | 3.009547        | 36.1050 | 11.1764 | 20.6751 | 20.6653    | 138.058          |
| 3     | 3.229600      | 2.998999        | 36.3396 | 11.3333 | 20.7175 | 20.7076    | 139.839          |


 Original Text:

Voters in 11 states will pick their governors tonight, and Republicans appear on track to increase their numbers by at least one, with the potential to extend their hold to more than two-thirds of the nation’s top state offices.Eight of the gubernatorial seats up for grabs are now held by Democrats; three are in Republican hands. Republicans currently hold 29 governorships, Democrats have 20, and Rhode Island’s Gov. Lincoln Chafee is an Independent.
Polls and race analysts suggest that only three of tonight’s contests are considered competitive, all in states where incumbent Democratic governors aren’t running again: Montana, New Hampshire and Washington.While those state races remain too close to call, Republicans are expected to wrest the North Carolina governorship from Democratic control, and to easily win GOP-held seats in Utah, North Dakota and Indiana.Democrats are likely to hold on to their seats in West Virginia and Missouri, and are expected to notch safe wins in races for seats they hold in Vermont and Delaware.

Generated Summary (Output)

Republicans in 11 states will pick their governors tonight, and Republicans appear on track to increase their numbers by at least one, with the potential to extend their hold to more than two-thirds of the nation’s top state offices.Eight of the gubernatorial seats up for grabs are now held by Democrats; three are in Republican hands.
