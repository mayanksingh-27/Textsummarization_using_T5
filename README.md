How It Works
	1.	Loads the CNN/DailyMail dataset.
	2.	Preprocesses the data by prefixing "summarize: " to each article.
	3.	Trains t5-small for 3 epochs using beam search during generation.
	4.	Evaluates on validation and test sets with ROUGE metrics.
	5.	Generates summary for a specific test example.

 Example ROUGE Scores (on Test Subset)
 {
  "rouge1": 42.15,
  "rouge2": 19.73,
  "rougeL": 35.85,
  "gen_len": 132.4
}

 Original Text:

Voters in 11 states will pick their governors tonight, and Republicans appear on track to increase their numbers by at least one, with the potential to extend their hold to more than two-thirds of the nation’s top state offices.Eight of the gubernatorial seats up for grabs are now held by Democrats; three are in Republican hands. Republicans currently hold 29 governorships, Democrats have 20, and Rhode Island’s Gov. Lincoln Chafee is an Independent.
Polls and race analysts suggest that only three of tonight’s contests are considered competitive, all in states where incumbent Democratic governors aren’t running again: Montana, New Hampshire and Washington.While those state races remain too close to call, Republicans are expected to wrest the North Carolina governorship from Democratic control, and to easily win GOP-held seats in Utah, North Dakota and Indiana.Democrats are likely to hold on to their seats in West Virginia and Missouri, and are expected to notch safe wins in races for seats they hold in Vermont and Delaware.

Generated Summary (Output)

Republicans in 11 states will pick their governors tonight, and Republicans appear on track to increase their numbers by at least one, with the potential to extend their hold to more than two-thirds of the nation’s top state offices.Eight of the gubernatorial seats up for grabs are now held by Democrats; three are in Republican hands.
