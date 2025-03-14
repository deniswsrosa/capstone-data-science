Word Prediction App
========================================================
author: Denis Rosa
date: 2025-03-14
autosize: true
transition: rotate
class: smaller
css: style.css

Data Science Capstone Project<br />
Johns Hopkins University<br />

========================================================
# **Objective**

<small>
This presentation features the Next Word Predict app
including an introduction to the application user
interface and details about the text prediction
algorithm.

This presentation is part of the Coursera Capstone Project Milestone Report.
It features a word prediction app written using shine.
You can see the app at <a target="_blank" href="https://deniswsrosa.shinyapps.io/denis_capstone_data_science/">
https://deniswsrosa.shinyapps.io/denis_capstone_data_science/</a>
</small>


========================================================
# **The Application**

<small>
Next Word Predict is a Shiny application designed to anticipate the next word(s) a user might type by leveraging a text prediction algorithm.

The app suggests possible next words in a sentence through an n-gram model, which analyzes sequences of n consecutive words from a given text.

To develop the predictive model, a vast dataset comprising blogs, news articles, and Twitter posts was utilized. N-grams were extracted from this dataset and employed to enhance the accuracy of predictions.

Different techniques in natural language processing and text mining were explored to optimize both the speed and precision of the predictions.
</small>

========================================================
# **Model Prediction**

<small>
The predictive text model was developed using a sample of 800,000 lines sourced from a larger dataset of blogs, news articles, and Twitter content.

To prepare the data, it was tokenized and cleaned with the tm package, alongside various regular expressions applied via the gsub function. During this preprocessing stage, the text was converted to lowercase, and elements such as non-ASCII characters, URLs, email addresses, Twitter handles, hashtags, ordinal numbers, offensive words, punctuation, and extra whitespace were removed. The cleaned text was then segmented into tokens (n-grams).

When a user inputs text, the algorithm searches for matches by iterating from the longest n-gram (4-gram) down to the shortest (2-gram). The predicted next word is selected based on the longest and most frequently occurring matching n-gram. A simple back-off strategy is used to refine the prediction.
</small>

========================================================
# **Shiny App UI**

<div style="display: flex; align-items: center;">
  <div style="flex: 1;">
    <small>
      The app will display the predicted next word once it detects that you have completed typing one or more words.
      <br><br>
      As you enter text, please wait a few seconds for the predictions to generate. You can use the slider tool to choose up to three possible next words. The most likely prediction will appear first, followed by the second and third most probable suggestions.
    </small>
  </div>
  <div style="flex: 1;">
    <img src="images/screenshot.png" style="margin-left:20px" style="max-width: 100%;">
  </div>
</div>

