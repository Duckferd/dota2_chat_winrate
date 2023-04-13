# dota2_chat_winrate
Quick Python/Jupyter Notebook Script to Compare User Wordcloud Vs. Winrate

## Table of Contents
- GitHub Main
- Introduction
- Usage
- Future Plans/Changelog
- Acknowledgements
- License

## GitHub Main 
- config.py
    - You may want to add this to your .gitignore (if forking). This file will contain the account_id that you are inputting to run the script. *Certain* people hate being targeted so keep them anynomous.
- derogatory_winrate.ipynb
    - Jupyter Notebook Python script that runs the account ID through OpenDota API and collects wordcloud information to compare to winrates
- stopwords.csv and filter-wordlist.csv
    - These files sort out the most commonly used words ("the", "and", etc.) that would otherwise be picked up and pollute the results. 

## Usage
- You will need to modify config.py to include the steam account ID of the user you are looking up
- Run the Jupyter Notebook file. It will generate a bar chart and scatterplot highlighting the account's most used words vs. win percentage.
    - You can change parameters such as min_cutoff to adjust how messy the generated graph is. Certain accounts talk a lot of smack, others are very quiet. 

## Future plans/Changelog
- Initial Commit on April 13th, 2023. 
- This project is currently on hiatus as main meme goal has been achieved.
- Future plans:
    - Potentially creating a sub-API out of the generated data and using Javascript libraries like plotly to create interactive charts
    - More varied datasets, including "top 10 trash talkers among teammates"

## Acknowledgements
- I would like to thank my good friends Tony and Ching for this project. Tony for the request/inspiration and Ching for being the ~~target~~ good natured test subject. 

## License
- MIT license