1.Data is extracted from Input.xlsx.
2. Creating a text file of stopwords from Url https://sraf.nd.edu/ 
3. we have to open Jupyter notebook and import required libraries
4. loading input excel file Input.xlsx
5. we have to extract title and content fro web page by using beautifulsoup
6. we now need to clean the extracted data and join it with data frame.
7. load stopwords from stopwords.txt file 
8. now filtering content using stopwords
9. Load a dictionary of positive and negative words
10. Now we have to perform data analysis.
11. 
1. We calculate below:

    a. Positive Score: This score is calculated by assigning the value of +1 for each word if found in the Positive Dictionary and then adding up all the values.

    b.Negative Score: This score is calculated by assigning the value of -1 for each word if found in the Negative Dictionary and then adding up all the values. We multiply the score with -1 so that the score is a positive number.
    
    c. Polarity Score: This is the score that determines if a given text is positive or negative in nature. It is calculated by using the formula: 
        Polarity Score = (Positive Score – Negative Score)/ ((Positive Score + Negative Score) + 0.000001)
        Range is from -1 to +1
    
    d. Subjectivity Score: This is the score that determines if a given text is objective or subjective. It is calculated by using the formula: 
       Subjectivity Score = (Positive Score + Negative Score)/ ((Total Words after cleaning) + 0.000001)
       Range is from 0 to +1

2    Analysis of Readability:
     Analysis of Readability is calculated using the Gunning Fox index formula described below.
     
     a. Average Sentence Length = the number of words / the number of sentences

     b. Percentage of Complex words = the number of complex words / the number of words 
     
     c. Fog Index = 0.4 * (Average Sentence Length + Percentage of Complex words)

3    Average Number of Words Per Sentence:

        Average Number of Words Per Sentence = the total number of words / the total number of sentences

4    Complex Word Count:
        Complex words are words in the text that contain more than two syllables.

5    Word Count:
        We count the total cleaned words present in the text by 

6    Syllable Count Per Word:
        We count the number of Syllables in each word of the text by counting the vowels present in each word. We also handle some exceptions like words ending with "es","ed" by not counting them as a syllable.

7    Personal Pronouns:
        To calculate Personal Pronouns mentioned in the text

8    Average Word Length

        Sum of the total number of characters in each word/Total number of words

12. We have to save extracted text to text file with each file haveing same name as URL_ID.

13. we have to save dataframe into the csv file.

